# Downloads and install Terraform

- https://www.terraform.io/downloads
- Install terrafrom ( i use win 10, litle problem)
- open powershell try Command " terrafrom "
- it is can't work
-  make c:/Terraform dir. Terraform.exe copy here to 
- click start menu and runing field type environment variables
- here select environment varaibles
- system variables add to new line " C:\Terrafrom
- reopen Power Shell and type again terrafrom is working

# Install AWS Cli

- https://aws.amazon.com/cli/
- Install it
- open Power Shell, type " Aws ". it's working

# Setup AWS user and Grp

- Login AWS
- start IAM Control
- Add terraform user and group
- Terraform Grp permissions: 
- AmazonRDSFullAccess
- AmazonEC2FullAccess
- IAmFullAccess
- AmazonS3FullAccess
- AmazonDynamoDBFullAccess
- AmazonRoute53FullAccess
- Terrafrom user: 
- create non-root AWS user
- Add the necessary IAM roles (e.g. AmazonEC2FullAccess)
- Save Access key + secret key (or use AWS CLI `aws configure` -- https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html)


# Setup security connect

- open power shell

        aws configure

- In AWS terraform_urer Security credentials Access key " Creating new Acces Key " Copy 
AccesKey and SecretKey.
- Region: [eu-central-1]
- output format: [json]

           cd  ~/.aws
           dir

- cheking credentials
- Next step jump on 02 folder, reamdy