# AWS Organizations Automation Demo

## License

All files in this repository is covered by the [Apache 2.0 license](LICENSE.txt)

## Reference

Original source from AWS blog post [here](https://aws.amazon.com/blogs/security/how-to-use-aws-organizations-to-automate-end-to-end-account-creation/)

## Changes from original source

* remove license boilerplate from CloudFormation templates (you can't have comments in JSON)
* line 90 of `organization-new-acc.sh`: changed the source_profile from `default` to `slalom-test` (my default profile is a different AWS account)

## Run

```
./organization-new-acc.sh --account_name "<account_name>" --account_email "<email_address>" --cl_profile_name "<profile_name>" --ou_name "<dest_ou_name>"
```

* `account_name`: name of new member account
* `account_email`: primary email of new member account
* `profile_name`: name of new AWS CLI profile this script will create
* `dest_ou_name`: name of OU to move the new member account into; this is optional - account will still get created if this isn't specified

