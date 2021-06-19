# Magento On Amazon Web Service

**Magento on AWS:**

```   
    * Magento is an open-source content management system for e-commerce websites. AWS enables you to set up the infrastructure to support Magento deployment in a flexible, scalable, and cost-effective manner in the AWS Cloud.
```         

* Magento Open Spource -> AWS cloud:

    ![magento-on-aws](https://user-images.githubusercontent.com/2525741/122633893-95492e00-d0f8-11eb-875a-0fdf371cfe4c.jpeg)

* AWS services:

```
    1. Amazon EC2 – The Amazon Elastic Compute Cloud (Amazon EC2) service enables you to launch virtual machine instances with a variety of operating systems. use to build and host your software systems.
    
    2. Amazon VPC – The Amazon Virtual Private Cloud (Amazon VPC) service lets you provision a private, isolated section of the AWS Cloud where you can launch AWS services and other resources in a virtual network that you define. You have complete control over your virtual networking environment, including selection of your own IP address range, subnet creation, and configuration of route tables and network gateways.

    3. Amazon ElastiCache(Redis) – The Amazon ElastiCache service makes it easy to deploy, operate, and scale an in-memory data store or cache in the cloud. The service improves the performance of web applications by allowing you to retrieve information from fast, managed, in-memory data stores, instead of relying entirely on slower disk-based databases.

    4. Amazon EFS – Amazon Elastic File System (Amazon EFS) provides simple, secure, durable, highly scalable file storage for use with EC2 instances. Here Magento deployment uses Amazon EFS to share and retrieve common media assets by web server instances.
    
    5. Amazon RDS – Amazon Relational Database Service (Amazon RDS) makes it easy to set up, operate, and scale a growing set of relational databases, including MySQL and Amazon Aurora, both of which are supported by the Magento Quick Start. With Amazon RDS, you can deploy scalable relational databases in minutes with cost-efficient and resizable hardware capacity.

    Note :

    * Before you launch this Quick Start, confirm that Amazon EFS is supported in the Region where you’re planning to deploy Magento.
    
    * Auto Scaling – Auto Scaling helps maintain high availability and manage capacity by automatically increasing or decreasing the EC2 instance fleet. You can use Auto Scaling to run your fleet at optimal utilization by increasing instance capacity during demand spikes and decreasing capacity during down times.

    * Elastic Load Balancing – Elastic Load Balancing automatically distributes incoming application traffic across multiple EC2 instances.
    
    * IAM – AWS Identity and Access Management (IAM) enables you to securely control access to AWS services and resources for your users. With IAM, you can manage users, security credentials such as access keys, and permissions that control which AWS resources users can access, from a central location.
```

* Deployment Scenarios:

```
    * Deploy Magento into a new VPC (end-to-end deployment). This option builds a new AWS environment consisting of the VPC, subnets, NAT gateways, security groups, and other infrastructure components, and then deploys Magento into that new VPC.

    * Deploy Magento into an existing VPC. This option provisions Magento in your existing AWS infrastructure.
```

* Deployment steps:

    Step 1. Prepare an AWS Account

```    
        * Create an AWS account(http://aws.amazon.com)
        
        * Choose the AWS Region where you want to deploy the Magento cluster on AWS.
  
        * Create a key pair in your preferred region
```

      ![create-key-pair](https://user-images.githubusercontent.com/2525741/122653031-9d888400-d15f-11eb-858f-41e08af67455.png)


   Step 2. Download the Magento Software

```
        *  Add the Magento downloaded files to the S3 bucket

```

   Step 3. Launch the Quick Start

```        
        * Deploy Magento into a new VPC on AWS (launch the AWS CloudFormation template into your AWS account.)
```

   Step 4. Test Your Magento Deployment 

```    
        * When the AWS CloudFormation template has successfully created the stack, all web server nodes will be running with the software installed in your AWS account. To connect to the Magento stack, use the URL of the Elastic Load Balancing endpoint

```

   ![elb-endpoint](https://user-images.githubusercontent.com/2525741/122653044-b002bd80-d15f-11eb-9cd3-c2ec8fe027e2.png)
   
   ![web-store](https://user-images.githubusercontent.com/2525741/122653056-c01a9d00-d15f-11eb-90d4-8b7badf8c936.png)

