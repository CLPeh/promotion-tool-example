# API and Interfaces

## API Endpoints
`/promotionTool/{{action}}` : This endpoint is for promotion-related operations

|  Endpoints | Description | Parameter | Response |
| ------ | ------ | ------ | ------ |
| GET /promotionTool<br>/GetPromotions | Retrieve a list of all promotion. | None<img width=400/> | Returns an array of promotion objects. |
| GET /promotionTool<br>/GetPromotionById/{id} | Retrieve a specific promotion by id. | PromotionId (uint, required)<br>ServiceType (int, nullable)<br>CallerOperatorId (uint, required)<br>CallerOperatorToken (string, required) | Returns the promotion object corresponding to the provided id. |
| POST /promotionTool<br>/CreatePromotion | Create a new promotion. | CallerOperatorToken (string, required)<br>TransactionReference (string, required)<br>CallerOperatorId (uint, required)<br>Type (PromotionType, required)<br>Status (PromotionStatus, required)<br>`> to be added...` | Returns created promotion object |
| PUT /promotionTool<br>/UpdatePromotionById/{id} | Update a specific promotion by id. | PromotionId (uint, required)<br>Status (PromotionStatus, nullable)<br>DurationFrom(DateTime, nullable)<br>DurationTo(DateTime, nullable)<br>`> to be added...` | Returns the updated promotion object. |
| PUT /promotionTool<br>/CancelPromotion/{id} | Update a specific promotion's status to 'Canceled' | PromotionId (uint, required)<br>OperatorToken (string, required)<br>Status (PromotionStatus, required)<br> | Returns the updated status promotion object. |

## Interfaces & Service Model
> to be updated... need or not
