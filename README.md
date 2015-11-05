#Setting up the Pipeline

###Requirements

- AWS account
- Github account
- EC2 Bitnami Jenkins AMI

###Step One : Configure Jenkins

* From console, navigate to EC2 and create an instance.  Use the *Bitnami Jenkins* AMI from the marketplace.

* Assign/Create the _________ role/service for Jenkins.

* Launch instance.

###Step Two : Create Pipeline

* From the console, navigate to **Code Pipeline.**

* **WRITE IN STEPS for how to configure the pipeline

* Remove the deploy stage as we will **not** be using Code Deploy to launch our containers.

###Step Three : Set-Up Bitnami Jenkins

* Create a freestlye project using the name you defined in build stage of the pipeline

* Check the *EXECUTE BUILD MULITPLE TIMES OR SOMETHING LIKE THAT*

* Check the Poll SCM and enter :

```
* * * * *
```

* Click to add a build stage and choose **Docker Build and Publish**

Enter into the following fields

**Pull a screen shot here of the fields and what I entered into them**

* Click to add a AWS Publish stage and leave the location field blank.

* Click *Apply* and *Save*

 Now from your terminal ssh into the EC2 instance in which Jenkins resides :
```
ssh -i *key.pem* ubuntu@*public_ip_address* 
```

* Create a JSON file with the following configuration.
```
ENTER THE flask-signup.json file
```



