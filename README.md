# Install InSpec on Unix/Linux/Mac

## Versioning and State of Development
This project uses the [Semantic Versioning Policy](https://semver.org/). 

### Branches
The master branch contains the latest version of the guide up to a new release. 

Other branches contain feature-specific updates to the guide. 

### Tags
Tags indicate official releases of the guide.

Please note 0.x releases are works in progress (WIP) and may change at any time.   

## Option 1 Install InSpec (Package installer)
First things first: We need InSpec on our workstation. For production and standalone environments, I recommend the ChefDK package, since it gives you Chef + Test-Kitchen + InSpec. You can download the package from [https://downloads.chef.io/chefdk](https://downloads.chef.io/chefdk).

## Option 2 Install InSpec (Terminal install)
Another option is to install InSpec via a command line script:

```
$ curl https://omnitruck.chef.io/install.sh | sudo bash -s -- -channel stable -P chefdk
```

## After Install
Once InSpec is installed, run `inspec version` to verify that the installation was successful.


# Install InSpec on Windows

## Option 1 (package installer)
First things first: We need InSpec on our workstation. For production and standalone environments, I recommend the ChefDK package, since it gives you Chef + Test-Kitchen + InSpec. You can download the package from [https://downloads.chef.io/chefdk](https://downloads.chef.io/chefdk).

## Option 2 (command line)
Another option is to install InSpec via a Powershell script:

```
$ . { iwr -useb https://omnitruck.chef.io/install.ps1 } | iex; install -channel stable -project chefdk
```

## After Install
Once InSpec is installed, run `inspec version` to verify that the installation was successful.

## NOTICE

© 2018 The MITRE Corporation.

Approved for Public Release; Distribution Unlimited. Case Number 18-3678.

## NOTICE
This software was produced for the U. S. Government under Contract Number HHSM-500-2012-00008I, and is subject to Federal Acquisition Regulation Clause 52.227-14, Rights in Data-General.  

No other use other than that granted to the U. S. Government, or to those acting on behalf of the U. S. Government under that Clause is authorized without the express written permission of The MITRE Corporation. 

For further information, please contact The MITRE Corporation, Contracts Management Office, 7515 Colshire Drive, McLean, VA  22102-7539, (703) 983-6000.

