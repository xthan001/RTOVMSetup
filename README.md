# RTOVMSetup
This is a fork of Zeropoint Security and the original work is from them. I modified a few aspects to work for my settings. Refer to https://github.com/ZeroPointSecurity/RTOVMSetup
## Windows

### 1. Install Boxstarter
```
. { Invoke-WebRequest -useb https://boxstarter.org/bootstrapper.ps1 } | iex; Get-Boxstarter -Force
```

### 2. Install Boxstarter Package
```
$Cred = Get-Credential $env:USERNAME
Install-BoxstarterPackage -PackageName https://raw.githubusercontent.com/xthan001/RTOVMSetup/master/setup -Credential $Cred
```

## Kali
```
kali@kali:~$ curl -sS https://raw.githubusercontent.com/xthan001/RTOVMSetup/master/kali.sh | sudo bash -
```
