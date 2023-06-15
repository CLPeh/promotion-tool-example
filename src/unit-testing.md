# Unit Testing

Do the unit testing based on [AAA Testing Structure](https://www.c-sharpcorner.com/UploadFile/dacca2/fundamental-of-unit-testing-understand-aaa-in-unit-testing/)
- Arrange: initialize data (map value into request, do the necessary setup of the test)
- Act: execute function (do the actual unit testing and the result will be obtained from the test application)
- Assert: check and verify the returned result with expected results

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
