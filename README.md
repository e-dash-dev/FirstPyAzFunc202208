# FirstPyAzFunc202208
Azure Function dev sample by python


## How to start Azure Function development on GitHub Codespaces

### 1. Create repository

with README file

### 2. Create Codespaces from repository

### 3. Access to Codespaces

Check environments from terminal:

```terminal
$ cat /etc/issue
Ubuntu 20.04.4 LTS
 
$ python --version 
Python 3.10.4
```

### 4. Check Azure Function Tools

#### Installed in default environment

- Azure Tools (at least "Azure Functions" tool required )
- Azure CLI Tools (preferred)

#### Manual install required (from terminal)

[Azure Functions Core Tools](https://github.com/Azure/azure-functions-core-tools#linux)

Need for local (out-of-azure) debugging (just skip if not needed)

- Setup package

```
wget -q https://packages.microsoft.com/config/ubuntu/20.04/packages-microsoft-prod.deb
sudo dpkg -i packages-microsoft-prod.deb
```

- Install

```
sudo apt-get update
sudo apt-get install azure-functions-core-tools-4
```

### 5. Create new function app

Create from **Azure** tool bar in Visual Studio code

if error occurs when create from gap of local(3.10) and Azure Function SDK (3.8), install as guided in output message (need 'sudo'):

```
sudo apt-get install python3.8-venv
```

### 6. Run and Debug function app

From **Run and debug** tool bar in Visual Studio Code (attach to **function app**)

Check localhost:7071 (or other port) tunnel to public address from port menu

http://localhost:7071/ -> https://YOUR-NAME_YOUR-REPONAME_VMNAME-7071.githubpreview.dev/
