<!-- BEGIN_TF_DOCS -->
## Requirements

No requirements.

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | n/a |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [aws_security_group.SG_skiff](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_env"></a> [env](#input\_env) | Define stage of development: dev, test, prod | `string` | `"dev"` | no |
| <a name="input_name_project"></a> [name\_project](#input\_name\_project) | Name of project which be placed in all the resources | `string` | `"skiff"` | no |
| <a name="input_port_to_open_in_sg"></a> [port\_to\_open\_in\_sg](#input\_port\_to\_open\_in\_sg) | list of opened ports in the server | `list` | <pre>[<br>  "443",<br>  "22",<br>  "80",<br>  "81",<br>  "1488"<br>]</pre> | no |
| <a name="input_sg_explain_word"></a> [sg\_explain\_word](#input\_sg\_explain\_word) | Enter the word that explain the SG. Example for the 'public': 10.171.x.x.-public-skiff-dev | `string` | `"custom"` | no |
| <a name="input_vpc_cidr_mask16"></a> [vpc\_cidr\_mask16](#input\_vpc\_cidr\_mask16) | Enter VPC CIDR/16 first two numbers (without dot in the end): Example: '10.171' | `any` | n/a | yes |
| <a name="input_vpc_id"></a> [vpc\_id](#input\_vpc\_id) | Enter desired VPC ID | `any` | n/a | yes |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_webserver_sg_id"></a> [webserver\_sg\_id](#output\_webserver\_sg\_id) | n/a |

layer2 skiff
<!-- END_TF_DOCS -->