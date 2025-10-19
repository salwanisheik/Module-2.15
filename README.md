# IAM Policy
Below is an example IAM policy that allows the EC2 instance to retrieve the secret prod/cart-service/credentials:
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Action": [
        "secretsmanager:GetSecretValue",
        "secretsmanager:DescribeSecret"
      ],
      "Resource": "arn:aws:secretsmanager:ap-southeast-1: 255945442255:secret:prod/cart-service/credentials-AbCdEf"
    }
  ]
}

