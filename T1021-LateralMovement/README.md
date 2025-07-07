# T1021 – Lateral Movement via Remote Services

This folder contains Sigma rules that detect adversary behavior consistent with lateral movement using remote execution tools like PSExec or SMB-based methods.

---

## 📘 Description

Remote process execution tools such as:
- `psexec.exe`
- `wmic.exe`
- `smbexec.py` (common in Cobalt Strike)

are widely used in internal network pivoting.

---

## 📂 Rules in this Folder

| File | Description |
|------|-------------|
| `psexec_like_execution.yaml` | Detects suspicious use of PsExec or related remote execution commands |

---

## 🔗 MITRE ATT&CK Mapping

- **T1021.002** – SMB/Windows Admin Shares
- **T1021.001** – Remote Services: Remote Desktop Protocol
- **T1021** – Remote Services

---

🛡️ Rule maintained by [Abhiraj Singh](https://github.com/Cyberta1k)
