# API Information
- [Grpc](#grpc-promotionclient)
- [Management Grpc](#management-grpc-promotionclient)
- [API Involved in Other Services](#api-involved-in-other-services)

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


## API Involved in Other Services  
Click [here](https://viewer.diagrams.net/#G1tbxrTbyO1cFPmTHQ1eRPHUOAm7aWiNSt) to view the promotion service relationship diagram.
<details><summary> Game Workflow </summary> 
  
trigger promotion win during game spin  

**Bet**  
Get Active Promotions  
Get Available Prize  
Fight Player Promotion  
Insert Pending Promotion Transaction  
Insert Success Promotion Transaction  
Delete Pending Promotion Transaction  
Get Pending Promotion Transaction  

  </details>

<details><summary> Game Proxy </summary> 
  
view promotion details directly from game  
  
**Bet Management**  
Get Promotions  
Get Promotion Transactions  
Get Promotion Terms  
Get Promotion Lite  
Get Player Promotion Transactions  
  
  </details>

<details><summary> Message Hub </summary> 
  
provide winning notif in game  
  
**Bet Management**  
Verify And Get Promotion Notification
  
  </details>
  
<details><summary> Back Office </summary> 
  
manage promotions (create, view, update, cancel)  
  
**Bet Management**  
Get Promotion By Id  
Get Promotions  
Create Promotion  
Update Promotion By Id  
Update Promotion Currency By Id  
Cancel Promotion  
Get Promotion Transactions  
Get Promotion Transaction Summary  
Get Const Promotion Type  
Get Promotion Win Summary  
Generate Prize  
Generate Prize Preview  
Get Prize Pool By Promotion Id   
Get Prize Pool List By Promotion Id  
Get Prize Distribution Count By Promotion Id  
Get Promotion Criteria By Id  
Export Promotion Info Request Data  
  
  </details>

<details><summary> Job Reporting </summary> 
  
prepare reports regarding promotion win amount to bet amount ratio (or RTP)  

**Bet Management**  
Get Promotions
  
  </details>
