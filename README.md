# <img src="https://github.com/pip-services/pip-services/raw/master/design/Logo.png" alt="Pip.Services Logo" style="max-width:30%"> <br/> Workspace for Content Management Pip.Services

This is a workspace for [Content Management Pip.Services](https://github.com/pip-services-content) 
implemented in 5 different languages: .NET, Java, Node.js, Go and Python.

The workspace enables build, test, and release across the following projects:

- **pip-services-devenv** - dockerized infrastructure services for development and testing
- **pip-services-quotes-node** - Inspirational quotes microservice in Node.js
- **pip-clients-quotes-node** - Client to Inspirational quotes microservice in Node.js
- **pip-clients-quotes-dotnet** - Client to Inspirational quotes microservice in .NET
- **pip-clients-quotes-java** - Client to Inspirational quotes microservice in Java
- **pip-clients-quotes-go** - Client to Inspirational quotes microservice in Go
- **pip-services-tags-node** - Search tags microservice in Node.js
- **pip-clients-tags-node** - Client to Search tags microservice in Node.js
- **pip-services-emailtemplates-node** - Email templates microservice in Node.js
- **pip-clients-emailtemplates-node** - Client to Email templates microservice in Node.js
- **pip-services-files-node** - Files microservice in Node.js
- **pip-clients-files-node** - Client to Files microservice in Node.js
- **pip-services-attachments-node** - File attachments microservice in Node.js
- **pip-clients-attachments-node** - Client to File attachments microservice in Node.js
- **pip-services-tips-node** - User tips microservice in Node.js
- **pip-clients-tips-node** - Client to User tips microservice in Node.js
- **pip-services-guides-node** - Application guides microservice in Node.js
- **pip-clients-guides-node** - Client to Application guides microservice in Node.js
- **pip-services-imagesets-node** - Image library microservice in Node.js
- **pip-clients-imagesets-node** - Client to Image library microservice in Node.js
- **pip-facade-content-node** - Facade operations for content microservices in Node.js

## Installation

- Install **pip-tasks-ps**, **pip-tasks-common-ps** and **pip-tasks-node-ps** Powershell modules, 
add them to **PSModulePath** and import into Powershell

- Clone this workspace to local disk
```bash
> git clone https://github.com/pip-services-content/pip-services-content-ws.git
```

- Got to the workspace folder and clone component repositories
```bash
> piptask clone -workspace
```

## Usage

- Setting default workspace
```bash
> pipuse <Path to this workspace>
```

- Start and stop infrastructure services
```bash
> piptask start -component pip-services-devenv
> piptask stop -component pip-services-devenv
```

- Building all components
```bash
> piptask build -all
```

- Test all components
``` bash
> piptask test -all
```

- Check out changes from remote repository
```bash
> piptask pull -all
```

- Check in changes to remote repository
```bash
> piptask push -m <Changes comment> -all
```

## Acknowledgements

The Infrastructure Pip.Services are created and maintained by **Sergey Seroukhov**
