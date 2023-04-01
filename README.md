# Deploy a high-availability web app using CloudFormation

In this project, I create a dummy application and provision the required infrastructure. This includes setting up compute, networks, load balancers and security rules.

# Deployment

Run the create.sh file to initiate deployment with AWS CloudFormation.

`.\create.sh udagram udagram_infra.yml udagram_params.json`

![Deployment progress](create_in_progress.PNG)

# Output
Once completed, the dummy web app can be tested by calling the load balancer url

![web app screenshot](load_balancer_url.PNG)

# Challenges

Installing apache via apt-get did not work as expected. I have to install httpd via yum in order to create a webserver
