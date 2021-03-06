# Red Hat OpenShift Service on AWS (ROSA) Command Line Tool

This project contains the `rosa` command line tool that simplifies the use of Red Hat OpenShift Service on AWS, also known as _ROSA_.

## Quickstart guide

Refer to the official ROSA documentation: https://access.redhat.com/products/red-hat-openshift-service-aws

1. Follow the [AWS Command Line Interface](https://aws.amazon.com/cli/) documentation to install and configure the AWS CLI for your operating system.
2. Download the [latest release of rosa](https://github.com/openshift/rosa/releases/latest) and add it to your path.
3. Initialize your AWS account by running `rosa init` and following the instructions.
4. Create your first ROSA cluster by running `rosa create cluster --interactive`

## Build from source

If you'd like to build this project from source use the following steps:

1. Checkout the repostiory into your `$GOPATH`

```
go get -u github.com/openshift/rosa
```

2. `cd` to the checkout out source directory

```
cd $GOPATH/src/github.com/openshift/rosa
```

3. Install the binary (This will install to `$GOPATH/bin`)

```
make install
```

NOTE: If you don't have `$GOPATH/bin` in your `$PATH` you need to add it or move `rosa` to a standard system directory eg. for Linux/OSX:

```
sudo mv $GOPATH/bin/rosa /usr/local/bin
```

## Have you got feedback?

We want to hear it. [Open an issue](https://github.com/openshift/rosa/issues/new) against the repo and someone from the team will be in touch.
