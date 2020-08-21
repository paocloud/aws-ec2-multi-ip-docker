### AWS EC2 Multi IP with Docker Source NAT.


ตั้งค่า AWS EC2 เพื่อให้สามารถใช้ IP Address ได้มากกว่า 1 เลข
และตั้งค่า Docker เพื่อกำหนดให้ Container ใช้ Public IP ในการออกเน็ตตามต้องการ

#### Idea
- AWS EC2 สามารถกำหนด IP Address ได้มากกว่า 1 เลขในเเต่ละ Interface
- Docker สามารถสร้าง Bridge Interface เพิ่มได้
- สามารถปรับเเต่ง iptables ของ Docker ได้ เพื่อให้ bridge เเต่ละตัวออกเน็ตคนละ IP กัน

#### Reference
- https://aws.amazon.com/premiumsupport/knowledge-center/ec2-ubuntu-secondary-network-interface/
- https://medium.com/@havloujian.joachim/advanced-docker-networking-outgoing-ip-921fc3090b09
- https://sysadmin.psu.ac.th/2018/11/26/ubuntu-server-18-04-config-static-ip-with-netplan/
- https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-eni.html
