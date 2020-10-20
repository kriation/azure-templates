# Virtual Machine Contributor (with sshPublicKeys)
This template creates a custom role in a subscription with privileges as defined in the [Virtual Machine Contributor](https://docs.microsoft.com/en-us/azure/role-based-access-control/built-in-roles#virtual-machine-contributor)
built-in role and specific permissions to generate, read, and write SSH keys for use by a VM. I discovered the need for
this role by the observations made in [this](https://blog.kriation.com/2020/ssh-key-management-in-azure.html) blog post.