# AWS::QuickSight::Template ResourcePermission<a name="aws-properties-quicksight-template-resourcepermission"></a>

Permission for the resource\.

## Syntax<a name="aws-properties-quicksight-template-resourcepermission-syntax"></a>

To declare this entity in your AWS CloudFormation template, use the following syntax:

### JSON<a name="aws-properties-quicksight-template-resourcepermission-syntax.json"></a>

```
{
  "[Actions](#cfn-quicksight-template-resourcepermission-actions)" : [ String, ... ],
  "[Principal](#cfn-quicksight-template-resourcepermission-principal)" : String
}
```

### YAML<a name="aws-properties-quicksight-template-resourcepermission-syntax.yaml"></a>

```
  [Actions](#cfn-quicksight-template-resourcepermission-actions): 
    - String
  [Principal](#cfn-quicksight-template-resourcepermission-principal): String
```

## Properties<a name="aws-properties-quicksight-template-resourcepermission-properties"></a>

`Actions`  <a name="cfn-quicksight-template-resourcepermission-actions"></a>
The IAMaction to grant or revoke permissions on\.  
*Required*: Yes  
*Type*: List of String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`Principal`  <a name="cfn-quicksight-template-resourcepermission-principal"></a>
The Amazon Resource Name \(ARN\) of the principal\. This can be one of the following:  
+ The ARN of an Amazon QuickSight user or group associated with a data source or dataset\. \(This is common\.\)
+ The ARN of an Amazon QuickSight user, group, or namespace associated with an analysis, dashboard, template, or theme\. \(This is common\.\)
+ The ARN of an AWS account root: This is an IAMARN rather than a Amazon QuickSightARN\. Use this option only to share resources \(templates\) across AWS accounts\. \(This is less common\.\)
*Required*: Yes  
*Type*: String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)