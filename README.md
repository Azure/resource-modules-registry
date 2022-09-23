# Resource Modules Registry

This repository is used to store a decoupled version of [Azure/ResourceModules](https://github.com/Azure/ResourceModules) and to publish modules to a public [Bicep registry](#).

## Modules

 | Module | Version | Public Bicep Registry Url Path |
  | - | - | - | 
  |  [Storage Account](https://github.com/Azure/ResourceModules/tree/main/modules/Microsoft.Storage/storageAccounts) | <a href="https://adpsxxazacrx009.azurecr.io/v2/bicep/modules/microsoft.storage.storageaccounts/tags/list"><image src="https://img.shields.io/badge/carmr-0.4-blue"></a> | `br:carmr.azurecr.io/bicep/modules/microsoft.storage.storageaccounts:latest`
 |  [Key Vault](https://github.com/Azure/ResourceModules/tree/main/modules/Microsoft.KeyVault/vaults)  | <a href="https://adpsxxazacrx009.azurecr.io/v2/bicep/modules/microsoft.KeyVault/vaults/tags/list"><image src="https://img.shields.io/badge/carmr-0.4-blue"></a> | `br:carmr.azurecr.io/bicep/microsoft.keyvault.vaults:latest`

 ## Usage
 
```bicep
 
module sa 'br:carmr.azurecr.io:microsoft.storage.storageaccounts:latest' = {
  name: 'sa'
  params: {
    name: name
  }
}

// with alias
module kv 'br/carmr:microsoft.keyvault.vaults:latest' = {
  name: 'kv'
  params: {
    name: name
  }
}
```

## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Trademarks

This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft
trademarks or logos is subject to and must follow
[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
Any use of third-party trademarks or logos are subject to those third-party's policies.
