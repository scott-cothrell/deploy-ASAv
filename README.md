# Notes


For both of the scripts, below, you have the option of deploying with 4 interfaces (with a DMZ) or with 3 interfaces (no DMZ).

Note the restrictions on the use of M4 instance types.

Note the Security Groups.
The management interface will, by default, be world accessible. The Security Group assigned will permit only
SSH, HTTPS, and all ICMP traffic.  You should consider changing the default value of 'MgmtExternalAccessCidr' to your private CIDR block.

CiscoASA-Build-customer - This script will deploy an ASAv after building the AWS VPC infrastructure (VPC,Subnets,Gateways,etc).

CiscoASA-customer - This script will allow you to use your own, existing infrastructure to deploy the ASAv.

  