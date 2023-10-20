# Service Level Model of Cloud

As you've discovered, Cloud Computing Services are a complex set of hundreds of offering and of course we humans like to put 
things into an organizational framework.   

The [NIST definition of cloud computing](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-145.pdf) defines what
cloud computing is, but also defines the so-called service models.   The convention is to take some aspect of IT, and add the suffix 
"...as a service" which is abbreviated "aaS."   This is based on the 'stack model' of IT, where each layer of functionality depends on the layer below. 

**Broad overview of service models**

* Infrastructure as a Service (IaaS):  What your IT department would provide, Nuts and bolts, DIY, Lego.  You need understanding of computing architecture as these services 
* Platform as a Service (PaaS): Everything in between, or pre-configured and managed infrastructure
* Software (aaS): Little to no configuration is needed but these system may be programmable and integrated with other services.  E.g. Office 365, Google Drive

![aaS](https://cloudtweaks.com/wp-content/uploads/2014/07/cloud-stack-images.png)

![Oracle stack model diagram](https://i1.wp.com/oracle-help.com/wp-content/uploads/2017/08/Cloud-Service-Models.png?resize=611%2C326)

I believe a sweet-spot for researchers who do not have time to aquire the expertise to manage low-level infrastructure and need something more flexible and programmable than Software, are the platforms.  These are often more expensive than DIY infrastruture, but are faster to provision and provide security controls. 

#### Cloud "Services" and the Packaging of Open Source Systems

Case Study on Open Source system as Cloud service: **MySQL **

Open source, free Relational database, e.g. SQL. Relational databases store tabular, linked data.   Used by some bioinformatics packages (e.g. https://orthomcl.org/orthomcl/app) and millions of websites. 

  * project: https://www.mysql.com/products/community/ and  https://mariadb.org/
  * DIY on Azure instructions (eg Iaas): [someone's DIY Mysql](https://github.com/Huachao/azure-content/blob/master/articles/virtual-machines/virtual-machines-linux-install-mysql.md) - don't follow these, they are old and may not work, just an example of the steps involved
  * Azure MySQL Service (e.g PaaS): [Azure Database for MySQL](https://azure.microsoft.com/en-us/services/mysql/) 
     * AWS MySQL Service: [Amazon RDS for MySQL](https://aws.amazon.com/rds/mysql/)
     * Google MySQL Service [Cloud SQL](https://cloud.google.com/sql/) 
  * other companies, such as [Aiven for MySQL](https://aiven.io/mysql)

  * Spin-offs: Amazon also offers [AWS Aurora](https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/CHAP_AuroraOverview.html)  which is a cloud scale database service that is MySQL-compatible see [Amazon Aurora Paper](https://dl.acm.org/doi/10.1145/3035918.3056101) 

What would a "SaaS" offering for your research look like?  A "Google Docs" for your databases?  How about a "PasS" that you could build?   Would it be reproducible by anyone doing the kind of research you do? 