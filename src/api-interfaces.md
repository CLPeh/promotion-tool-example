# API and Grpc
- [Grpc](#grpc-promotionclient)
- [Management Grpc](#management-grpc-promotionclient)

## API 
### Grpc PromotionClient

|  API | Description | Request | Response |
| ------ | ------ | ------ | ------ |
| InsertPendingPromotionTransaction |  | InsertPendingPromotionTransactionRequest | InsertPendingPromotionTransactionResponse |
| DeletePendingPromotionTransaction |  | DeletePendingPromotionTransactionRequest | DeletePendingPromotionTransactionResponse |
| InsertSuccessPromotionTransaction |  | InsertPromotionTransactionRequest | InsertPromotionTransactionResponse |
| GetActivePromotions | Retrieve the active promotions | GetActivePromotionsRequest | GetPromotionsResponse |
| GetAvailablePrize | Retrieve available promotion prize | GetAvailablePrizeRequest | CommonResponse |
| FightPlayerPromotion |  | FightPlayerPromotionRequest | FightPlayerPromotionResponse |
| GetPendingPromotionTransaction |  | GetPendingPromotionTransactionRequest | GetPendingPromotionTransactionResponse |

### Management Grpc PromotionClient

|  API | Description | Request | Response |
| ------ | ------ | ------ | ------ |
| GetPromotionTerms |  | GetPromotionTermsRequest | GetPromotionTermsResponse |
| GetPromotionLite |  | GetPromotionLiteRequest | GetPromotionLiteResponse |
| GetPromotionById |  | GetPromotionByIdRequest | GetPromotionByIdResponse |
| GetPromotionCriteriaById |  | GetPromotionCriteriaByPromotionIdRequest | GetPromotionCriteriaByPromotionIdResponse |
| GetPromotions | Retrieve all the promotions | GetPromotionsRequest | GetPromotionsResponse |
| CreatePromotion | Create new promotion | CreatePromotionRequest | CreatePromotionResponse |
| UpdatePromotionById | Update specific promotion info by ID given | UpdatePromotionByIdRequest | UpdatePromotionByIdResponse |
| UpdatePromotionCurrencyById | Update promotion currency by ID given | UpdatePromotionCurrencyByIdRequest | UpdatePromotionByIdResponse |
| CancelPromotion | Update the promotion status to canceled | CancelPromotionRequest | CancelPromotionResponse |
| GetPromotionTransactions | Retrieve promotion transactions history | GetPromotionTransactionRequest | GetPromotionTransactionResponse |
| GetPromotionTransactionSummary | Retrieve promotion transactions summary | GetPromotionTransactionSummaryRequest | GetPromotionTransactionSummaryResponse |
| GetPlayerPromotionTransactions | Retrieve player promotion transaction | GetPlayerPromotionTransactionRequest | GetPlayerPromotionTransactionResponse |
| GetConstPromotionType |  | GetConstPromotionTypeRequest | GetConstPromotionTypeResponse |
| GetPromotionWinSummary |  | GetPromotionWinSummaryRequest | GetPromotionWinSummaryResponse |
| GeneratePrize |  | GeneratePrizeRequest | GeneratePrizeResponse |
| GeneratePrizePreview |  | GeneratePrizePreviewRequest | GeneratePrizePreviewResponse |
| GetPrizePoolByPromotionId | Retrieve promotion prize pool by ID given | GetPrizePoolByPromotionIdRequest | GetPrizePoolByPromotionIdResponse |
| GetPrizePoolListByPromotionId | Retrieve promotion prize pool list by ID given | GetPrizePoolListByPromotionIdRequest | GetPrizePoolListByPromotionIdResponse |
| GetPrizeDistributionCountByPromotionId | Retrieve prize distribution count by ID given | GetPrizeDistributionCountByPromotionIdRequest | GetPrizeDistributionCountByPromotionIdResponse |
| VerifyAndGetPromotionNotification |  | GetPromotionTransactionRequest | VerifyAndGetPromotionNotificationResponse |
| ExportPromotionInfoRequestData |  | ExportPromotionInfoRequestDataRequest | ExportPromotionInfoRequestDataResponse |
