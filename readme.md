<!-- BEGIN_TF_DOCS -->
## Requirements

No requirements.

## Providers

No providers.

## Modules

| Name | Source | Version |
|------|--------|---------|
| <a name="module_create_SG_for_DB"></a> [create\_SG\_for\_DB](#module\_create\_SG\_for\_DB) | ./layer2.SG | n/a |
| <a name="module_create_SG_private"></a> [create\_SG\_private](#module\_create\_SG\_private) | ./layer2.SG | n/a |
| <a name="module_create_SG_public"></a> [create\_SG\_public](#module\_create\_SG\_public) | ./layer2.SG | n/a |
| <a name="module_create_simple_public_instance"></a> [create\_simple\_public\_instance](#module\_create\_simple\_public\_instance) | ./layer3.Servers | n/a |
| <a name="module_create_skiff_VPC_and_subnets"></a> [create\_skiff\_VPC\_and\_subnets](#module\_create\_skiff\_VPC\_and\_subnets) | ./layer1.Network | n/a |

## Resources

No resources.

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_name_project"></a> [name\_project](#input\_name\_project) | Name of project which be placed in all the resources | `string` | `"skiff3"` | no |
| <a name="input_temp_vpc_cidr_mask16"></a> [temp\_vpc\_cidr\_mask16](#input\_temp\_vpc\_cidr\_mask16) | First two numbers of the VPC (without dot in the end). Example: '10.178' | `string` | `"10.171"` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_id_servers"></a> [id\_servers](#output\_id\_servers) | n/a |
| <a name="output_output_public_subnet_ids"></a> [output\_public\_subnet\_ids](#output\_output\_public\_subnet\_ids) | n/a |

main skiff
<!-- END_TF_DOCS -->