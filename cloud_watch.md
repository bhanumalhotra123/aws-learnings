AWS CloudWatch for Enhanced Monitoring and Automation

Are you looking to keep a watchful eye on your AWS activities? 🕵️‍♂️ Look no further than AWS CloudWatch, your trusty sidekick for monitoring and optimizing your AWS resources!

Let's dive into the nitty-gritty of how to harness its power step-by-step:

1. Accessing the Command Center: CloudWatch Console
AWS CloudWatch is your service for real-time monitoring and actionable insights. Access its command center through the AWS Console.

2. Real-Life Metrics for Real Success
Imagine having a crystal ball for your AWS resources. CloudWatch provides real-time metrics for everything from API requests to memory utilization. Get ready to transform data into success!

3. Alarms: Proactive Measures
Don't just watch – take action. Set up CloudWatch alarms to receive notifications when metrics breach predetermined thresholds. Turn data into automated decisions!

4. Delving into Log Insights
CloudWatch not only monitors, but it logs. Dive into log groups and uncover every action, whether it's a successful project or a failed attempt. Your insights, your control!

5. Empowerment with Custom Metrics
CloudWatch is flexible, but what if you need something unique? Integrate custom metrics to enhance monitoring capabilities. Make CloudWatch work for you!

6. Cost Optimization: Making Every Bit Count
It's not just monitoring; it's about optimizing costs. CloudWatch collaborates with other services to trigger actions and maximize efficiency. Your wallet will thank you!

Let's Make It Practical: Monitoring CPU Utilization on EC2

Launch an EC2 Instance: Start by launching an EC2 instance through the EC2 dashboard.

SSH In: Securely access your instance via SSH using the key pair.

Initial CPU Check: Run commands to gauge initial CPU utilization using tools like top or htop.

Browse CPU Metrics: In CloudWatch, find "Metrics" and pick the EC2 service. Explore "Per-Instance Metrics" and locate "CPUUtilization."

Detailed Monitoring: Go to your instance's "Monitoring" tab and enable "Detailed Monitoring" for 1-minute intervals.

Increase CPU Load: Execute an app/script to significantly utilize CPU resources. Get ready to see metrics in action!

Watch the Spike: Back in CloudWatch Metrics, witness the spike in "CPUUtilization" as your app kicks in.

Create an Alarm: In CloudWatch, select "Alarms," then "Create Alarm." Choose the metric (CPUUtilization) and resource (your EC2 instance).

Configure SNS Topics: While creating the alarm, set up an SNS topic for notifications. Specify your email as the endpoint.

Define Alarm Details: Give your alarm a name and a notification message that delivers a punch.

Confirm Subscription: Check your email, confirm the subscription, and get ready for notifications.

Test the Alarm: Run your app/script again and enjoy the triumphant ding of your email notification!



![image](https://github.com/bhanumalhotra123/aws-learnings/assets/144083659/9ba737a0-ea53-47c2-ad1f-40cba0f3844b)
![image](https://github.com/bhanumalhotra123/aws-learnings/assets/144083659/78f70289-e23a-49d9-bc48-56feb20c1973)
![image](https://github.com/bhanumalhotra123/aws-learnings/assets/144083659/6207d4b6-48cf-442e-942d-715beff2183c)
![image](https://github.com/bhanumalhotra123/aws-learnings/assets/144083659/dd464574-dafb-45d5-b64f-59f92729336c)
![image](https://github.com/bhanumalhotra123/aws-learnings/assets/144083659/1c80245e-03c9-43e4-a102-e47636125f88)
![image](https://github.com/bhanumalhotra123/aws-learnings/assets/144083659/78624beb-289a-46da-b10b-085250ad8f65)
![image](https://github.com/bhanumalhotra123/aws-learnings/assets/144083659/f4f2e9c2-3608-4231-bd59-e8c4e4d0cda8)



