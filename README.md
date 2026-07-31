# Cybersecurity Reports

**English** · [Español](README.es.md) · [Italiano](README.it.md)

A collection of technical reports on labs, machines and CTF challenges I have solved.

Each report is a standalone PDF covering the objective, the environment, the attack phases with
supporting evidence, and closing technical and defensive conclusions. The style is deliberately
narrative rather than a list of commands: the goal is to explain **why** a technique works, not
just to show that it does.

---

## Available reports

| Report | Context | Category | Key techniques | Read |
|---|---|---|---|---|
| The Emptiness Machine | HTB Cyber Apocalypse 2026 | Binary Exploitation | FSOP, House of Apple 2, partial overwrite, libc leak | [EN](English/The-Emptiness-Machine-HTB-2026-EN.pdf) · [ES](Espa%C3%B1ol/The-Emptiness-Machine-HTB-2026-ES.pdf) · [IT](Italiano/The-Emptiness-Machine-HTB-2026-IT.pdf) |
| False Ferry | HTB Cyber Apocalypse 2026 | Cloud Security | AWS IAM enumeration, STS AssumeRole, S3 object versioning | [EN](English/False-Ferry-HTB-2026-EN.pdf) · [ES](Espa%C3%B1ol/False-Ferry-HTB-2026-ES.pdf) · [IT](Italiano/False-Ferry-HTB-2026-IT.pdf) |
| Fireflow | HTB (Medium, Linux) | Web / RCE / Kubernetes | Subdomain enumeration, unauthenticated RCE (CVE-2026-33017, Langflow), credential reuse, JWT alg=none forgery, kubelet exec via nodes/proxy | [EN](English/Fireflow-HTB-2026-EN.pdf) · [ES](Espa%C3%B1ol/Fireflow-HTB-2026-ES.pdf) · [IT](Italiano/Fireflow-HTB-2026-IT.pdf) |

---

## Skills covered

**Binary exploitation**: static analysis with objdump and nm, function reversing, exploitation of
internal glibc structures, mitigation bypass (Full RELRO, PIE, NX), GDB debugging with breakpoints
and hardware watchpoints, exploit automation in Python with pwntools.

**Cloud security**: AWS enumeration with the CLI, IAM permission analysis, role assumption via STS,
recovery of previous object versions from S3 buckets.

**Web exploitation and application security**: subdomain and API enumeration, identification and
exploitation of public CVEs (unauthenticated remote code execution), analysis of vulnerable code paths
from source, JWT security (algorithm confusion and the alg=none flaw), forging authentication tokens.

**Container and Kubernetes security**: enumeration of a compromised pod, review of service account
permissions, abuse of the nodes/proxy permission to reach the kubelet, command execution inside a
privileged pod mounting the host filesystem for container-to-host escape.

---

## Contact

Giampiero Saponaro, junior cybersecurity specialist

- LinkedIn: [linkedin.com/in/giampiero-saponaro-cybersecurity](https://www.linkedin.com/in/giampiero-saponaro-cybersecurity)
- Portfolio: [giampierosap.github.io/GiampieroSaponaro](https://giampierosap.github.io/GiampieroSaponaro)

---

*All reports refer exclusively to authorised lab environments and completed CTF challenges.*
