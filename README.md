# Infraestrutura como Código Utilizando Terraform
[![image](https://user-images.githubusercontent.com/63075243/156845137-3e12ada2-85be-4b4d-87df-d2a403182473.png)](https://github.com/thiagof-araujo/terraform_EC2/blob/main/LICENSE)

# Sobre o Projeto

Foi utilizado infraestruta como código para criar duas instancias EC2 na AWS utilizando terraform. Também foram criados dois workspace de Dev e Prod.

![image](https://github.com/thiagof-araujo/Terraform_EC2/blob/main/imagem/terraform%20ec2.drawio.png)

## Tecnlogias utilizadas
- AWS S3
- AWS EC2
- AWS CLI
- Terraform
- Linux

<!-- BEGIN_TF_DOCS -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_aws"></a> [aws](#requirement\_aws) | 4.26.0 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | 4.26.0 |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [aws_instance.this](https://registry.terraform.io/providers/hashicorp/aws/4.26.0/docs/resources/instance) | resource |
| [aws_internet_gateway.this](https://registry.terraform.io/providers/hashicorp/aws/4.26.0/docs/resources/internet_gateway) | resource |
| [aws_key_pair.this](https://registry.terraform.io/providers/hashicorp/aws/4.26.0/docs/resources/key_pair) | resource |
| [aws_route.this](https://registry.terraform.io/providers/hashicorp/aws/4.26.0/docs/resources/route) | resource |
| [aws_security_group.sg-web](https://registry.terraform.io/providers/hashicorp/aws/4.26.0/docs/resources/security_group) | resource |
| [aws_subnet.this](https://registry.terraform.io/providers/hashicorp/aws/4.26.0/docs/resources/subnet) | resource |
| [aws_vpc.this](https://registry.terraform.io/providers/hashicorp/aws/4.26.0/docs/resources/vpc) | resource |
| [aws_ami.ubuntu](https://registry.terraform.io/providers/hashicorp/aws/4.26.0/docs/data-sources/ami) | data source |
| [aws_availability_zones.available](https://registry.terraform.io/providers/hashicorp/aws/4.26.0/docs/data-sources/availability_zones) | data source |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_aws_instance_type"></a> [aws\_instance\_type](#input\_aws\_instance\_type) | n/a | `string` | n/a | yes |
| <a name="input_aws_profile"></a> [aws\_profile](#input\_aws\_profile) | n/a | `string` | n/a | yes |
| <a name="input_aws_public_key"></a> [aws\_public\_key](#input\_aws\_public\_key) | value | `string` | n/a | yes |
| <a name="input_aws_region"></a> [aws\_region](#input\_aws\_region) | n/a | `string` | n/a | yes |
| <a name="input_prefix"></a> [prefix](#input\_prefix) | n/a | `string` | n/a | yes |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_ec2_public_ip"></a> [ec2\_public\_ip](#output\_ec2\_public\_ip) | n/a |
<!-- END_TF_DOCS -->
