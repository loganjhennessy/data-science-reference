# Use cases for AWS

# Core AWS services

* EC2 (elastic compute cloud): computers for diverse problems
  - Instance: type of hardware
  - AMI (Amazon Machine Image): an OS
  - Region: geographic location
  - AZ (availability zone): specific subset of a region
* EBS (elastic block store): virtual hard disks
  - More expensive than S3.
  - Mounts to an EC2 instance.
* S3 (simple storage service): long-term bulk storage
  - Like a Dropbox, without the nice GUI.
  - Meant to be accessed programmatically.
  - Does not require a running EC2 server to access, it is always
    available.
* DynamoDB: NoSQL database
  - Like MongoDB, but infinitely scalable

# AWS CLI

* Manage EC2 instances
* Some commands
  - `aws s3 ls` - lists s3 buckets
  - `aws ec2 describe-instances --output table`
  - `aws ec2 describe-instances --output json`
  - `aws help`
  - `aws ec2 help`

## Profiles

* The first time you run `aws configure`, you will be prompted for your
  credentials. Those will be your default creds from that point forward.
* Running with the option `--profile <some_profile_name>` creates a new
  profile with the credentials you subsequently specify.
* For anything but the default profile, you need to enter the
  `--profile <some_profile_name>` argument for it to work.

# SSH

Putting a `config` file in your `~/.ssh` allows you to run a very
simple command to connect to your server like so:
```
ssh <host-name>
```

Use `tmux` when you want to ensure that jobs do not stop when you close
the ssh connection.

# S3 Bucket

# Reference Material

## Extremely useful

* [AWS in plain English](https://www.expeditedssl.com/aws-in-plain-english)
  - This is one of the more useful references to read through. It
    explains each of the AWS services are and what they "should have
    been called."
* [EC2Instances.info](http://www.ec2instances.info/)
  - Very useful reference that lists the hourly prices for different EC2
    instances.

## Other

* [Open Guide to AWS](https://github.com/open-guides/og-aws)
* [AWS Documentation](https://aws.amazon.com/documentation/)
* [AWS Support](https://aws.amazon.com/premiumsupport/)
