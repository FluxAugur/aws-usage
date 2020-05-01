# AWS Created Role

## Required Roles

### **AmazonAppStreamServiceAccess**  

##### *arn:aws:iam::fluxaugur:role/AmazonAppStreamServiceAccess*

> Creator requires
>
> - **AdministratorAccess**
> *arn:aws:iam::aws:policy/AdministratorAccess*
>
> or
>
> - *iam:CreateRole*
> - *iam:AttachRolePolicy*
>
> ---
> Attach policy
>
> - **AmazonAppStreamFullAccess**
>   *arn:aws:iam::aws:policy/service-role/AmazonAppStreamServiceAccess*

### *ApplicationAutoScalingForAmazonAppStreamAccess*

##### *arn:aws:iam::aws:role/service-role/ApplicationAutoScalingForAmazonAppStreamAccess*

> Creator requires
>
> - **AdministratorAccess**
> *arn:aws:iam::aws:policy/AdministratorAccess*
>
> or
>
> - *iam:CreateRole*
> - *iam:AttachRolePolicy*
>
> ---
> Attach policy
>
> - **AmazonAppStreamFullAccess**
> *arn:aws:iam::aws:policy/service-role/ApplicationAutoScalingForAmazonAppStreamAccess*

### **AWSServiceRoleForApplicationAutoScaling_AppStreamFleet**

##### *arn:aws:iam::fluxaugur:role/aws-service-role/AWSServiceRoleForApplicationAutoScaling_AppStreamFleet*

> Creator Requires
>
> - **AdministratorAccess** arn:aws:iam::aws:policy/AdministratorAccess
>
> or
>
> - *iam:CreateRole*
> - *iam:AttachRolePolicy*
> - *iam:CreateServiceLinkedRole*
>
> ---
>
> Attach policy
>
> - **AWSApplicationAutoscalingAppStreamFleetPolicy**
> *arn:aws:iam::aws:policy/aws-service-role/AWSApplicationAutoscalingAppStreamFleetPolicy*
>
> ---
>
> Inline trust relationship
>
> - **AWSApplicationAutoscalingAppStreamFleetPolicy** (file)
>
> > {  
> > > "Version": "2012-10-17",  
> > > "Statement": [  
> > > {  
> > > > "Effect": "Allow",  
> > > > "Principal": {  
> > > > > "Service": "appstream.application-autoscaling.amazonaws.com"  
> > > > },  
> > > > "Action": "sts:AssumeRole"  
>
> > > > }  
>
> > > ]  
>
> > }  
