<!-- BEGIN_TF_DOCS -->
Networking skiff2

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
| [aws_instance.skiff_webserver1](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/instance) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_sg_id"></a> [sg\_id](#input\_sg\_id) | Security Groups' ID for the instances | `any` | n/a | yes |
| <a name="input_subnet_ids"></a> [subnet\_ids](#input\_subnet\_ids) | List of public subnets' ids | `any` | n/a | yes |
| <a name="input_ami_linux"></a> [ami\_linux](#input\_ami\_linux) | Specify ami for instance | `string` | `"ami-052efd3df9dad4825"` | no |
| <a name="input_file_for_user_data"></a> [file\_for\_user\_data](#input\_file\_for\_user\_data) | Specify path ot file with user data. Default: 'user\_data.sh' | `string` | `"user_data.sh"` | no |
| <a name="input_instance_type"></a> [instance\_type](#input\_instance\_type) | Specify instance type. Default: t3.nano | `string` | `"t3.nano"` | no |
| <a name="input_key_pair_name"></a> [key\_pair\_name](#input\_key\_pair\_name) | Name of the key pair | `string` | `"devops-poligon-master"` | no |
| <a name="input_number_of_servers"></a> [number\_of\_servers](#input\_number\_of\_servers) | Specify number of instances | `number` | `1` | no |
| <a name="input_server_name"></a> [server\_name](#input\_server\_name) | Name of the servers | `string` | `"skiff"` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_id_aws_instances"></a> [id\_aws\_instances](#output\_id\_aws\_instances) | n/a |
<!-- END_TF_DOCS -->