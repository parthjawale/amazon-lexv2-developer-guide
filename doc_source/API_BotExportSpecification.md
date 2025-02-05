# BotExportSpecification<a name="API_BotExportSpecification"></a>

Provides the identity of a the bot that was exported\.

## Contents<a name="API_BotExportSpecification_Contents"></a>

 **botId**   <a name="lexv2-Type-BotExportSpecification-botId"></a>
The identifier of the bot assigned by Amazon Lex\.  
Type: String  
Length Constraints: Fixed length of 10\.  
Pattern: `^[0-9a-zA-Z]+$`   
Required: Yes

 **botVersion**   <a name="lexv2-Type-BotExportSpecification-botVersion"></a>
The version of the bot that was exported\. This will be either `DRAFT` or the version number\.  
Type: String  
Length Constraints: Minimum length of 1\. Maximum length of 5\.  
Pattern: `^(DRAFT|[0-9]+)$`   
Required: Yes

## See Also<a name="API_BotExportSpecification_SeeAlso"></a>

For more information about using this API in one of the language\-specific AWS SDKs, see the following:
+  [ AWS SDK for C\+\+](https://docs.aws.amazon.com/goto/SdkForCpp/models.lex.v2-2020-08-07/BotExportSpecification) 
+  [ AWS SDK for Go](https://docs.aws.amazon.com/goto/SdkForGoV1/models.lex.v2-2020-08-07/BotExportSpecification) 
+  [ AWS SDK for Java V2](https://docs.aws.amazon.com/goto/SdkForJavaV2/models.lex.v2-2020-08-07/BotExportSpecification) 
+  [ AWS SDK for Ruby V3](https://docs.aws.amazon.com/goto/SdkForRubyV3/models.lex.v2-2020-08-07/BotExportSpecification) 