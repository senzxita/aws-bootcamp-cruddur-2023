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

<img width="811" alt="Screenshot 2023-02-18 at 05 55 07" src="https://user-images.githubusercontent.com/20463821/219869660-c4c47b9f-c6f1-49cc-b42d-3a200ebe964c.png">

## GitPod
Installed AWS CLI through Gitpod and created the 

