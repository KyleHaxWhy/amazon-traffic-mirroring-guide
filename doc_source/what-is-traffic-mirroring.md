# What Is Traffic Mirroring?<a name="what-is-traffic-mirroring"></a>

Traffic Mirroring is an Amazon VPC feature that you can use to copy network traffic from an elastic network interface of Amazon EC2 instances and then send it to out\-of\-band security and monitoring appliances for content inspection, threat monitoring, and troubleshooting\. These appliances can be deployed as individual instances, or as a fleet of instances behind a Network Load Balancer with a User Datagram Protocol \(UDP\) listener\. Traffic Mirroring supports filters and packet truncation, so that you only extract the traffic of interest to monitor by using monitoring tools of your choice\.

## Traffic Mirroring Concepts<a name="concepts"></a>

The following are the key concepts for Traffic Mirroring:
+ **Target** — The destination for mirrored traffic\.
+ **Filter** — A set of rules that defines the traffic that is copied in a Traffic Mirror session\.
+ **Session** — An entity that describes Traffic Mirroring from a source to a target using filters\.

## Working with Traffic Mirroring<a name="traffic-mirroring-use-cases"></a>

You can create, access, and manage your Traffic Mirror resources using any of the following interfaces:
+ **AWS Management Console**— Provides a web interface that you can use to access your Traffic Mirror resources\.
+ **AWS Command Line Interface \(AWS CLI\)** — Provides commands for a broad set of AWS services, including Amazon VPC, and is supported on Windows, macOS, and Linux\. For more information, see [AWS Command Line Interface](https://aws.amazon.com//cli/)\.
+ **AWS SDKs** — Provide language\-specific APIs and takes care of many of the connection details, such as calculating signatures, handling request retries, and error handling\. For more information, see [AWS SDKs](https://aws.amazon.com/tools/#SDKs)\.
+ **Query API**— Provides low\-level API actions that you call using HTTPS requests\. Using the Query API is the most direct way to access Amazon VPC, but it requires that your application handle low\-level details such as generating the hash to sign the request, and error handling\. For more information, see the [Amazon EC2 API Reference](https://docs.aws.amazon.com/AWSEC2/latest/APIReference/)\.

## Traffic Mirroring Benefits<a name="traffic-mirroring-benefits"></a>

Traffic Mirroring offers the following benefits:
+ **Simplified operation** — Mirror any range of your VPC traffic without having to manage packet forwarding agents on your EC2 instances\.
+ **Enhanced security** — Traffic Mirroring captures packets at the elastic network interface, which cannot be disabled or tampered with from a user space\.
+ **Increased monitoring options** — You can send your mirrored traffic to any security device\.

## Pricing<a name="pricing"></a>

For information about pricing, see [VPC pricing](https://aws.amazon.com/vpc/pricing/)\.