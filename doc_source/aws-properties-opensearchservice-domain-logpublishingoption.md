# AWS::OpenSearchService::Domain LogPublishingOption<a name="aws-properties-opensearchservice-domain-logpublishingoption"></a>

Specifies whether the OpenSearch Service domain publishes the OpenSearch application, search slow logs, or index slow logs to Amazon CloudWatch\. Each option must be an object of name `SEARCH_SLOW_LOGS`, `APPLICATION_LOGS`, `INDEX_SLOW_LOGS`, or `AUDIT_LOGS` depending on the type of logs you want to publish\. For the full syntax, see the [examples](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-opensearchservice-domain.html#aws-resource-opensearchservice-domain--examples)\.

If you enable a slow log, you still have to enable the *collection* of slow logs using the OpenSearch REST API\. To learn more, see [Enabling log publishing \(AWS CLI\)](https://docs.aws.amazon.com/opensearch-service/latest/developerguide/createdomain-configure-slow-logs.html#createdomain-configure-slow-logs-cli)\.

## Syntax<a name="aws-properties-opensearchservice-domain-logpublishingoption-syntax"></a>

To declare this entity in your AWS CloudFormation template, use the following syntax:

### JSON<a name="aws-properties-opensearchservice-domain-logpublishingoption-syntax.json"></a>

```
{
  "[CloudWatchLogsLogGroupArn](#cfn-opensearchservice-domain-logpublishingoption-cloudwatchlogsloggrouparn)" : String,
  "[Enabled](#cfn-opensearchservice-domain-logpublishingoption-enabled)" : Boolean
}
```

### YAML<a name="aws-properties-opensearchservice-domain-logpublishingoption-syntax.yaml"></a>

```
  [CloudWatchLogsLogGroupArn](#cfn-opensearchservice-domain-logpublishingoption-cloudwatchlogsloggrouparn): String
  [Enabled](#cfn-opensearchservice-domain-logpublishingoption-enabled): Boolean
```

## Properties<a name="aws-properties-opensearchservice-domain-logpublishingoption-properties"></a>

`CloudWatchLogsLogGroupArn`  <a name="cfn-opensearchservice-domain-logpublishingoption-cloudwatchlogsloggrouparn"></a>
Specifies the CloudWatch log group to publish to\.  
*Required*: No  
*Type*: String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`Enabled`  <a name="cfn-opensearchservice-domain-logpublishingoption-enabled"></a>
If `true`, enables the publishing of logs to CloudWatch\.  
Default: `false`\.  
*Required*: No  
*Type*: Boolean  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

## See also<a name="aws-properties-opensearchservice-domain-logpublishingoption--seealso"></a>
+ [Monitoring OpenSearch logs with Amazon CloudWatch Logs](https://docs.aws.amazon.com/opensearch-service/latest/developerguide/createdomain-configure-slow-logs.html) and [LogPublishingOptions](https://docs.aws.amazon.com/opensearch-service/latest/developerguide/configuration-api.html#configuration-api-datatypes-logpublishingoptions) in the *Amazon OpenSearch Service Developer Guide*\.

