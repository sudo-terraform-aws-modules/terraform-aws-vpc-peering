<!-- BEGIN_TF_DOCS -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | >= 0.14.5 |
| <a name="requirement_aws"></a> [aws](#requirement\_aws) | ~> 3.0 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | ~> 3.0 |
| <a name="provider_time"></a> [time](#provider\_time) | n/a |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [aws_vpc_peering_connection.vpc_peering](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/vpc_peering_connection) | resource |
| [aws_vpc_peering_connection_options.vpc_peering_accepter_options](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/vpc_peering_connection_options) | resource |
| [time_sleep.peer_activation](https://registry.terraform.io/providers/hashicorp/time/latest/docs/resources/sleep) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_dns_resolution"></a> [dns\_resolution](#input\_dns\_resolution) | (optional) Enable DNS resolution for remote VPC | `bool` | `false` | no |
| <a name="input_peer_account_id"></a> [peer\_account\_id](#input\_peer\_account\_id) | (optional) Speicfy the AWS account id for peering VPC | `string` | n/a | yes |
| <a name="input_peer_region"></a> [peer\_region](#input\_peer\_region) | (optional) Speicfy the region peering VPC | `string` | n/a | yes |
| <a name="input_peer_vpc_id"></a> [peer\_vpc\_id](#input\_peer\_vpc\_id) | Specify the VPC Peering ID | `string` | n/a | yes |
| <a name="input_tags"></a> [tags](#input\_tags) | (optional) map of tags to be assigned to hosted zone | `map(any)` | `{}` | no |
| <a name="input_vpc_id"></a> [vpc\_id](#input\_vpc\_id) | Specify the VPC ID | `string` | n/a | yes |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_vpc_connection_peering_id"></a> [vpc\_connection\_peering\_id](#output\_vpc\_connection\_peering\_id) | n/a |
<!-- END_TF_DOCS -->