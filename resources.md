---
layout: default
title: Resources
permalink: "/resources/"
sort_order: 2
---

# Available Resources

Thanks for participating! Below is a list of the server resources available, provided by [Amazon Web Services][aws]. Please [email Daniel Ryan][daniel_at_openchattanooga] to request a resource.

## App Servers

We have 5 flavors of app servers available:

* Ubuntu Server 14.04 LTS
* Red Had Enterprise Linux 6.5
* SuSE Linux Enterprise Server 11 sp3
* Amazon Linux 2014.03.1
* Microsoft Windows Server 2012 Base

By default, all servers are t1.micro with 0.6 GB of RAM and 8 GB of attached storage. Larger [EC2 Instance Types][ec2_types] are available; please let Daniel know if you need a larger instance or more storage added.

Additionally, if you'd prefer to use [OpsWorks][opsworks], just let us know.

### Connecting to App Servers over SSH

When your servers are ready, you'll receive a pem encoded SSH key and the URL of the server. To connect, run the following in a terminal window:

```ssh -i <path/to/key.pem> <username>@<url>```

Usernames are:

* Ubuntu: ubuntu
* RHEL: ec2-user
* SuSE: root
* Amazon Linux: ec2-user
* Windows: ec2-user

On *nix systems, you can gain root access once you've logged in by running `sudo su`.

## Databases

You may choose to install a database on your app server, however, we recommend using [RDS][rds] for relational databases or [DynamoDB][dynamodb] for NoSQL. RDS supports the following databases:

* MySQL
* PostgreSQL
* Oracle Standard or Enterprise Edition
* Microsoft SQLServer Web, Standard or Enterprise Edition

## File Storage

Static file storage is available via [S3][s3] and [Glacier][glacier]. Let us know how many storage buckets you need.

## Additional Services

The full suite of [AWS][aws] products are available. A few we recommend:

* [Route53][route53] for DNS
* [ElastiCache][elasticache] for Memcache
* [Elastic MapReduce][emr] for Big Data analysis via Hadoop
* [SES][ses] for sending email
* [SQS][sqs] for queueing messages
* [SWF][swf] for automating tasks

[aws]: http://aws.amazon.com/ "Amazon Web Services"
[daniel_at_openchattanooga]: mailto:daniel@openchattanooga.com "Email Daniel Ryan"
[ec2_types]: https://aws.amazon.com/ec2/instance-types/ "EC2 Instance Types"
[opsworks]: https://aws.amazon.com/opsworks/ "AWS OpsWorks"
[rds]: https://aws.amazon.com/rds/ "AWS Relational Database Service"
[dynamodb]: http://aws.amazon.com/dynamodb/ "AWS DynamoDB"
[s3]: http://aws.amazon.com/s3/ "AWS Simple Storage Service"
[glacier]: http://aws.amazon.com/glacier/ "AWS Glacier"
[route53]: http://aws.amazon.com/route53/ "AWS Route53"
[elasticache]: http://aws.amazon.com/elasticache/ "AWS ElastiCache"
[emr]: http://aws.amazon.com/elasticmapreduce/ "AWS Elastic MapReduce"
[ses]: http://aws.amazon.com/ses/ "AWS Simple Email Service"
[sqs]: http://aws.amazon.com/sqs/ "AWS Simple Queue Service"
[swf]: http://aws.amazon.com/swf/ "AWS Simple Work Flow"
