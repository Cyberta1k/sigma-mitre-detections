# Sigma Detection Rules by MITRE ATT&CK ID

Curated Sigma rules written for real-world detection scenarios, aligned with MITRE ATT&CK techniques.

## 📁 Structure
Each folder = one MITRE technique. Inside: `.yaml` rule + brief explanation.

### Example Techniques:
- 🔹 T1059 - PowerShell Execution
- 🔹 T1547 - Registry Persistence
- 🔹 T1021 - Lateral Movement via PSExec
- 🔹 T1003 - LSASS Memory Dump

## 🛠 Tools Used
- SigmaHQ rule format
- ATT&CK Navigator (for mapping)
- Live test data from Windows, Wazuh, Sysmon

## 🤝 Contributions Welcome!
Feel free to fork, adapt, or suggest use cases.


## 🧭 MITRE ATT&CK Navigator Support

You can visualize the techniques covered in this repo with MITRE Navigator.

🔗 [Navigator Layer JSON](./mitre-navigator/abhiraj_sigma_mitre_layer.json)  
🧭 Load this file in [MITRE ATT&CK Navigator](https://mitre-attack.github.io/attack-navigator/enterprise/) to see visual technique coverage.

---
Maintained by [Abhiraj Singh](https://github.com/Cyberta1k)
