## Packer tutorial  

[docker](https://learn.hashicorp.com/collections/packer/docker-get-started)

[aws](https://learn.hashicorp.com/collections/packer/aws-get-started)


Main commands  
`packer init .`  
`packer build aws-ubuntu.pkr.hcl`  

```
jason@DEV-52WP6M3:~/Documents/packer_tutorial$ packer build aws-ubuntu.pkr.hcl
learn-packer.amazon-ebs.ubuntu: output will be in this color.

==> learn-packer.amazon-ebs.ubuntu: Prevalidating any provided VPC information
==> learn-packer.amazon-ebs.ubuntu: Prevalidating AMI Name: learn-packer-linux-aws-redis
    learn-packer.amazon-ebs.ubuntu: Found Image ID: ami-0b0ea68c435eb488d
==> learn-packer.amazon-ebs.ubuntu: Creating temporary keypair: packer_6304ab8d-d0e5-73eb-f88f-8acbafb9ff5f
==> learn-packer.amazon-ebs.ubuntu: Creating temporary security group for this instance: packer_6304ab93-4679-298a-a6db-e274d0c5339a
==> learn-packer.amazon-ebs.ubuntu: Authorizing access to port 22 from [0.0.0.0/0] in the temporary security groups...
==> learn-packer.amazon-ebs.ubuntu: Launching a source AWS instance...

...
...

...
...

==> learn-packer.amazon-ebs.ubuntu: Waiting for AMI to become ready...
==> learn-packer.amazon-ebs.ubuntu: Skipping Enable AMI deprecation...
==> learn-packer.amazon-ebs.ubuntu: Terminating the source AWS instance...
==> learn-packer.amazon-ebs.ubuntu: Cleaning up any extra volumes...
==> learn-packer.amazon-ebs.ubuntu: No volumes to clean up, skipping
==> learn-packer.amazon-ebs.ubuntu: Deleting temporary security group...
==> learn-packer.amazon-ebs.ubuntu: Deleting temporary keypair...
Build 'learn-packer.amazon-ebs.ubuntu' finished after 4 minutes 27 seconds.

==> Wait completed after 4 minutes 27 seconds

==> Builds finished. The artifacts of successful builds are:
--> learn-packer.amazon-ebs.ubuntu: AMIs were created:
us-east-1: ami-0f207bec2307f4cfa
```