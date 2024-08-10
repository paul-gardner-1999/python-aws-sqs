# python-aws-sqs
Simple tests with was sqs

### Prerequisites
* docker desktop
* aws cli

## Set up awslocal to access localstack s3
```bash
alias awslocal='AWS_ACCESS_KEY_ID="test" AWS_DEFAULT_REGION="us-east-1" AWS_SECRET_ACCESS_KEY="test" aws --endpoint-url=http://localhost:4566'
```

## Spin up environment
```bash
docker compose up --detach
awslocal cloudformation deploy --stack-name demo --template-file ./cloud-formation.yml
```