<!-- BEGIN_TF_DOCS -->
bootstrap skiff

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
| [aws_eip.nat](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/eip) | resource |
| [aws_internet_gateway.main_gateway](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/internet_gateway) | resource |
| [aws_nat_gateway.ng](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/nat_gateway) | resource |
| [aws_route_table.internal_subnets](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table) | resource |
| [aws_route_table.public_subnets](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table) | resource |
| [aws_route_table_association.internal_routes_skiff](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_route_table_association.public_routes_skiff](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association) | resource |
| [aws_subnet.DB_subnets](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_subnet.internal_subnets](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_subnet.public_subnets](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/subnet) | resource |
| [aws_vpc.skiff_vpc](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/vpc) | resource |
| [aws_availability_zones.available_zones](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/availability_zones) | data source |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_count_subnets"></a> [count\_subnets](#input\_count\_subnets) | number of public subnets with mask /24 to create | `number` | `4` | no |
| <a name="input_count_subnets_db"></a> [count\_subnets\_db](#input\_count\_subnets\_db) | number of DB-subnets with mask /24 to create | `number` | `0` | no |
| <a name="input_count_subnets_internal"></a> [count\_subnets\_internal](#input\_count\_subnets\_internal) | number of internal subnets with mask /24 to create | `number` | `0` | no |
| <a name="input_env"></a> [env](#input\_env) | Define stage of development: dev, test, prod | `string` | `"dev"` | no |
| <a name="input_name_of_VPC"></a> [name\_of\_VPC](#input\_name\_of\_VPC) | name of VPC to find | `string` | `"10.0.x.x-main"` | no |
| <a name="input_name_of_instance_type"></a> [name\_of\_instance\_type](#input\_name\_of\_instance\_type) | Instance Type | `string` | `"t3.nano"` | no |
| <a name="input_name_project"></a> [name\_project](#input\_name\_project) | Name of project which be placed in all the resources | `string` | `"skiff"` | no |
| <a name="input_tag_of_subnets_to_find"></a> [tag\_of\_subnets\_to\_find](#input\_tag\_of\_subnets\_to\_find) | subnets with specified tag | `string` | `"*external*"` | no |
| <a name="input_vpc_cidr_mask16"></a> [vpc\_cidr\_mask16](#input\_vpc\_cidr\_mask16) | First two numbers of the VPC (without dot in the end) | `string` | `"10.173"` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_DB_subnet_ids"></a> [DB\_subnet\_ids](#output\_DB\_subnet\_ids) | n/a |
| <a name="output_internal_subnet_ids"></a> [internal\_subnet\_ids](#output\_internal\_subnet\_ids) | n/a |
| <a name="output_public_subnet_ids"></a> [public\_subnet\_ids](#output\_public\_subnet\_ids) | n/a |
| <a name="output_vpc_cidr"></a> [vpc\_cidr](#output\_vpc\_cidr) | n/a |
| <a name="output_vpc_cidr_mask16"></a> [vpc\_cidr\_mask16](#output\_vpc\_cidr\_mask16) | n/a |
| <a name="output_vpc_id"></a> [vpc\_id](#output\_vpc\_id) | OUTPUT outputs needs for communication with others developers |
<!-- END_TF_DOCS -->