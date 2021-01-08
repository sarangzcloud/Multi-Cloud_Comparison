# Multi-Cloud_Comparison

Here you go with a quick revision guide for Multi-Cloud Studies.
P.S -- I am updating it as much as possible. Do let me know if you come across any errors or wanna add an update.


|AWS|GCP|Azure|
|-|-|-|
|EC2|Virtual machine instances|Azure Virtual Machines|
|S3|Google Cloud Storage|Azure Blob storage Continers|
|AWS S3 - Infrequent Access ||Azure Cool Blob Storage tier|
|AWS Glacier||Azure Archive Blob Storage|
|EC2|GCE --Google Compute Engine|
|ECS||Azure Container Instances|
|User-Data in EC2|Startup Scripts|Extensions or Cloud-init|
|ASG|Managed Instance Group|Azure Virtual Machine Scale Sets|
|Launch Configuration|Instance Template|
|AZ|Zones|7 Georaphies, each has atlest 1 Region, each region has min 3 AZ, each AZ has min 1 DC|
|ap-south-1|asia-south1 , Delhi WIP|3 regions West India (Mumbai) Central India (Pune) South India (Chennai)|
|ap-south-1 a,b,c|asia-south1 -a,-b,-c|
|VPC|VPC|VNET|
|VPC is AWS Region(In AWS Region means a geography)|VPC is Global|VNET is Region Specific(In Azure Region means a location in a Geography)|
|security groups|firewall rules in vpc| |
|SGs can be used in Inbound/outbound rule definitions.|GCP recommends using SAs for the same.||
|Public IP /NAT etc is needed for Outbound Internet.||Default all Services have outbound Internet connectivity.|
|EBS|Persistent Disk or PD|Data Disks in blob|
|Policies|Permissions|
|st1 and sc1 -- HDD |standard PD -- HDD|
|AWS Lightsail||Azure DevTest Labs||
|EC2 -- Only key|Only Key|VMs -- username and password and keys|
|ec2-user||azureuser|
|Public IP setting is VPC based, VM will get if in that VPC||Public IP is per VM|
|5 IPs are reserved per subnet(1st 4 and last 1)|4 IPs are reserved per primary subnet|5 IP addresses are reserved each subnet|
|CIDR cannot be extended, secondary can be added|for Custom, Subnet CIDR can be extended, for auto no|
|Allowed block min /28 to max /16|Min /29 max /9|/29 to /8|
|Elastic Beanstalk or Heroku|GAE|Azure App Service|
|Spot Instances |preemptible| Azure Spot VMs|
|2 Min Notice||30 Seconds Notice||
|AWS OpsWork||Azure Automation State Configuration|
|Placement groups || proximity placement group|
|Lambda|Cloud Functions|Azure Functions|
|Instance Store|Local SSD|Azure Temporary Disks|
|EFS (only for posix, cannot be mounted over internet witout direct-connect etc)|Cloud File Store|Azure Storage -- > Azure Files (for windows, linux and macos.They can be mounted on-prem over internet.)|
|Storage Gateway||StorSimple||
|Storage Gateway -- File Gateway||Azure File Sync|
|Data Sync||File Sync||
|AWS Image makes one each||Azure Capture/ Make Image make one IMG for all VHDs.|
|AWS Trusted Advisor ||Azure Security Advisor|
|Eventual consistency for Objects in S3|Strong Consistency|
|AWS RDS|Cloud SQL No MariaDB, No Oracle|
|Redhshift -Coloumnar and Athena |Bigquery -Coloumnar and serverless|
|DynamoDB, Cassandra, HBASE|BigTable -- NoSQL|
|Dynamo DB|Cloud Datastore|Azure Table storage, Azure Cosmos DB|
||firebase and |
|SnowCone, Snowball,Snowball Edge, Snow mobile|~~Data~~ Google Transfer Appliance|DataBox (DataBox Disk, Databox and Databox Heavy)|
|||Online Data Box (Databox Edge and Databox Gateway)|
||Storage Transfer Service||
|Route53 -- Registrar|Google Domains  -- Registrar -Supports DNSSEC|
|Route53|CloudDNS|Azure DNS|
|Elastic IP|Static IP|
|ELB(Elastic Load Balancing)|CLB(Cloud Load Balancing)|Azure Load Balancer|
|CloudFront, Akamai|CloudCDN|Azure Content Delivery Network|
|Direct Connect|Dedicated Interconnect| Azure ExpressRoute
|AWS VPN|Cloud VPN|
||Cloud InterConnect|
||Cloud Router|
||CDN Interconnect|
|AWS Sagemaker|Cloud ML engine (Tesnorflow, MXnet)|
|AWS REkognition|Cloud Vision API|
|Polly and Transcribe|Cloud Speech API|
|AWS Comprehend|Cloud Natural Language API|
|AWS Translate|Cloud Transalte API|
|AWS Lex|DialogFlow|
|AWS Rekognition|Cloud Video Intelligence API|
|AWS IoT|Cloud IoT Core|
|AWS SNS,SQS,Kinesis|Cloud Pub/Sub|Azure Queue storage|Event Grid, Notification Hub|
|AWS Glue -- ETL|DataPrep -- Does more of cleaning of data|
|AWS EMR |Cloud Dataproc|Azure Databricks|
|More Like EMR |Cloud DataFlow|
|jupyter|Cloud Datalab|
|AWS Quicksight or Tableau|Cloud Data Studio|
|AWS IAM |Cloud IAM||
|AWS Cognito User Pools||Azure AD B2C|
|AWS Cognito Idenity pools||Azure AD B2B|
|IAM Roles|Service Accounts|
|AWS Organisation|||
|Cloud Trail|Cloud Audit Logging|
|Shiled and WAF|CLoud Armor|Azure DDoS Protection|
|Similar to Macie|Cloud DLP API|
|AWS GuardDuty|Event Threat Detection|
|subnets are zonal|subnets are regional|
|AWS Security Hub -- SIEM|Cloud SCC -- SIEM|
|AWS KMS|Cloud KMS|Azure Key Vault|
|AWS HSM|CloudHSM|
|Cloudwatch|StackDriver|
|AWS XRay|Stackdriver Trace|Azure Application Insights (APM)
|CloudFormation|Deployment Manager| Azure Resource Manager Templates|
|AWS Code Commit /Git|Cloud Sorce Repos|
|AWS CodeBuild|Cloud Build -- Jenkins|
|AWS ECR |Container Registery|Container Registery|
|ALB||Azure Application Gateway|
|Somehwhat like API Gateway|Cloud Endpoints||
|AWS Device Farm|Test lab for Android|
|AWS Cloud9|CloudShell (Sudo yes)| Azure Cloud Shell (No Sudo)|
|AWS Health Dashboard https://status.aws.amazon.com/|GCP Health Dashboard https://status.cloud.google.com/| Azure https://status.azure.com/en-us/status |
|AWS Personal HD| NA|
|AWS https://console.aws.amazon.com/  |GCP https://console.cloud.google.com/|Azure https://portal.azure.com/ |
|EKS|GKE|Azure Kubernetes Service (AKS)|
|Fargate |~ Cloud Run||
|Dedicated Hosts|Sole-tenant nodes|Host Group|
|EC2 Bare Metal Instances |Bare Metal Solution|
|ElasticCache |Cloud Memorystore|Azure Cache for Redis|
|Amazon DocumentDB |Cloud Firestore|
|AWS AppMesh|Traffic Director|Service Fabric Mesh |
|Dual Stack VPC | IPv4 Only VPC|Dual Stack VNET|
|Dual Stack ELB|No Dual Stack CLB (Create 2 separate LBs)|Dual Stack LBs|
|Path Based Switching|URL Maps||
|Amazon CloudWatch alarms|Cloud Monitoring they are called alerting policies||
|Cloud Watch|Cloud Monitoring|Azure Monitor (Insights and Log anlytics)|
|https://calculator.aws/|https://cloud.google.com/products/calculator/ |https://azure.microsoft.com/en-us/pricing/calculator/|
|||https://azure.microsoft.com/en-us/pricing/tco/|
|Support Plans Basic,Developer($29),Enterprise($15,000) and Business($100) |Basic, Developer, Production and Premium Support |Free,Developer($29),Standard($100), professional Direct($1000)
| | |
| | |
| | |
