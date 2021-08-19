# DescribeResourcePolicy<a name="API_DescribeResourcePolicy"></a>

Gets the resource policy and policy revision for a bot or bot alias\.

## Request Syntax<a name="API_DescribeResourcePolicy_RequestSyntax"></a>

```
GET /policy/resourceArn/ HTTP/1.1
```

## URI Request Parameters<a name="API_DescribeResourcePolicy_RequestParameters"></a>

The request uses the following URI parameters\.

 ** [resourceArn](#API_DescribeResourcePolicy_RequestSyntax) **   <a name="lexv2-DescribeResourcePolicy-request-resourceArn"></a>
The Amazon Resource Name \(ARN\) of the bot or bot alias that the resource policy is attached to\.  
Length Constraints: Minimum length of 1\. Maximum length of 1011\.  
Required: Yes

## Request Body<a name="API_DescribeResourcePolicy_RequestBody"></a>

The request does not have a request body\.

## Response Syntax<a name="API_DescribeResourcePolicy_ResponseSyntax"></a>

```
HTTP/1.1 200
Content-type: application/json

{
   "policy": "string",
   "resourceArn": "string",
   "revisionId": "string"
}
```

## Response Elements<a name="API_DescribeResourcePolicy_ResponseElements"></a>

If the action is successful, the service sends back an HTTP 200 response\.

The following data is returned in JSON format by the service\.

 ** [policy](#API_DescribeResourcePolicy_ResponseSyntax) **   <a name="lexv2-DescribeResourcePolicy-response-policy"></a>
The JSON structure that contains the resource policy\. For more information about the contents of a JSON policy document, see [ IAM JSON policy reference ](https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies.html)\.  
Type: String  
Length Constraints: Minimum length of 2\.

 ** [resourceArn](#API_DescribeResourcePolicy_ResponseSyntax) **   <a name="lexv2-DescribeResourcePolicy-response-resourceArn"></a>
The Amazon Resource Name \(ARN\) of the bot or bot alias that the resource policy is attached to\.  
Type: String  
Length Constraints: Minimum length of 1\. Maximum length of 1011\.

 ** [revisionId](#API_DescribeResourcePolicy_ResponseSyntax) **   <a name="lexv2-DescribeResourcePolicy-response-revisionId"></a>
The current revision of the resource policy\. Use the revision ID to make sure that you are updating the most current version of a resource policy when you add a policy statement to a resource, delete a resource, or update a resource\.  
Type: String  
Length Constraints: Minimum length of 1\. Maximum length of 5\.  
Pattern: `^[0-9]+$` 

## Errors<a name="API_DescribeResourcePolicy_Errors"></a>

For information about the errors that are common to all actions, see [Common Errors](CommonErrors.md)\.

 **InternalServerException**   
  
HTTP Status Code: 500

 **ResourceNotFoundException**   
  
HTTP Status Code: 404

 **ThrottlingException**   
  
HTTP Status Code: 429

## See Also<a name="API_DescribeResourcePolicy_SeeAlso"></a>

For more information about using this API in one of the language\-specific AWS SDKs, see the following:
+  [ AWS Command Line Interface](https://docs.aws.amazon.com/goto/aws-cli/models.lex.v2-2020-08-07/DescribeResourcePolicy) 
+  [ AWS SDK for \.NET](https://docs.aws.amazon.com/goto/DotNetSDKV3/models.lex.v2-2020-08-07/DescribeResourcePolicy) 
+  [ AWS SDK for C\+\+](https://docs.aws.amazon.com/goto/SdkForCpp/models.lex.v2-2020-08-07/DescribeResourcePolicy) 
+  [ AWS SDK for Go](https://docs.aws.amazon.com/goto/SdkForGoV1/models.lex.v2-2020-08-07/DescribeResourcePolicy) 
+  [ AWS SDK for Java V2](https://docs.aws.amazon.com/goto/SdkForJavaV2/models.lex.v2-2020-08-07/DescribeResourcePolicy) 
+  [ AWS SDK for JavaScript](https://docs.aws.amazon.com/goto/AWSJavaScriptSDK/models.lex.v2-2020-08-07/DescribeResourcePolicy) 
+  [ AWS SDK for PHP V3](https://docs.aws.amazon.com/goto/SdkForPHPV3/models.lex.v2-2020-08-07/DescribeResourcePolicy) 
+  [ AWS SDK for Python](https://docs.aws.amazon.com/goto/boto3/models.lex.v2-2020-08-07/DescribeResourcePolicy) 
+  [ AWS SDK for Ruby V3](https://docs.aws.amazon.com/goto/SdkForRubyV3/models.lex.v2-2020-08-07/DescribeResourcePolicy) 