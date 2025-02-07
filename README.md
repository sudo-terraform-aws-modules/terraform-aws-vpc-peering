# sudo-terraform-module-vpc-peering
Template repository for Terraform modules

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

## Modules

| Name | Source | Version |
|------|--------|---------|
| <a name="module_accepter"></a> [accepter](#module\_accepter) | ./modules/accepter | n/a |
| <a name="module_requester"></a> [requester](#module\_requester) | ./modules/requester | n/a |

## Resources

| Name | Type |
|------|------|
| [aws_caller_identity.account](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/caller_identity) | data source |
| [aws_region.region](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/region) | data source |
| [aws_vpc.vpc](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/vpc) | data source |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_auto_accept"></a> [auto\_accept](#input\_auto\_accept) | (optional) specify the auto accept. Default: true | `bool` | `true` | no |
| <a name="input_dns_resolution"></a> [dns\_resolution](#input\_dns\_resolution) | (optional) Enable DNS resolution for remote VPC | `bool` | `false` | no |
| <a name="input_peer_account_id"></a> [peer\_account\_id](#input\_peer\_account\_id) | (optional) Speicfy the AWS account id for peering VPC | `string` | `""` | no |
| <a name="input_peer_region"></a> [peer\_region](#input\_peer\_region) | (optional) Speicfy the region peering VPC | `string` | `""` | no |
| <a name="input_peer_vpc_id"></a> [peer\_vpc\_id](#input\_peer\_vpc\_id) | Specify the VPC Peering ID | `string` | n/a | yes |
| <a name="input_tags"></a> [tags](#input\_tags) | (optional) map of tags to be assigned to hosted zone | `map(any)` | `{}` | no |
| <a name="input_vpc_id"></a> [vpc\_id](#input\_vpc\_id) | Specify the VPC ID | `string` | n/a | yes |

## Outputs

No outputs.
<!-- END_TF_DOCS -->