# T1003 – Credential Dumping (LSASS Memory Dump)

This folder includes Sigma rules to detect attempts to dump the LSASS process memory — a well-known technique to steal credentials from RAM.

---

##  Description

Adversaries may try to extract credentials by accessing or dumping `lsass.exe`. Tools like `ProcDump`, `rundll32`, or direct access to `lsass.exe` are used in:

- Internal reconnaissance
- Post-exploitation credential harvesting
- Lateral movement & privilege escalation

---

## 📂 Rules in this Folder

| File | Description |
|------|-------------|
| `lsass_memory_dump.yaml` | Detects LSASS memory access attempts using procdump.exe, comsvcs.dll, etc. |

---

## 🔗 MITRE ATT&CK Mapping

- **T1003.001** – OS Credential Dumping: LSASS Memory
- **T1003** – Credential Dumping

---

🛡️ Rule maintained by [Abhiraj Singh](https://github.com/Cyberta1k)
