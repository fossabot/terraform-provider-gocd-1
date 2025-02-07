[![codecov](https://codecov.io/gh/cloudandthings/terraform-provider-gocd/branch/develop/graph/badge.svg)](https://codecov.io/gh/cloudandthings/terraform-provider-gocd)
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fcloudandthings%2Fterraform-provider-gocd.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fcloudandthings%2Fterraform-provider-gocd?ref=badge_shield)

# Terraform Provider GoCD

This repository is a *template* for a [Terraform](https://www.terraform.io) provider. It is intended as a starting point for creating Terraform providers, containing:

 - A resource, and a data source (`internal/provider/`),
 - Examples (`examples/`) and generated documentation (`docs/`),
 - Miscellaneous meta files.
 
These files contain boilerplate code that you will need to edit to create your own Terraform provider. A full guide to creating Terraform providers can be found at [Writing Custom Providers](https://www.terraform.io/docs/extend/writing-custom-providers.html).

Please see the [GitHub template repository documentation](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/creating-a-repository-from-a-template) for how to create a new repository from this template on GitHub.

Once you've written your provider, you'll want to [publish it on the Terraform Registry](https://www.terraform.io/docs/registry/providers/publishing.html) so that others can use it.


## Requirements

-	[Terraform](https://www.terraform.io/downloads.html) >= 0.13.x
-	[Go](https://golang.org/doc/install) >= 1.15

## Building The Provider

1. Clone the repository
1. Enter the repository directory
1. Build the provider using the Go `install` command: 
```sh
$ go install
```

## Adding Dependencies

This provider uses [Go modules](https://github.com/golang/go/wiki/Modules).
Please see the Go documentation for the most up to date information about using Go modules.

To add a new dependency `github.com/author/dependency` to your Terraform provider:

```
go get github.com/author/dependency
go mod tidy
```

Then commit the changes to `go.mod` and `go.sum`.

## Using the provider

Fill this in for each provider

## Developing the Provider

If you wish to work on the provider, you'll first need [Go](http://www.golang.org) installed on your machine (see [Requirements](#requirements) above).

To compile the provider, run `go install`. This will build the provider and put the provider binary in the `$GOPATH/bin` directory.

To generate or update documentation, run `go generate`.

In order to run the full suite of Acceptance tests, run `make testacc`.

*Note:* Acceptance tests create real resources, and often cost money to run.

```sh
$ make testacc
```


## License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fcloudandthings%2Fterraform-provider-gocd.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fcloudandthings%2Fterraform-provider-gocd?ref=badge_large)