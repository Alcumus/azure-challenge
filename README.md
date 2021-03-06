Infrastructure Coding Test
==========================

# Goal
Script the creation of a web server, and a script to check the server is up.

# Prerequisites
You will need an Azure account. Create one if you don't own one already. You can use free-tier resources for this test.

# The Task
You are required to set up a new server in Azure. It must:

* Be publicly accessible.
* Run Nginx.
* Serve a `/version.txt` file, containing only static text representing a version number, for example:

```
1.0.6
```

# Mandatory Work
Fork this repository.

* Alter the README to contain the instructions required to:
  * Create and configure the resources.
  * Run the checker script.
* Provide a script that can be run periodically (and externally) to check if the server is up and serving the expected version number. Use your scripting language of choice.
* Provide scripts for the creation and configuration steps (it doesn't have to be a single script)



# Extra Credit
We know time is precious, we won't mark you down for not doing the extra credits, but if you want to give them a go...

* Use IAC software (such as terraform) to create the resources.
* Put the server behind a load balancer.
* Run Nginx inside a Docker container.
* Make the checker script SSH into the instance, check if Nginx is running and start it if it isn't.
* Have a domain name and a valid SSL certificate (Let's Encrypt) or be able to describe what would need to happen to get SSL certificate and a secure nginx configuration.

# Questions

#### What scripting languages can I use?
Any one you like. You’ll have to justify your decision. We use bash, Ansible and Terraform. However, feel free to pick something you're familiar with, as you'll need to be able to discuss it.

#### Will I have to pay for the Azure charges?
No. You are expected to use free-tier resources only and not generate any charges. Please remember to delete your resources once the review process is over, so you are not charged by Azure.

#### What will you be evaluating me on?
Scripting skills, elegance, understanding of the technologies you use, security, documentation.

#### Will I have a chance to explain my choices?
Feel free to comment your code or put explanations in a pull request within the repo.
If we proceed to a phone interview, we’ll be asking questions about why you made the choices you made.
