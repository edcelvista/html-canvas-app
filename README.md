{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "AllowSpecificIPs",
            "Effect": "Allow",
            "Principal": "*",
            "Action": "s3:GetObject",
            "Resource": "arn:aws:s3:::edcelvistadotcom-others/*",
            "Condition": {
                "IpAddress": {
                    "aws:SourceIp": "180.191.98.163/32"
                }
            }
        }
    ]
}