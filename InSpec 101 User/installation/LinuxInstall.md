# Install InSpec on Linux

## Install Ruby

When installing from source, gem dependencies may require ruby build tools to be installed.

For CentOS/RedHat/Fedora:  
`$ yum -y install ruby ruby-devel make gcc gcc-c++`

For Debian/Ubuntu:  
`$ apt-get -y install ruby ruby-dev gcc g++ make`

## Option 1 Install InSpec (Package installer)
First things first: We need InSpec on our workstation. There are two packages that offer an easy way to get started. For production and standalone environments, I recommend the InSpec package. Alternatively there is ChefDK, if you need Chef + Test-Kitchen + InSpec. You can download both packages from [https://downloads.chef.io/](https://downloads.chef.io/).

## Option 2 Install InSpec (Terminal install)
Another option is to install InSpec via a command line script:

```
$ curl https://omnitruck.chef.io/install.sh | sudo bash -s -- -P inspec
```

## After Install
Once InSpec is installed, run `inspec version` to verify that the installation was successful.
