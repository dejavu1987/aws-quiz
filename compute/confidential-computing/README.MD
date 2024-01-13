## AWS Nitro System and Nitro Enclaves
The networking, monitoring, and storage functions in the AWS Nitro System are abstracted into which component?

- [ ] Nitro chip
- [x] Nitro card
- [ ] Motherboard
- [ ] Nitro hypervisor

#### Explanation

The networking and IO functions, monitoring, security management, and storage are abstracted away into separate Nitro cards. The Nitro security chip, integrated into the motherboard, protects all hardware resources and isolates VMs.

## Which is a key feature of AWS Nitro Enclaves?

- [ ] Fast external network connectivity
- [ ] Multiple secure local channels between the AWS Nitro Enclave and the Amazon EC2 instance
- [ ] Only root user access
- [x] No persistent storage

#### Explanation

AWS Nitro enclaves provide an additional isolation where customers can isolate themselves from their highly sensitive code. These are hardened isolated machines, so there's no network, external network connectivity, there is no persistent storage, there's no interactive or root user access. There's only one secure local channel between the enclave that got spun up and the Amazon EC2 instance from which it got spun up.

## Confidential computing is the use of specialized hardware and associated firmware to protect what kind of data?

- [ ] Data before use
- [x] Data in use
- [ ] Data after use
- [ ] Data in store

#### Explanation

Confidential computing capabilities protect data while it is being processed and in use.
