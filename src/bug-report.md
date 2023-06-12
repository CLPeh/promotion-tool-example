# Issue Tracking and Bug Report
<details><summary> Error message not display as expected  </summary>

> Issue ID: #1234  
> Severity: Medium  
> Priority: High  

### Description  
The error message is not come out as expected.

### Steps to Reproduce  
1. Replace the test data for GetPromotionTransaction: operatorId = "123!@#"
2. Execute debug tests on GetPromotionTransaction function.
  
### Expected Behavior
Error message "Operator not found!" will be shown.

### Actual Behavior
Error message "Common exception" was shown.

### Environment  
Branch: develop  
  
### Additional Information  
This issue is not present on desktop browsers.  
The issue started occurring after the recent deployment of version 2.1.0.    
  
### Screenshots  
<img src="./images/error-bug/Screenshot 2023-06-08 113230.png">
  
</details>
