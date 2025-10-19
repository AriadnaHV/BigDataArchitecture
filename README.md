# BigDataArchitecture
Deliverable for earning credit in this module.

In this project, I used Google Cloud Platform to create and configure a Dataproc Hadoop cluster, a Cloud Storage Hadoop bucket, and a ComputeEngine ElasticSearch VM instance. 
Then I connected them, added some data into the ElasticSearch instance from the Hadoop cluster, and finally ran some simple data analytics using Kibana.

Part 1) Creation and configuration of a Hadoop cluster to be used in connection with an ElasticSearch-Kibana VM instance.
a) In Dataproc, I created a Hadoop cluster, deciding on where to set up the machines (region), what type of machines to use, how to provision them, how to access them, etc.
b) In Cloud Storage, I create a bucket for connecting to the cluster and loaded the elasticsearch-hadoop and commons-httpclient configuration jar files into it.
c) Finally, from the cluster's master node SSH, I uploaded those jar files from the bucket into the Hadoop cluster.

Part 2) Creation and configuration of an ElasticSearch & Kibana VM instance.
a) I created a new VM instance in ComputeEngine cluster, deciding on the region, type of machine, how to provision it, how to access it, etc.
b) I properly configured the ElasticSearch software, modifying the elasticsearch.yml file.
c) I also set up the firewalls that enable connection with the Hadoop cluster and the ElasticSearch & Kibana instance. 

Part 3) Configuration of the connection between the Hadoop cluster and the ElasticSearch instance, loading the appropriate jar files and modifying them for configuring Hive, including restarting of Hive.

Part 4) From the ElasticSearch server, creation of an index in json format, and then from the Hadoop cluster, aggregation of data to the index created in the ElasticSearch server, making use of the Hive connector.

Part 5) From the Kibana graphic interface, perform some very simple data analysis and produce graphs.
