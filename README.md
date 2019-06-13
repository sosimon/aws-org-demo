# AWS Organizations Automation Demo

## License

All files in this repository is covered by the [Apache 2.0 license](LICENSE.txt)

## Reference

Original source from AWS blog post [here](https://aws.amazon.com/blogs/security/how-to-use-aws-organizations-to-automate-end-to-end-account-creation/)

## Changes from original source

* remove license boilerplate from CloudFormation templates (you can't have comments in JSON)
* line 90 of `organization-new-acc.sh`: changed the source_profile from `default` to `slalom-test` (my default profile is a different AWS account)