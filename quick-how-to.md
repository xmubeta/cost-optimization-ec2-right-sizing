This is a quick guide to deploy EC2 right sizing solution.

You can lauch it in BJS region or ZHY region. The result will cover all EC2s in both regions.

1.	Go to cloudformation (You need Admin permission)

2.	Create a stack with the following template
https://s3.cn-north-1.amazonaws.com.cn/right-sizing/right-sizing.json

![image](https://github.com/xmubeta/cost-optimization-ec2-right-sizing/blob/master/images/step-1.jpg)

3. Supply with some parameter: (Specify Access CIDR Block with your IP if you want to access the right-sizing EC2)

![image](https://github.com/xmubeta/cost-optimization-ec2-right-sizing/blob/master/images/step-2.jpg)

4. Acknowledge the IAM creation and start to create

![image](https://github.com/xmubeta/cost-optimization-ec2-right-sizing/blob/master/images/step-3.jpg)

5. It could take 15 minutes or more. After it completes, you will find the results in the s3 bucket:

![image](https://github.com/xmubeta/cost-optimization-ec2-right-sizing/blob/master/images/step-4.jpg)

6. Check the results for recommended instance types:

![image](https://github.com/xmubeta/cost-optimization-ec2-right-sizing/blob/master/images/step-5.jpg)
