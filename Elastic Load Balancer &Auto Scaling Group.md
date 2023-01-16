Why use a load balancer?
• Spread load across multiple downstream instances 
• Expose a single point of access (DNS) to your application
• Seamlessly handle failures of downstream instances 
• Do regular health checks to your instances 
• Provide SSL termination (HTTPS) for your websites
• High availability across zones

What’s an Auto Scaling Group?
• The goal of an Auto Scaling Group (ASG) is to:
• Scale out (add EC2 instances) to match an increased load
• Scale in (remove EC2 instances) to match a decreased load
• Ensure we have a minimum and a maximum number of machines running
• Automatically register new instances to a load balancer
• Replace unhealthy instances
