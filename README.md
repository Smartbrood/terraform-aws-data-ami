terraform-aws-data-ami
======================

Terraform module to get Ubuntu, Centos, AWS ECS optimized AMI IDs for working region

Distribution names currently supported: ecs, centos7, ubuntu1604, ubuntu1204.


Usage
-----

```hcl
module "ubuntu1604" {
    source = "Smartbrood/data-ami/aws"
    distribution = "ubuntu1604"
}


output "ubuntu1604_ami_id" {
  value       = "${module.ubuntu1604.ami_id}"
}
```


Authors
-------

Module managed by [Smartbrood LLC](https://github.com/Smartbrood).


License
-------

Apache 2 Licensed. See LICENSE for full details.
