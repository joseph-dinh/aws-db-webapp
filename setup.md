Sign in to your AWS account
If you don't have one the free tier account for AWS is sufficient
Head to the RDS Management Console databases tab from the AWS dashboard and click create database
![image](https://user-images.githubusercontent.com/118394420/225163937-0e49eb00-ebd0-4da4-86cb-4591a84ab8bc.png)

Select Easy Create and choose a database, I will be using PostgreSQL.
![image](https://user-images.githubusercontent.com/118394420/225164056-f7c3506b-d0af-446a-a330-9741e74ce189.png)

Once you have created your database, you should see your Database in your Databases tab in the Amazon RDS dashboard.
Click on your database and click on your inbound EC2 security group rules.
![image](https://user-images.githubusercontent.com/118394420/225167941-e2b9aa37-7040-4a5e-97dd-1596470fbecf.png)
![image](https://user-images.githubusercontent.com/118394420/225167977-68f7b687-9017-4eb2-8702-f2932064fec4.png)

Edit inbound rules and add a rule that allows
Type - All traffic, source My IP.
This allows only our IP to access our database that we just created in AWS so we can begin testing.
Keep in mind that we will need to allow the IP of the web server too later when we push to production.
![image](https://user-images.githubusercontent.com/118394420/225168015-f651dbdc-59b7-408c-bad9-cff522e0f388.png)
![image](https://user-images.githubusercontent.com/118394420/225168214-3f6ca8e0-d19a-4bcf-a251-761c240f70d6.png)

