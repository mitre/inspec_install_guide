# How to Install InSpec

## Versioning and State of Development

This project uses the [Semantic Versioning Policy](https://semver.org/).

### Branches

The master branch contains the latest version of the guide up to a new release.

Other branches contain feature-specific updates to the guide.

### Tags

Tags indicate official releases of the guide.

Please note 0.x releases are works in progress (WIP) and may change at any time.

## Instructions

First things first, we need InSpec on our workstation. For production and standalone environments, the InSpec omnibus package gives you the bare minimum of what you need. This can be manually installed from a downloaded package or installed using a handy installer script provided by Chef.

### Option 1: Manual installation

This option is best when working in an air-gapped environment. Downloading the latest package files for InSpec from [Chef's downloads page](https://downloads.chef.io/inspec) will allow you to transfer the installers where you need them to go, then, depending on the operating system, install them in the platform-appropriate manner.

### Option 2: Automated installation

Another option is to install InSpec via a command line script, provided and maintained by Chef. This will only work if your firewall does not restrict WAN access to the following domains:

- `omnitruck.chef.io`
- `packages.chef.io`

Unix/Linux/Mac:

```
$ curl https://omnitruck.chef.io/install.sh | sudo bash -s -- -c stable -P inspec -v 3
```

Windows:

```
$ . { iwr -useb https://omnitruck.chef.io/install.ps1 } | iex; install -channel stable -project inspec -version 3
```

### After Install

Once InSpec is installed, run `inspec version` to verify that the installation was successful.

## NOTICE

© 2018 The MITRE Corporation.

Approved for Public Release; Distribution Unlimited. Case Number 18-3678.

This software was produced for the U. S. Government under Contract Number HHSM-500-2012-00008I, and is subject to Federal Acquisition Regulation Clause 52.227-14, Rights in Data-General.

No other use other than that granted to the U. S. Government, or to those acting on behalf of the U. S. Government under that Clause is authorized without the express written permission of The MITRE Corporation.

For further information, please contact The MITRE Corporation, Contracts Management Office, 7515 Colshire Drive, McLean, VA  22102-7539, (703) 983-6000.
