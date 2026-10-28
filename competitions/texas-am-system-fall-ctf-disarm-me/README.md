# Texas A&M System Fall CTF — Disarm Me

**3rd place team finish · Fall 2026 · Dhruv Guda**

My team placed third in the Texas A&M System Fall CTF — Disarm Me. This showcase documents my technical work from the competition, from initial network enumeration to an internal SSH pivot and VPN credential recovery.

## **[Competition Report](competitions/texas-am-system-fall-ctf-disarm-me/Texas_A_M_System_Fall_CTF___Disarm_Me___ReadMe.pdf)** 

## What this work demonstrates

- **Reconnaissance:** Used Nmap and DNS queries to identify exposed services and an outlying domain name.
- **Windows access:** Checked MS17-010 and verified a SYSTEM-level Meterpreter session on the competition file server.
- **Host investigation:** Inspected processes and extracted the requested account-hash evidence.
- **Credential recovery:** Used John the Ripper to recover a password from the collected hashes.
- **Internal-network access:** Corrected a pivot route, located an SSH host, and used recovered credentials to access it.
- **Technical documentation:** Recorded the challenge prompts, commands, selected output, and reasoning behind each step.

## Challenges documented

| Challenge | Work documented |
| --- | --- |
| Name_Drop | DNS enumeration and identification of the outlying FQDN |
| Ground_Truth | Windows SMB vulnerability check, host access, and session verification |
| Process_Oriented | Process inspection and executable identification |
| Hash_Brown | Local account-hash recovery and suffix extraction |
| Internal_Focus | Internal subnet discovery and SSH port scanning |
| Easy_Enigma | Offline password cracking and verification |
| VPN Credentials | Route correction, SSH access, and credential-file recovery |

## Result and scope

The **third-place result belongs to the team**; the report presents my recorded challenge work. Cat_Code remains an unfinished lead and is not counted among the documented findings. The DNS loop is labeled as reconstructed where the original notes had damaged formatting.

This work took place in a competition lab. The report distinguishes observed evidence from interpretation and keeps incomplete steps explicit.

[All competitions](../README.md) · [Back to portfolio](../../README.md)
