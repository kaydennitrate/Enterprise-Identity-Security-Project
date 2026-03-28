# Lab 4: OS Hardening and Network Perimeter Security

## 4.1 Security Objective
To apply defense-in-depth principles by hardening the local Operating System (OS) and the physical network gateway. This prevents unauthorized horizontal movement and limits the attack surface available to external threats.

## 4.2 Technical Procedure
- Linux System Hardening (Directory ACLs):
Accessed the Azure Cloud Shell (Bash environment).
Executed mkdir /finance_audit_vault to create a secure data repository.
Applied chmod 700 /finance_audit_vault to restrict all Read, Write, and Execute permissions exclusively to the root owner.
Verified permissions using ls -ld, ensuring the output reflected drwx------.

- Network Perimeter Security (Gateway Configuration):
Authenticated to the Huawei ONT administrative interface.
MAC Whitelisting: Enabled hardware-address filtering to restrict network access to authorized device IDs only.
SSID Obfuscation: Disabled SSID broadcasting to hide the network from wireless reconnaissance tools.

## 4.3 Evidence
- Outcome:
System-level ACLs enforced; network visibility eliminated to increase the security posture of the environment.
