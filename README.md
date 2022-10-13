# LocalStack Gitpod Template

Click the button below to start a new development environment:

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#hhttps://github.com/omenking/localstack-gitpod-template)

This gitpod environment will automatically install and start localstack.

To start using localstack go to the terminal named `aws-cli` and enter the following commands to give it a try:

> You need to wait for the LocalStack Server to run, check the localstack terminal tab and make sure its running before executing any of the commands below.

## Example:

### Create an S3 Bucket
```sh
awslocal s3 mb s3://my-bucket
```

### List as S3 Buckets
```sh
awslocal s3 ls
```

### Upload a File
```sh
echo "Hello World" >> file.txt
awslocal s3 cp file.txt s3://my-bucket
```

### Download a File
```sh
awslocal s3 cp s3://my-bucket/file.txt /tmp/file2.txt
cat /tmp/file2.txt
```