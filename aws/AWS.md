## Amazon Web Services for Developers

- For this guide, I assume that you are a developer, or you have knowledge of basic concepts of software development, and I also assume that you have knowledge about server side development like APIs, SDKs.

### What is AWS?

- AWS is a cloud computing platform service
- As you know whenever any one talking about aws you have to go aws website, so let's start with https://aws.amazon.com/console/ I recommend going to the free version https://aws.amazon.com/free for learning.

### Introduced to AWS Console

- If you visit console.aws.amazon.com you will see a console dashboard which has various widgets which says "Recently Visited," "AWS Health," "Cost and usage", etc..
- From console, you can see the "Services" button by clicking on that it will show several AWS services which categorizes in different types of category like Analytics, Blockchain, Compute, Storage, Database, etc... 
- All categories contain different types of services like Compute has EC2, Lambda, etc...
- In the top right corner you can see your region, which is your default one, but you can change that by clicking on that button as well

![Screenshot 2023-09-18 at 9.39.52 AM.png](Screenshot%202023-09-18%20at%209.39.52%20AM.png)

### Security

- As with any platform where you have a profile or account, you should always need security.
- In AWS, you can manage security related stuff in IAM (Identity and Access Management) service.
- From console by clicking on the Services button, you can see Security, Identity and Compliance tab by clicking on that you will see IAM clicking on that you will redirect to IAM dashboard.
- Now, let's learn about primary concepts

    #### Users

    - By clicking on the Users you will see the Users tab, and in that you can create users, assign groups, describe policy to the specific account.
    - you can set policy via JSON obj as well
    - you can create policy, so whenever a new user gets created, you can assign them to created policy.
    
    #### Roles

    - this allows you to assign policies to a role that a service can adopt when it's running.
    - So if you have a Lambda that needs to access DynamoDB and SNS, you could create a role with those two and assign it to the Lambda. Then the Lambda would have permission for that.
  
    #### User groups

    - to add multiple users, we can create user groups. it is just a handy way to manage all users where you can define policies and all user level features to groups.