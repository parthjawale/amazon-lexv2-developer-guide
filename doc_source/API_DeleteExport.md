# DeleteExport<a name="API_DeleteExport"></a>

Removes a previous export and the associated files stored in an S3 bucket\.

## Request Syntax<a name="API_DeleteExport_RequestSyntax"></a>

```
DELETE /exports/exportId/ HTTP/1.1
```

## URI Request Parameters<a name="API_DeleteExport_RequestParameters"></a>

The request uses the following URI parameters\.

 ** [exportId](#API_DeleteExport_RequestSyntax) **   <a name="lexv2-DeleteExport-request-exportId"></a>
The unique identifier of the export to delete\.  
Length Constraints: Fixed length of 10\.  
Pattern: `^[0-9a-zA-Z]+$`   
Required: Yes

## Request Body<a name="API_DeleteExport_RequestBody"></a>

The request does not have a request body\.

## Response Syntax<a name="API_DeleteExport_ResponseSyntax"></a>

```
HTTP/1.1 202
Content-type: application/json

{
   "exportId": "string",
   "exportStatus": "string"
}
```

## Response Elements<a name="API_DeleteExport_ResponseElements"></a>

If the action is successful, the service sends back an HTTP 202 response\.

The following data is returned in JSON format by the service\.

 ** [exportId](#API_DeleteExport_ResponseSyntax) **   <a name="lexv2-DeleteExport-response-exportId"></a>
The unique identifier of the deleted export\.  
Type: String  
Length Constraints: Fixed length of 10\.  
Pattern: `^[0-9a-zA-Z]+$` 

 ** [exportStatus](#API_DeleteExport_ResponseSyntax) **   <a name="lexv2-DeleteExport-response-exportStatus"></a>
The current status of the deletion\. When the deletion is complete, the export will no longer be returned by the [ListExports](API_ListExports.md) operation and calls to the [DescribeExport](API_DescribeExport.md) with the export identifier will fail\.  
Type: String  
Valid Values:` InProgress | Completed | Failed | Deleting` 

## Errors<a name="API_DeleteExport_Errors"></a>

For information about the errors that are common to all actions, see [Common Errors](CommonErrors.md)\.

 **InternalServerException**   
  
HTTP Status Code: 500

 **PreconditionFailedException**   
  
HTTP Status Code: 412

 **ServiceQuotaExceededException**   
  
HTTP Status Code: 402

 **ThrottlingException**   
  
HTTP Status Code: 429

 **ValidationException**   
  
HTTP Status Code: 400

## See Also<a name="API_DeleteExport_SeeAlso"></a>

For more information about using this API in one of the language\-specific AWS SDKs, see the following:
+  [ AWS Command Line Interface](https://docs.aws.amazon.com/goto/aws-cli/models.lex.v2-2020-08-07/DeleteExport) 
+  [ AWS SDK for \.NET](https://docs.aws.amazon.com/goto/DotNetSDKV3/models.lex.v2-2020-08-07/DeleteExport) 
+  [ AWS SDK for C\+\+](https://docs.aws.amazon.com/goto/SdkForCpp/models.lex.v2-2020-08-07/DeleteExport) 
+  [ AWS SDK for Go](https://docs.aws.amazon.com/goto/SdkForGoV1/models.lex.v2-2020-08-07/DeleteExport) 
+  [ AWS SDK for Java V2](https://docs.aws.amazon.com/goto/SdkForJavaV2/models.lex.v2-2020-08-07/DeleteExport) 
+  [ AWS SDK for JavaScript](https://docs.aws.amazon.com/goto/AWSJavaScriptSDK/models.lex.v2-2020-08-07/DeleteExport) 
+  [ AWS SDK for PHP V3](https://docs.aws.amazon.com/goto/SdkForPHPV3/models.lex.v2-2020-08-07/DeleteExport) 
+  [ AWS SDK for Python](https://docs.aws.amazon.com/goto/boto3/models.lex.v2-2020-08-07/DeleteExport) 
+  [ AWS SDK for Ruby V3](https://docs.aws.amazon.com/goto/SdkForRubyV3/models.lex.v2-2020-08-07/DeleteExport) 