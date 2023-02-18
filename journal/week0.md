# Week 0 — Billing and Architecture

## AWS 
I created an AWS IAM account and provided adminstrative access to the account, created a Billing Full Access policy and attached the policy to the account.
Logged in to the admin account (IAM account) and changed my password, set up MFA and created access keys, also enabled console access.

<img width="818" alt="Screenshot 2023-02-18 at 05 43 01" src="https://user-images.githubusercontent.com/20463821/219869203-a574b719-06a0-445e-8f6a-aa943286afcc.png">

Created a Zero Spend Budget on my IAM account since I'm using a Free Tier

<img width="1065" alt="Screenshot 2023-02-18 at 05 51 18" src="https://user-images.githubusercontent.com/20463821/219869463-74de4555-9511-4bff-820c-97f56499dc5e.png">

## Gitpod
I integrated GitPod with GitHub and downloaded a browser extension for easy access. 

<img width="1003" alt="Screenshot 2023-02-18 at 05 52 28" src="https://user-images.githubusercontent.com/20463821/219869526-5e35030b-6221-4857-8f5e-a1eaf75f8b10.png">

## Logical Architectural Diagram
I recreated the Logical architectural diagram and also added some new information
Placing  WAF and CloudFront before the Application Loadbalancer will help monitor and filter malicious traffic from again access to the application. It prevents downtime and allows real users access the application. While CloudFront is used to bring the content closer to the user wherever they may be accessing the application from. It routes the content to the edge location closest to the user. Lastly added an SNS service where lambda functions give notification and received by the users, based on several checks. View the diagram on Lucid charts [here](https://lucid.app/documents/view/de284010-2d55-43f1-bda2-44f14965328f)

<img width="798" alt="Screenshot 2023-02-18 at 06 18 37" src="https://user-images.githubusercontent.com/20463821/219870823-822543d8-ab1f-4744-aad0-09d50e30db62.png">


## GitPod
Installed AWS CLI through Gitpod and created the budget (One Dollar Budget) through CLI, and setup billing alarms (through CloudWatch) and SNS topic

<img width="1063" alt="Screenshot 2023-02-18 at 06 08 45" src="https://user-images.githubusercontent.com/20463821/219870370-43735016-5323-4475-b99e-a2a2c50f4f5c.png">

<img width="913" alt="Screenshot 2023-02-18 at 06 12 23" src="https://user-images.githubusercontent.com/20463821/219870504-bae95ac4-32b2-4081-bbb5-6b1c1aa37c9b.png">

<img width="1069" alt="Screenshot 2023-02-18 at 06 13 17" src="https://user-images.githubusercontent.com/20463821/219870532-44e76c67-0c15-4333-b021-a313e7b8b72e.png">

## References
I made use of the following resources
- [Video](https://www.youtube.com/watch?v=OdUnNuKylHg&list=PLBfufR7vyJJ7k25byhRXJldB5AiwgNnWv&index=15) in the student portal 
- [AWS CLI documentation](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)
- [The CloudBootcamp Repo](https://github.com/omenking/aws-bootcamp-cruddur-2023/blob/week-0/journal/week0.md)

I learned a great deal. Thank you!
