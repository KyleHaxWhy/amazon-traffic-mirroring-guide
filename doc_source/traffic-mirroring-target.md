# Traffic Mirror Targets<a name="traffic-mirroring-target"></a>

A target is the destination for a Traffic Mirror session\.

The Traffic Mirror target can be an elastic network interface, or a Network Load Balancer\. After you create a target, assign it to a Traffic Mirror session\. For more information, see [Create a Traffic Mirror Session](traffic-mirroring-session.md#create-traffic-mirroring-session)\.

You must configure a security group for the Traffic Mirror target that allows VXLAN traffic from the source to the target\.

You can share a Traffic Mirror target across accounts\. To share a Traffic Mirror target, create the target, and then share the target\. For more information, see [Sharing a Traffic Mirror Target](cross-account-traffic-mirroring-targets.md#tm-sharing)\.

## Create a Traffic Mirror Target<a name="create-traffic-mirroring-target"></a>

Create a Traffic Mirror target\.

**To create a Traffic Mirror target using the console**

1. Open the Amazon VPC console at [https://console\.aws\.amazon\.com/vpc/](https://console.aws.amazon.com/vpc/)\.

1. In the **Region** selector, choose the AWS Region that you used when you created the VPCs\.

1. On the navigation pane, choose **Traffic Mirroring**, **Mirror Targets**\.

1. Choose **Create Traffic Mirror Target**\.

1. For **Name tag**, enter a name for the Traffic Mirror target\.

1. \(Optional\) For **Description**, enter a description for the Traffic Mirror target\.

1. For **Target type**, choose the Traffic Mirror target type\.

1. For **Target**, choose the Traffic Mirror target\.

1. \(Optional\) Add or remove a tag\.

   \[Add a tag\] Choose **Add tag** and do the following:
   + For **Key**, enter the key name\.
   + For **Value**, enter the key value\.

   \[Remove a tag\] Next to the tag, choose **Remove tag**\.

1. Choose **Create**\.

**To create a Traffic Mirror target using the AWS CLI**  
Use the [create\-traffic\-mirror\-target](https://docs.aws.amazon.com/cli/latest/reference/ec2/create-traffic-mirror-target.html) command\.

## Modify Traffic Mirror Target Tags<a name="modify-traffic-mirroring-targets"></a>

Add a tag to the Traffic Mirror target, or remove a tag from the Traffic Mirror target\.

**To modify your Traffic Mirror targets using the console**

1. Open the Amazon VPC console at [https://console\.aws\.amazon\.com/vpc/](https://console.aws.amazon.com/vpc/)\.

1. In the **Region** selector, choose the AWS Region that you used when you created the Traffic Mirror target\.

1. On the navigation pane, choose **Traffic Mirroring**, **Mirror Targets**\.

1. Select the Traffic Mirror target\.

1. Choose **Tags**, **Manage tags**\.

1. Add or remove a tag\.

   \[Add a tag\] Choose **Add tag**, and then do the following:
   + For **Key**, enter the key name\.
   + For **Value**, enter the key value\.

   \[Remove a tag\] Next to the tag, choose **Remove tag**\.

1. Choose **Save changes**\.

## View Traffic Mirror Target Details<a name="view-traffic-mirroring-targets"></a>

View the Traffic Mirror target details\.

**To view your Traffic Mirror targets using the console**

1. Open the Amazon VPC console at [https://console\.aws\.amazon\.com/vpc/](https://console.aws.amazon.com/vpc/)\.

1. In the **Region** selector, choose the AWS Region that you used when you created the Traffic Mirror target

1. On the navigation pane, choose **Traffic Mirroring**, **Mirror Targets**\.

1. Select the Traffic Mirror target\.

**To view your Traffic Mirror targets using the AWS CLI**  
Use the [describe\-traffic\-mirror\-targets](https://docs.aws.amazon.com/cli/latest/reference/ec2/describe-traffic-mirror-targets.html) command\.

## Delete a Traffic Mirror Target<a name="delete-traffic-mirroring-target"></a>

Before you delete a Traffic Mirror target, pause all Traffic Mirror sessions that use the Traffic Mirror target\.

**To delete your Traffic Mirror target using the console**

1. Open the Amazon VPC console at [https://console\.aws\.amazon\.com/vpc/](https://console.aws.amazon.com/vpc/)\.

1. In the **Region** selector, choose the AWS Region that you used when you created the Traffic Mirror target\.

1. On the navigation pane, choose **Traffic Mirroring**, **Mirror Targets**\.

1. Select the Traffic Mirror target\.

1. Choose **Delete**\.

1. In the **Delete confirmation** dialog box, enter **delete**, and then choose **Delete**\.

**To delete a Traffic Mirror target using the AWS CLI**  
Use the [delete\-traffic\-mirror\-target](https://docs.aws.amazon.com/cli/latest/reference/ec2/delete-traffic-mirror-target.html) command\.