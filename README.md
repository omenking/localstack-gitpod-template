# LocalStack Gitpod Template

This gitpod environment will automatically install and start localstack.

To start using localstack go to the terminal named `aws-cli` and enter the following commands to give it a try:

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