# Launch instance in Public 1A
aws ec2 run-instances --image-id ami-06e46074ae430fba6 --instance-type t2.micro --security-group-ids sg-07332a20b70d9557e --subnet-id subnet-0344672a3eae72d07 --key-name AWS-SA-C03 --user-data user-data-subnet-id.txt


# Launch instance in Public 1B
aws ec2 run-instances --image-id ami-06e46074ae430fba6 --instance-type t2.micro --security-group-ids sg-07332a20b70d9557e --subnet-id subnet-0b14db7c91735b0d4 --key-name AWS-SA-C03 --user-data user-data-subnet-id.txt



# Launch instance in Private 1B
aws ec2 run-instances --image-id ami-06e46074ae430fba6 --instance-type t2.micro --security-group-ids sg-07332a20b70d9557e --subnet-id subnet-09bca810e5c18181f --key-name AWS-SA-C03 --user-data user-data-subnet-id.txt


# Terminate instances

aws ec2 terminate-instances --instance-ids i-0bff7cc281d63c5c8

aws ec2 stop-instances --instance-ids i-0a621e54a1c80a341 i-0bff7cc281d63c5c8 i-07913dd2ea216d0fa