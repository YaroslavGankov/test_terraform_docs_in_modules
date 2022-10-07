<!-- BEGIN_TF_DOCS -->
shared skiff
some changes in notes.md file

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
| [aws_lb.simple_elb](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb) | resource |
| [aws_lb_listener.simple_elb](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb_listener) | resource |
| [aws_lb_target_group.simple_elb](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb_target_group) | resource |
| [aws_lb_target_group_attachment.attach_instances](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb_target_group_attachment) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_current_VPC_id"></a> [current\_VPC\_id](#input\_current\_VPC\_id) | n/a | `any` | n/a | yes |
| <a name="input_current_subnets_id"></a> [current\_subnets\_id](#input\_current\_subnets\_id) | n/a | `any` | n/a | yes |
| <a name="input_id_aws_instances"></a> [id\_aws\_instances](#input\_id\_aws\_instances) | n/a | `any` | n/a | yes |
| <a name="input_sg_ids"></a> [sg\_ids](#input\_sg\_ids) | n/a | `any` | n/a | yes |
| <a name="input_name_project"></a> [name\_project](#input\_name\_project) | Name of project which be placed in all the resources | `string` | `"skiff"` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_web_loadbalancer_url"></a> [web\_loadbalancer\_url](#output\_web\_loadbalancer\_url) | n/a |
<!-- END_TF_DOCS -->