# Azure AKS
[![Changelog](https://img.shields.io/badge/changelog-release-green.svg)](CHANGELOG.md) [![Notice](https://img.shields.io/badge/notice-copyright-yellow.svg)](NOTICE) [![Apache V2 License](https://img.shields.io/badge/license-Apache%20V2-orange.svg)](LICENSE) [![TF Registry](https://img.shields.io/badge/terraform-registry-blue.svg)](https://registry.terraform.io/modules/claranet/aks/azurerm/)

This terraform module create an [Azure AKS](https://azure.microsoft.com/fr-fr/services/kubernetes-service/) and associated [Azure Application Gateway](https://azure.microsoft.com/fr-fr/services/application-gateway/) as ingress controller.

Inside the cluster, velero, kured and cert-manager are also installed.


## Requirements and limitations

  * [Azurerm Terraform provider](https://www.terraform.io/docs/providers/azurerm/) >= 1.42
  * [Helm terraform provider](https://registry.terraform.io/providers/hashicorp/helm/1.0.0) >= 1.0.0
  * [Kubectl command](https://kubernetes.io/docs/tasks/tools/install-kubectl/)
  * A Microsoft.Storage [service endpoint](https://docs.microsoft.com/en-us/azure/virtual-network/virtual-network-service-endpoints-overview) into the nodes subnet
  
## Terraform version compatibility

| Module version | Terraform version |
| -------------- | ----------------- |
| >= 2.x.x       | 0.12.x            |
| < 2.x.x        | 0.11.x            |

## Usage

This module is optimized to work with the [Claranet terraform-wrapper](https://github.com/claranet/terraform-wrapper) too which set some terraform variables in the environment needed by this module.
More details about variables set by the `terraform wrapper` available in the [documentation](https://github.com/claranet/terraform-wrapper#environment).

You can use this module by including it this way:

```hcl

TODO
```

## Inputs

## Outputs

## Related documentation

- Kured documentation: [github.com/weaveworks/kured](https://github.com/weaveworks/kured)

