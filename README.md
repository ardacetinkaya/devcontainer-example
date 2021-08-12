# devcontainer.json Example

This is simple example for _**devcontainer.json**_ for development configuration for [GitHub Codespaces](https://github.com/features/codespaces). 
Within this container configuration;

- Azure CLI
- Terraform
- Node
- .NET 5

are kind of components(which are my daily routines nowadays) that can be included in the container configuration for development.

```json
		"args": { 
			// Update 'VARIANT' to pick a .NET Core version: 2.1, 3.1, 5.0
			"VARIANT": "5.0",
			"INSTALL_NODE": "true",
			"NODE_VERSION": "lts/*",
			"INSTALL_AZURE_CLI": "true",
			"INSTALL_TERRAFORM": "true",
			"TERRAFORM_FILE":"terraform_1.0.4_linux_amd64.zip",
			"TERRAFORM_VERSION":"https://releases.hashicorp.com/terraform/1.0.4/terraform_1.0.4_linux_amd64.zip"
		}
```

Also some extensions can be set for the development container for VS Code
```
	"extensions": [
		"ms-dotnettools.csharp",
		"hashicorp.terraform",
		"ms-vscode.azure-account",
		"ms-azuretools.vscode-azurefunctions",
		"ms-azuretools.vscode-azureresourcegroups",
		"github.copilot",
		"ms-mssql.mssql",
		"hookyqr.beautify",
		"ms-azuretools.vscode-docker"
	]
```

### References:
- https://code.visualstudio.com/docs/remote/devcontainerjson-reference
- https://github.com/microsoft/vscode-dev-containers
