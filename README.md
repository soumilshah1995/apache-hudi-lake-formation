![image](https://user-images.githubusercontent.com/39345855/215276228-bfb10f6c-4b9f-4efb-8dd5-0393a39b2b13.png)


* Let's look at how we get fine-grained access to hudi Datalake using AWS Lake formation. In this video, I'll teach you how to restrict intern and analyst access to specific columns by using lake formation.


# Video Guide : 


#### Note
* When you create user analyst or intern make sure to add this policy and role 
```
Policy Name : AmazonAthenaFullAccess
Inline Policy : 
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Action": [
                "s3:Put*",
                "s3:Get*",
                "s3:List*"
            ],
            "Resource": [
                "arn:aws:s3:::XXXX/*"
            ],
            "Effect": "Allow"
        }
    ]
}

```





