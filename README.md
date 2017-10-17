AWS S3 Logs Terraform module
====================================

Terraform module wich creates a S3 bucket suitable to be used as a ALB logs storage

Usage
-----

```hcl
module "s3_logs" {
  source                  = "git::https://github.com/egarbi/terraform-aws-s3-logs"
  name                    = "example"
  environment             = "testing"
  account_id              = "12345678901"
  logs_expiration_enabled = "true"
  logs_expiration_days    = "30"
}
```

> Note: All the credit here is for segment guys.
>
> They built this module https://github.com/segmentio/stack/blob/master/s3-logs/main.tf
