# Install InSpec on Unix/Linux/Mac

## Option 1 Install InSpec (Package installer)
First things first: We need InSpec on our workstation. For production and standalone environments, I recommend the ChefDK package, since it gives you Chef + Test-Kitchen + InSpec. You can download the package from [https://downloads.chef.io/](https://downloads.chef.io/).

## Option 2 Install InSpec (Terminal install)
Another option is to install InSpec via a command line script:

```
$ curl https://omnitruck.chef.io/install.sh | sudo bash -s -- -channel stable -P chefdk
```

## After Install
Once InSpec is installed, run `inspec version` to verify that the installation was successful.


# Install InSpec on Windows

## Option 1 (package installer)
First things first: We need InSpec on our workstation. For production and standalone environments, I recommend the ChefDK package, since it gives you Chef + Test-Kitchen + InSpec. You can download the package from [https://downloads.chef.io/](https://downloads.chef.io/).

## Option 2 (command line)
Another option is to install InSpec via a Powershell script:

```
$ . { iwr -useb https://omnitruck.chef.io/install.ps1 } | iex; install -channel stable -project chefdk
```

## After Install
Once InSpec is installed, run `inspec version` to verify that the installation was successful.
