Streamwave is a rapidly expanding broadcasting company that receives satelite contribution feeds from International clients. As part of a cloud migration initiative, a requirement exists to ingest live media streams into AWS while isolating public facing ingest endpoints from Internal processing infrastructure
I am tasked with designing a VPC that mirrors this segmentation - a public subnet exposing ingest endpoints via an Internet Gateway & a private subnet hosting processing resources

This project demostrates the design & deployment of a secure & scalable AWS Virtual Private Cloud suitable for a multi-tier application
It follows AWS best practiced and includes public/private subnets, routing, NAT & Bastion Access.
