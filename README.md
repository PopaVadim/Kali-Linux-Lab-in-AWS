<h1>Kali Linux Lab in AWS</h1>

<h2>Description</h2>
This project is a walkthrough of how to create a Kali Linux lab in the Cloud using an AWS Free Tier Account. These services allow us to get some exposure and hands-on experience with AWS Cloud Services free of charge for a period of 1 year. We have the option to receive more services than the Free Tier offers for the standard Amazon rates. To avoid any unwanted charges we will set up Amazon Alerts if we are getting close to consuming our Free Tier limits. 
 
<br />


<h2>Environments and Utilities Used</h2>

- <b>AWS</b>
- <b>Kali Linux</b>
- <b>MacOS</b> 
- <b>Xfce Desktop Envoirment<b/>
- <b>TightVNC<b/>
- <b>Terminal</b> 

<h2 align="center">Project walk-through</h2>
<p align="center">
<b>Below we will show how to create an Amazon Free Tier Account.</b> <br/> <br />

<b>First we will browse to https://aws.amazon.com then at the top right hand corner we will click "Create an AWS Account"</b><br/>
<b></b> <br/>
<img width="1502" alt="Screen Shot 2023-01-06 at 4 23 12 PM" src="https://user-images.githubusercontent.com/117952272/211168408-402939ba-40e0-43c0-a311-35224b37c57e.png">
<br/>

<b>Next in order to create an AWS account you will be asked to provide your Root user email address and an AWS account name. When you are finished click on Verify email address.<b/></b><br/>

<img width="1471" alt="Screen Shot 2023-01-06 at 4 26 10 PM" src="https://user-images.githubusercontent.com/117952272/211392415-86ff62cb-8650-4877-873f-5bdf3f9d978b.png">
<br/><br/>

<b>After your email was succesfully verified you will be prompted to create the Root User password. When you are done press the Continue.<b/>
<br/>

<img width="1225" alt="Screen Shot 2023-01-06 at 4 27 55 PM" src="https://user-images.githubusercontent.com/117952272/211393493-a64d04dc-1c00-481c-96d9-6d2762b3cc2d.png">
<br/><br/>

<b>The following step will be filling up the Contact Information and clicking to acknowledging the AWS Customer Agreement and press Continue again.<b/><br/><br/>
<img width="1064" alt="Screen Shot 2023-01-06 at 4 29 32 PM" src="https://user-images.githubusercontent.com/117952272/211395062-83b0e5e1-40ba-4095-9cf0-8ace034d3f23.png">
<br/><br/>

<b>As a final step we will have to choose a support plan. In our case the Free Basic support covers all our needs for this particular lab. When we are ready we will press Complete sign up to finalize our AWS account set up.<b/>
<br/><br/>
 
<img width="899" alt="Screen Shot 2023-01-06 at 4 33 49 PM" src="https://user-images.githubusercontent.com/117952272/211396018-5ed7511c-e2cf-4b5f-9f06-4e35403dcf03.png">
<br/><br/>

<b>Now the account is being created we are just waiting for an email confirmation. As soon as we received it, we will be able to access AWS Management Console and start enjoying our Free Tier Account.<b/> 
<br/><br/>
<img width="1471" alt="Screen Shot 2023-01-06 at 4 35 40 PM" src="https://user-images.githubusercontent.com/117952272/211396984-1c5aebfb-f14e-4f43-84e6-b7b29a4064f1.png">
<br/><br/>

<b>Now we will set up Multifactor Authentication to secure our AWS account and all our AWS resources. To do that we will go to the Services tab and click Security and find Identity and Access Management then click on Assign MFA.<b/>
<br/><br/>
<img width="1488" alt="Screen Shot 2023-01-06 at 4 46 41 PM" src="https://user-images.githubusercontent.com/117952272/211407658-98b79f94-534e-426e-af1a-3d4020dd1fda.png">
<br/><br/>

<b>Then we will be prompted to specify the multifactor authentication device we want to use. You choose the one that works the best for you.<b/>
<br/><br/>

<img width="1202" alt="Screen Shot 2023-01-06 at 4 47 20 PM" src="https://user-images.githubusercontent.com/117952272/211408843-454424fa-8ab9-48ae-8065-e24fb75fd9f0.png">
<br/><br/>

<b>Below we can see that the Multifactor Authentication was successfully assigned.<b/>
<br/><br/>
<img width="1491" alt="Screen Shot 2023-01-06 at 4 51 46 PM" src="https://user-images.githubusercontent.com/117952272/211409700-45676417-2cf1-47ee-9863-30429f039557.png">
<br/><br/>

<b>To avoid any potential unwanted charges we will set up a billing alarm that will be triggered if the threshold exceeds 10 US dollars. The Billing Alarm will let us know immediately if this condition is met and send us a notification to the email we choose.<b/> <br/><br/>
<p align="center">
<b>See how to set the Billing Alarm in the steps below:<b/>

<img width="1491" alt="Screen Shot 2023-01-06 at 4 53 11 PM" src="https://user-images.githubusercontent.com/117952272/211415598-cc333fdd-d16b-4c0c-8956-ae27da517d50.png">


<img width="1488" alt="Screen Shot 2023-01-06 at 4 56 18 PM" src="https://user-images.githubusercontent.com/117952272/211415653-9583e312-351e-4180-b8aa-131dd3bc6e22.png">
 
 
<img width="1274" alt="Screen Shot 2023-01-06 at 4 58 41 PM" src="https://user-images.githubusercontent.com/117952272/211415679-26963b94-e680-46f4-82e2-3de1595c0784.png">


<img width="1279" alt="Screen Shot 2023-01-06 at 4 59 51 PM" src="https://user-images.githubusercontent.com/117952272/211415708-a014d3be-5984-46ff-873c-d3854b559ee7.png">
 
<img width="1383" alt="Screen Shot 2023-01-06 at 5 00 57 PM" src="https://user-images.githubusercontent.com/117952272/211415763-d4fb7251-acc1-4b89-9e52-f36766db4770.png">


<img width="1267" alt="Screen Shot 2023-01-06 at 5 03 46 PM" src="https://user-images.githubusercontent.com/117952272/211415946-d5899289-62cd-4af6-af5a-31ec7208c9dc.png">


<img width="1458" alt="Screen Shot 2023-01-06 at 5 05 28 PM" src="https://user-images.githubusercontent.com/117952272/211415958-751f546c-501e-41c7-91cf-03e1e0894797.png">
