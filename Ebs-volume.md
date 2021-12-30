*   An Ec2 machine's root volume is lost when it's manually terminated.
*   Unexpected termination can occur at any time in the aws email you receive.
*   We sometimes need to store instance data somewhere.
*   An EBS (Elastic Block Store) volume is a network drive you can attach while your instance is running.
*   It allows your instance data to persist.
*   It's a network drive, not a physical drive.
*   It detached from one EC2 instance and attached to another instance very quickly.
*   It's locked to the availability zone volume, so us-east-1a can't attach to another region, us-east-1b.
*   To move the volume across, we first take a snapshot.
*   A snapshot can be used to backup an Ebs volume.  
*   snapshot take backup used space size 
