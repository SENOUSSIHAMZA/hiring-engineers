##Prerequisites - Setup the environment

Before starting the assignment I made a priliminary research on Datadog Doc to see how it exactly works.

I'm working on a Linux Ubuntu 16.04 OS.

As recommended I used a Vagrant environment.
![vagrant-setup](https://user-images.githubusercontent.com/25555806/42341848-551f4e78-808c-11e8-9c3d-97b069209ede.png)
![vagrant-setup2](https://user-images.githubusercontent.com/25555806/42341885-73ba7b28-808c-11e8-9de3-927829463189.png)


### Add tags in the Agent config file and show a screenshot of my host and its tags on the Host Map page in Datadog.

To start this task I made a quick research on Datadog help forum to know where the Agent file is located (https://help.datadoghq.com/hc/en-us/articles/203037169-Where-is-the-configuration-file-for-the-Agent-).

I installed Datadog Agent
![instaling datadog agent](https://user-images.githubusercontent.com/25555806/42343707-d6218216-8091-11e8-86b9-f8405bec4d76.png)

Then I followed the Doc to assign tags on datadog.yaml


![assigntags](https://user-images.githubusercontent.com/25555806/42344024-ec27eb08-8092-11e8-8615-127b249766f8.png)

And had the tags displayed :

![tags-on-agent](https://user-images.githubusercontent.com/25555806/42344262-acd9806e-8093-11e8-9fa0-5eefcd9b1ac2.png)

### Install a database on your machine (MongoDB, MySQL, or PostgreSQL) and then install the respective Datadog integration for that database.
For the next step I needed to install MySql database on my machine and install the respective Datadog integration for that database.
![msql-integration1](https://user-images.githubusercontent.com/25555806/42344580-af4aebca-8094-11e8-9f0e-86ddc7ed108b.png)

![msql-integration-2](https://user-images.githubusercontent.com/25555806/42344601-c18e7bee-8094-11e8-8885-5dcf1e011e46.png)

and it worked !


![inetgration-success](https://user-images.githubusercontent.com/25555806/42344824-67c3a7be-8095-11e8-8d7e-2610c73c3b2b.png)

### Create a custom Agent check that submits a metric named my_metric  a random value between 0 and 1000.

Here's my my_metric.py:

![mymetricpy](https://user-images.githubusercontent.com/25555806/42345175-6f1a21a4-8096-11e8-87b4-adf2480e2f20.png)

Then I put my my_metric.yaml in the /conf.d directory.

### Change your check's collection interval so that it only submits the metric once every 45 seconds.

 I did this by editing the my_metric.yaml file so that it specifies the collection interval, If min_collection_interval is not specified, the check would run about every 15-20 seconds.

### Bonus Question Can you change the collection interval without modifying the Python check file you created?

Yes, by editing the my_metric.yaml file.


## Is there anything creative you would use Datadog for?

I am a data scientist, and I think that dataog could be a very helpful use to companies in order to collect and Visualize data no matter what field they are working on.
I think that adding some machine learning functunalities as MLaaS would be a useful add to datadog and will help it bring more customers and more companies to use the platform.


