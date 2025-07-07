# T1547 – Registry Run Key Persistence

This folder contains Sigma detection rules for identifying persistence techniques via modification of Windows Registry "Run" keys — commonly used by malware and adversaries to maintain access after reboot.

---

##  Description

The rule detects attempts to set persistence by modifying the following registry paths:
- `HKCU\Software\Microsoft\Windows\CurrentVersion\Run`
- `HKLM\Software\Microsoft\Windows\CurrentVersion\Run`

---

## 📂 Rules in this Folder

| File | Description |
|------|-------------|
| `registry_runkey_modify.yaml` | Detects modifications to Run keys in registry, a known persistence vector |

---

## 🔗 MITRE ATT&CK Mapping

- **T1547.001** – Registry Run Keys / Startup Folder
- **T1547** – Boot or Logon Autostart Execution

---

🛡️ Rule maintained by [Abhiraj Singh](https://github.com/Cyberta1k)
