AWS Cloud Practitioner Essentials

-----------------13--------------
terraform workspace select * "jabejaie beine work space ha"
terraform workspace new * "sakhte worspace jadid"
terraform workspace list
WORCKSPACE
terraform 'work space name' init
${aws_instance.webserver.public_ip} "Ip automatic jaygozin mikone"
provisioner "remote-exec"
provisioner "local-exec"
Terraform provisioner "mesle Ansible amal mikone"
terraform refresh "*.tfstate update mikone"
terraform providers "list provider ha neshun mide"
terraform fmt "file haye terraform neshun mide"
terraform apply -refresh=false "*.tfstate update nemishe"
sakhte alias
terraform show "check kardan vaziat provider"
terraform validate "check mikone daturat dorost bashe"
terraform destroy "dastore rollback"
file terraform.tfstate "kholase vaziate provider"
terraform apply -auto-approve "automatic YES mizane"
mkdir terraform_test1
cd terraform_test1/
main.tf
terraform init "scan mikone, provider haye nasb nashode nasb mikone"
terraform plan "dry-run, check kardan khoruji file"
terraform apply
terraform - install-autocomple "completion faal mishe"
terraform providers "AWS, Azure, GoogleCloudPlatform, Kubernetes, Alibaba Cloud, ..."
zabane terraform HCL
Immutable VS Mutable "tafavotesh ine Immutable config taghir nemide, pak mikone dobare misaze"
Terraform -> plan -> apply <- (destroy)
-----------------12--------------
Plan (dry-run) -> Apply (run)
Terraform files
terraform.state "cached configuration"
terraform.tfvars "variables"
main.tf
Google Workspace
Immutable "rollback, az aval ba kole mohit jadid jay gozin mishe ba taghirat jadid"
Terraform (Destroy/Push Masterless/Agentless) "Provisioning, Cloud usage"
Mutable "taghirat mostaghim emal mishe, "
Ansible "config manager, OS usage"
cloud-init
terraform cloud
SALTSTACK
YAML
Infrastructure as Code (laC) "Config M anager"
Imperative Way "The How"
Declarative Way "The What"
puppet
Agentbased
Servicebased
SSL
Freeze Configuration
ANSIBLE
Agentless
serviceless
YAML
Ingress "Inbound, Outbound"
AWS Egress "Outbound" only IPv6
AWS Well-Architected "Free tool to review architectures"
data source Grafana -> X-ray -> CloudWatch
AWS Grafana
-----------------11--------------
EC2 Image Builder
Storage Gateway
Amazon Textract "OCR"
Amazon Personalize "personalized recommendations"
Amazon Kendra "document search service"
Amazon Forecast "forecast Product Demand Planning, Financial Planning, Resource Planning"
Amazon SageMaker "AI, build ML models"
Amazon Comprehend "Natural Language Processing - NLP"
Amazon Connect
Amazon Lex "Alexa"
Amazon Translate
Amazon Polly "text to speech"
Amazon Transcribe "speech to text"
Amazon Rekognition "images and videos analyzer"
Root User Privileges
CIS Foundations Benchmark "check kardan amniat"
nessus
Security Check
AWS Security Hub
AWS Config "auditing, log config ha zade shode"
AWS Certificate Manager (ACM)
AWS KMS (Key Management Service)
Symmetric "Single Key"
Asymmetric "Public & private key"
Penetration Testing on AWS Cloud
AWS Firewall
K6 "Load Tester"
DDOS Protection
AWS Shield "Layer 4 is TCP"
AWS WAF "Layer 7 is HTTP, Deploy on Application Load Balancer, API Gateway, CloudFront"
CloudFront and Route 53
CloudFlare WAF "Web Application Firewall" iejad rule mahdudiat baraye user haye website
CloudFlare DDOS
-----------------10--------------
Health Dashboard "Health Dashboard AWS services"
CodeGuru "Code reviewer"
Improve application code security, quality, and performance with ML
X-Ray "Tracer, Debugger log"
CloudTrail "dashboard of CloudWatch logs"
EventBridge
CloudWatch Alarms actions
Auto Scaling
EC2 Actions: stop, terminate, reboot or recover an EC2 instance
SNS notifications
CloudWatch
Amazon MQ
SNS "Simple Notification Service"
apache flink
Kinesis "Collect, process, and analyze data streams in real time"
1.Kinesis Data Streams "Collect and store data"
2.Kinesis Data Firehose "Process and deliver data"
3.Managed Apache Flink "Process and analyze"
Defaut retention "modat zamani ke mitune safo negah dare"
Amazon SQS "Simple Queue Service, serverless, shabihe KAFKA"
from 1 message per second to 10,000 per second
retention: 4 days, maximum of 14 days
Apache Kafka, RabbitMQ "messaging queue"
EC2 Architecture
WaveLength
Smart Cities, ML-assisted diagnostics, Connected Vehicles, Interactive Live Video Streams, AR/VR, Real-time, Gaming
Outposts
Global Content Delivery Network (CDN): CloudFront
Enable Origin Shield "ezafe kardan region"
Route 53 "DNS server, Domain registration, Health checks"
top-level domain (TLD)
second-level domain (SLD)
*ECS "SWARM, Best Practice"
*CodeDeploy, CodePipeline "Best Practice"
GitHub "Best Practice build"
-----------------9--------------
OpsWorks "IAC, server configuration automatically" ba SSH ya SSM
agent ohai ru remote ha nasb shavad
base chef ya puppet
cockpit linux "web-based graphical interface for managing servers" Session Manager
Systems Manager (SSM) "ba SSL vasl mishe be server"
Cloud9 "cloud IDE, mese gitlab CE"
CodeStar "discontinued"
CodeArtifact
CodeBuild "build mikone natije PUSH mikone"
CodePipeline "Build va Deploy"
CodeArtifact "moadele ECR"
CodeCommit "repo"
Beanstalk "Select Wizard Services"
1.Environment
2.Application
LAMP "Linux, Apache, MySQL, PHP/Perl/Python"
LightSail
CloudFormation
AWS Batch "Script runner"
API Gateway
EventBridge "create, run, and manage tasks, Cron job"
-----------------8--------------
AWS Batch "Auto script cron"
API Gateway "serverless API"
AWS EventBridge "Customization"VS CloudWatch events "use template"
Throttle "modiriate request ha"
Destination configuration "daryaft notification"
EventBridge "" serverless
Trigger "che zamani code run beshe"
Lambda:
Application "majmue chandin function, CI/CD pipeline"
Function
Enable function URL "URL to assign project"
Enable Code signing "code open source nist"
blueprint "sample"
Serverless Services:
Amazon S3
DynamoDB
199
Fargate
Lambda
Lambda "Compile/Build/Deploy"
FaaS (Function as a Service)
Auto Scaling
no servers to manage
App-> Cannot Containerize
Upload .zip Code ya Copy Paste Code ya S3
run task OR deploy task (deployment to more option)
Task definitions "container build"
ECS application type service: majmue task ha
CDK (Cloud Development Kit) "code is "compiled" into a CloudFormation template (JSON/YAML)"
Cloud Formation (infrastructure as Code) "automation"
ghabeliate rollback
.yaml .json
auto schedule
ECS (Elastic Container Service) "docker swarm" best practice backend
EC2 be onvane worker
Application Load Balancer
Auto Scaling Group
Fargate "Swarm, Docker container" serverless, best practice frontend
ECR (Elastic Container Registry) "Container Repository"
Firewall (VPC) Security Group (EC2)
-----------------7--------------
Bastion Host Creation:
VPC "tenancy ekhtesasi ya eshteraki" Enable DNS hostnames
Public Subnet "Auto Assign IP Address"
Private Subnet
Internet gateway "Attach to VPC"
Public Route tables "auto created, Edit Route Tables, 0.0.0.0/0 -> Internet Gateway"
Assign to VPC
Route Tables > Subnet Association > Edit Subnet Association > Public Subnet
NAT gateway "Public subnet"
Private Route tables "Edit Subnet Association > Private Subnet, 0.0.0.0/0 > NAT Gateway"
Subnet Association > Edit Subnet Association > Private Subnet
EC2 "Public Subnet"
EC2 "Private Subnet"
Direct Connect (DX) "connection between on-premises and AWS, bedune internet"
VPN "Site-to-Site, az internet"
VPC Endpoints service
VPC Endpoints "connect network privately"
peering connection "Connect two VPC, NOT transitive, "
Kinesis Data Firehose
netflow
Security Groups "instance level, allow rules only, allow and deny rules, stateful, "
Network ACL "subnet level, stateless, "
NAT gateway (NGW) "vasl kardan VPC private be VPC public"
Flow log
Internet gateways
Bastion Host "Jump host" 1CPU1RAM
endpoint "beine VPC region haye mokhtalef gharar migire"
subnet "ba subnet AZ moshakhas mishe"
public subnet
private subnet
VPC "per regional"
-----------------6--------------
DMS (Database Migration Service) "tabdile file be database, database to other database"
 Glue (extract, transform, and load) "serverless, report giri, data for analytics" ETL tools
QLDB (Quantum Ledger Database) "Block chain, NFT, finance cases"
Neptune "graph database, NoSQL, heap data, Serverless"
QuickSight "vasl kardan RDS, Auroa, Athena, Redshift, S3 be ham"
BA, Serverless machine learning-powered business intelligence service to create interactive dashboards.
Athena "Serverless, analyze data stored in Amazon S3"
EMR (Elastic MapReduce) "Hadoop clusters (Big Data)"
Redshift (Postgres) "OLAP"
DB
OLTP (transactional processing and real-time)
OLAP (data analysis and reporting) "BI, Big data, Reporting" data warehouses
key/value database (NoSQL)
DocumentDB "MongoDB, modiriate ba admin, NoSQL"
DynamoDB (MongoDB, NoSQL) "serverless, PayG"
ElastiCache (Redis) -> add nodes "ezafe karan secondary baraye replica"
RDS "ta 15 ta replicas"
RDS
OS patching
backups
Monitoring
replicas
Multi AZ (DR), Multi Region(read)
Scaling capability
Storage backed
RDS (Relational DB Service)
Postgres
MySQL
MariaDB
Oracle
Microsoft SQL Server
Aurora (AWS Proprietary database)
TSDB "Monitoring estefade mishe"
Relational Database (RDBMS)
AtlasDB
Couchbase
DBaaS
-----------------5--------------
AWS OpsHub "modiriate dastgahaye Snow family"
AWS Snow Family "etelaate bishtar az 500TB"
Snowcone
Snowmobile
Snowball Edge
aws s3 ls "list s3"
aws configure "command tanzimate avalye"
IAM -> Users -> Security credentials -> Access keys
AWS CLI
batch "schedule job"
S3
* Standard
Intelligent-Tiering
Express One Zone "analytics and ML workloads"
Standard-lA "Standard-Infrequent Access"
One Zone-lA "One Zone-Infrequent Access"
Glacier Instant Retrieval "Glacier Instant Retrieval" arzuntarin
Glacier Flexible Retrieval "Glacier Flexible Retrieval"
Glacier Deep Archive
Outposts
aws.amazon.com/s3/storage-classes/
S3 "block storage"
Bucket
Object
AWS grafana
CloudTrail
SNS "ersal email, SMS, push notification service"
Beanstalk
lightsail "VPS"
Auto scaling "ASG"
system manager "add service haye khareje AWS"
-----------------4--------------
ELB
Application Load Balancer "ALB" HTTP HTTPS
Network Load Balancer "NLB" TLS UDP TCP
Gateway Load Balancer "GWLB"
ELB "Elastic Load Balancer" SaaS "DNS name Public" CNAME record, layer7
Aval Target group sakhte mishe "tarafe instance"
Load Balancer
Agility "sorate bishtare ezafe kardan manabe"
Elasticity "Auto Scaling"
Scalability "scale up or scale out"
HACS
active backup "round robin"
SLB
2N+1
GDR "DR, GDR"
high Availability "chand ta Horizontal Scalability"
*Horizontal Scalability (scale out "afzayesh manabe"/Scale in "kahesh manabe")
Vertical Scalability (Scale up/Scale down)
ELS
Network Interfaces
attach "faghate be 1 EC2"
Associate "be chand EC2"
Key Pair
Placement Group "taste bandi instance ha baraye modiriate behtar"
Cluster
Partition
Spread
Elastic IPs
Security Group
HDD "backup volume" nemishe OS nasb kard /boot
faghat io1 va io2 multi attach
OpenZFS "bara MacOS"
Lustre "ESx, faghat ba linux" high performance, baraye machine learning estefade mishe
FSx "windows file server"
EBS vs EFS
EFS "file system, faghat ba linux, multi AZ, gerun tare" NFS Amazon
EC2
Instance-Store (Amazon machine IMAGE) "sorate bala, data sabet, arzun tare" bayad back up giri beshe
EBS "avalin bar EC2 ba EBS sakhte mishe"
Create image
-----------------3--------------
Attach network interface to Instances
AMI "amazon machine image" Instances-> actions-> Image and templates-> Create image
Public
Your own
AWS Marketplace
Lifecycle Manager "snapshot automatic ba baze zamani"
snapshot "EBS volume backup"
create new volume
copy volume baraye enteghal be yek region digar
Archive snapshot "less cost"
VMware Tanzu
Volume -> modify "extend storage"
df -Th
lsblk "noe virtualization" Xen,Nitro
Volumes
Amazon EC2 Capacity Blocks for ML "machine learning khube"
On-Demand "mah be mah pardakht mishe"
Amazon EC2 Spot Instances "az manabe share estefade mishe"
AI, Data analyst, Machine learning "High GPU"
Jump Host (SSH gateway), "Bastion server"
Security group
IP ye layer balatar set shode, IP public tu server neshun dade nemishe
Instance create
snapshot
AMI (amazon machine images) "backup giri az compute va storage va security group va network"
Elastic IP
Dedicated
Bills
Calculator
Budgets
Free tier status


-----------------2--------------
aws ec2 ls "command list ec2 neshun mide"
aws s3 ls "command list s3 neshun mide"
AWS cloudshell
AWS codecommit
Access key "baraye login be CLI, ..."
Identity provider
Role
AWS CloudFormation
User
User group
User Policy
IAM (Identity & Access Management)
AWS CloudFront (CDN)
Route 53 (DNS manager)
Object Storage
CDN (globally, user ziad, Static Data)
DR (Disaster Recovery)
Live Migration
GDR (Geographical Disaster Recovery)
Region -> Availability zone -> Local Zone
region haye yeksan ba IP local ghabel dast rasan
Service Quotas
skillbuilder.aws
OS system image backup (S3)
EC2 (elastic computing)
Instance
OVS
SR-IOV
-----------------1--------------
AWS calculator
Storage: Object(Virtual) "Ceph , min io" (S3 Amazon), Block(physical) EBS Amazon, File
OpenStack: Under Cloud, Over Cloud
SDN Architecture (Software defined networking)
Opnestack, docker swarm, K8S
NFV Architecture (network function virtualization): tabdile physical(compute, memory, network) be virtual (compute, memory, network)
min io, ESXi, Ceph
DBaaS : Database as service
SaaS(service narmafzar): narmafzar besurate amade erae mishe
PaaS: application va data manage mishe
IaaS(service zirsakht): az laye OS be baed manage mishe
Linode, OVH, Hetzner, DigitalOcean, Azure, AWS, GoogleCloud, IBM Cloud, OracleCloud
Private Cloud (OpenStack, CloudStack), Public Cloud, Hybrid Cloud
ECS (docker amazon) EKS(kuber amazon) AWS Code commit (git)
AWS= keifiate bala, poshtibani khub
Bare-metal (be surate mostaghim ru server nasb mishe)
Live migration (HOT) 5-7 Seconds
Cold migration
Cloud (Instance) 1:1 1:2 1:4
Compute (CPU, RAM)
Storage
Network
Virtualization vs Cloud (OVS - SRSOV)
HACS (round robin, blue green, SLB, DR, GDR)
loud balancing
round robin
clustering (HA)
Active backup
