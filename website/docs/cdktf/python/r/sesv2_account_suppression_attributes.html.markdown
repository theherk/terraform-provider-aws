---
subcategory: "SESv2 (Simple Email V2)"
layout: "aws"
page_title: "AWS: aws_sesv2_account_suppression_attributes"
description: |-
  Manages AWS SESv2 (Simple Email V2) account-level suppression attributes.
---


<!-- Please do not edit this file, it is generated. -->
# Resource: aws_sesv2_account_suppression_attributes

Manages AWS SESv2 (Simple Email V2) account-level suppression attributes.

## Example Usage

```python
# DO NOT EDIT. Code generated by 'cdktf convert' - Please report bugs at https://cdk.tf/bug
from constructs import Construct
from cdktf import TerraformStack
#
# Provider bindings are generated by running `cdktf get`.
# See https://cdk.tf/provider-generation for more details.
#
from imports.aws.sesv2_account_suppression_attributes import Sesv2AccountSuppressionAttributes
class MyConvertedCode(TerraformStack):
    def __init__(self, scope, name):
        super().__init__(scope, name)
        Sesv2AccountSuppressionAttributes(self, "example",
            suppressed_reasons=["COMPLAINT"]
        )
```

## Argument Reference

The following arguments are required:

* `suppressed_reasons` - (Required) A list that contains the reasons that email addresses will be automatically added to the suppression list for your account. Valid values: `COMPLAINT`, `BOUNCE`.

## Attribute Reference

This resource exports no additional attributes.

## Import

In Terraform v1.5.0 and later, use an [`import` block](https://developer.hashicorp.com/terraform/language/import) to import account-level suppression attributes using the account ID. For example:

```python
# DO NOT EDIT. Code generated by 'cdktf convert' - Please report bugs at https://cdk.tf/bug
from constructs import Construct
from cdktf import TerraformStack
#
# Provider bindings are generated by running `cdktf get`.
# See https://cdk.tf/provider-generation for more details.
#
from imports.aws.sesv2_account_suppression_attributes import Sesv2AccountSuppressionAttributes
class MyConvertedCode(TerraformStack):
    def __init__(self, scope, name):
        super().__init__(scope, name)
        Sesv2AccountSuppressionAttributes.generate_config_for_import(self, "example", "123456789012")
```

Using `terraform import`, import account-level suppression attributes using the account ID. For example:

```console
% terraform import aws_sesv2_account_suppression_attributes.example 123456789012
```

<!-- cache-key: cdktf-0.20.8 input-e4fe45ccad6391ce28893fb1f786a670740820da345f9e02df98116ee33cd05d -->