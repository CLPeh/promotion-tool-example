# Unit Testing

Do the unit testing based on AAA Testing Structure
- Arrange: initialize data (map value into request)
- Act: execute function (run method)
- Assert: compare result with expectation

## Test Case
**CreatePromotion**  
- Create new promotion
  - Recreate the promotion if inactive
- NonGlobalCallerOnly
- NonGlobalInvalidCallerOToken
- IsGlobalWith2SubOperators
- IsGlobal2InvalidSubOperators
- IsGlobal2SubOperatorsNotChildofCaller
- IsGlobalSubOperatorNotChildofCaller
- InvalidDate
- InvalidPeriod
  - nonGlobal -> only create for promotion for caller operator
  - isGlobal -> create for valid subOperators (if subOperators count > 1)  
<br>  

**UpdatePromotion**
- Update promotion name  
<br>  

**CancelPromotion**
- Cancel existing promotion  
<br>  

**GetPromotionById**
<br>  

**GetPromoTransaction**
- ExternalNoToken
- ExternalInvalidToken
- BOValidToken
- BOInvalidToken
- GPValidToken
- GPInvalidToken
- ServiceType: 
  - External
  - BO - BackOffice
  - GP - GameProxy
<br>  

**GetPromoTransactionSummary**
- ExternalNoTokenOpId
- ExternalInvalidToken
- BONoTokenOpId
- BOValidToken
- BOInvalidToken
