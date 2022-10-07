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
| [aws_autoscaling_group.simple_autoscale](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/autoscaling_group) | resource |
| [aws_launch_configuration.simple_webserver](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/launch_configuration) | resource |
| [aws_lb.simple_elb](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb) | resource |
| [aws_lb_listener.simple_elb](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb_listener) | resource |
| [aws_lb_target_group.simple_elb](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb_target_group) | resource |
| [aws_ami.latest_ubuntu](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/ami) | data source |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_current_VPC_id"></a> [current\_VPC\_id](#input\_current\_VPC\_id) | n/a | `any` | n/a | yes |
| <a name="input_current_subnets_id"></a> [current\_subnets\_id](#input\_current\_subnets\_id) | n/a | `any` | n/a | yes |
| <a name="input_sg_ids"></a> [sg\_ids](#input\_sg\_ids) | n/a | `any` | n/a | yes |
| <a name="input_file_for_user_data"></a> [file\_for\_user\_data](#input\_file\_for\_user\_data) | Specify path ot file with user data. Default: 'user\_data.sh' | `string` | `"user_data.sh"` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_web_loadbalancer_url"></a> [web\_loadbalancer\_url](#output\_web\_loadbalancer\_url) | n/a |

Security skiff
<!-- END_TF_DOCS -->