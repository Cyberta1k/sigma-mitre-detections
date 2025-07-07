# T1059 – Command and Scripting Interpreter (PowerShell)

This folder contains Sigma rules focused on detecting malicious PowerShell usage, aligned with [MITRE ATT&CK T1059.001](https://attack.mitre.org/techniques/T1059/001/).

---

## 📘 Description

PowerShell is a powerful built-in scripting language in Windows and is commonly abused by attackers to execute payloads, download remote scripts, or run encoded commands.

These rules aim to detect encoded or obfuscated PowerShell commands typically used in:

- Initial access
- Payload execution
- Living off the land techniques

---

## 📂 Rules in this Folder

| File | Description |
|------|-------------|
| `powershell_encoded_command.yaml` | Detects use of `-EncodedCommand` or `-enc` flag in PowerShell execution |

---

## 🛠️ Test Environment

- Log source: Windows Event Logs (`EventID 4688` from Sysmon or native logs)
- Category: `process_creation`
- Tested in: Wazuh, Elastic Stack, and Sigma CLI

---

## 🔗 MITRE ATT&CK Mapping

- **T1059.001** – PowerShell
- **T1059** – Command and Scripting Interpreter
- Tags used in rule:  
  `attack.execution`, `attack.t1059.001`, `powershell`, `encoded-command`

---

🛡️ Rule maintained by [Abhiraj Singh](https://github.com/Cyberta1k)
