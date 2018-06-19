# Overview

Harden the IaaS environment created by [the PCF pipelines](https://github.com/pivotal-cf/pcf-pipelines).

# Usage

Apply the `harden-network` YAML patch to the `install-pcf` pipeline for AWS before loading the pipeline into Concourse. No
additional parameters are required.

# Hardening Applied

* Lock down security groups
* Create VPC Endpoints for S3 and EC2
* Encrypt S3 buckets

# Limitations

* Currently supports only AWS.

# Warning

*I quickly extracted this from my [bootstrap](https://github.com/crdant/bootstrap) repository and applied minimal testing.
This may bork your PCF environment.*
