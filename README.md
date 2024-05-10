# IAM
*** AMAZON WEB SERVICES ***

IAM (Identity and Access Management)

* What is IAM?
-> AWS IAM is a web service that helps you to securely control access to AWS Resources.
-> With IAM, you can centrally manage permissions that control which AWS Resources users can access.
-> You use IAM to control who is authenticated (signed in) and authorized (has permissions) to use resources.

* IAM Features
1. Shared access to your AWS account.
2. Granular permissions.
3. Secure access to AWS resources for applications that run Amaozon EC2.
4. Multi-factor authentication.
5. Identity federation.
6. PCI DSS Compliance.
7. Integrated with many AWS Services.
8. Eventually consistent.
9. Free to use.

* Users
Q. How to create user?
-> Go to management console -> Search IAM -> Go to users -> Click create user -> Provide a name and tick "Provide user access to AWS Management Console" -> Create a password for the user.
-> Then set permisssions to that user for accessing AWS services-
1. Add user to group
2. Copy permissions.
3. Attach policies directly.
Usually, we select 3rd option. Then select policies to assign to user for eg. FullS3Access. This will give user the permissions to access full S3 service.
-> Review and then create user.

* Groups
-> Instead of creating number of users and attaching policies to all the users individually, we should create group.
-> In groups, we add users and we can attach policies directly to the group. 
-> So that by default whatever user is added to group that users will get those permissions automatically.

* Policies
-> A policy is an object in AWS that defines permissions.
-> By default AWS has created a lot of policies for us.
-> But we can also create the policies ourselves and then assign to users or groups.

* Roles
-> Role is an identity within an AWS account that has specific permissions.
-> IAM Roles are similar to IAM users, but they aren't associated with a specific person.
-> Instead roles are used to connect AWS services.

* Best practices for AWS IAM
1. Use groups instead of individual users.
2. Use least priviledge.
3. Use multi-factor authentication.
4. Use strong passwords.
5. Rotate credentials.
6. Audit logs.
7. Use policy connections.
8. Set permissions guardrails.
9. Ensure IAM groups don't have administrative permissions.
10. Ensure that your AWS Cloud account has a strong IAM password policy in use.

Note:- 
1. A single user can be added to multiple groups.
2. An AWS account can have upto 5000 users.
3. An AWS account can have upto 1000 roles.
4. You can assign one IAM user to upto 10 groups.
5. You can also attach upto 10 managed policies to each group.
