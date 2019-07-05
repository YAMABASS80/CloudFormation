# Security Group Stack

This template creates simple security group on top of the VPC that has created in `../network/network.yaml`.

Note that, youd dont have to specify VPC ID in this template with using,

```
      VpcId:
        Fn::ImportValue: !Sub ${VpcName}-VpcId
```

This code means, import VPC ID that the network stack has already created.
