# task5-EL-



## 🛠 Tools Used
* **VirusTotal:** For static analysis and multi-engine detection reports.
* **Any.Run:** For interactive sandbox analysis and observing real-time behavior.

---

## 🔍 Malware Classification Reference
I have categorized the primary malware types studied during this task:

| Type | How it Spreads | Key Behavior |
| :--- | :--- | :--- |
| **Virus** | Attaches to host files | Requires human action to execute. |
| **Worm** | Exploits network vulnerabilities | Self-replicating; spreads without help. |
| **Trojan** | Social engineering (Phishing) | Disguises as useful software. |
| **Ransomware** | Exploits/Phishing | Encrypts data and demands a ransom. |



---

## 📂 Analysis Lifecycle
The analysis follows the standard malware lifecycle to understand the threat from start to finish:

1.  **Delivery:** How the sample enters the environment (e.g., Email, Web).
2.  **Execution:** The initial run of the malicious code.
3.  **Persistence:** How the malware stays on the system after a reboot.
4.  **Action on Objectives:** The final goal (Stealing credentials, encrypting files).



---

## 📊 Findings & Indicators (Example)
*This section summarizes the findings from a sample analysis conducted on VirusTotal.*

* **Sample Hash:** `ed01ebfbc9eb5bbea545af4d01bf5f1071661840480439c6e5babe8e080e41aa` (WannaCry)
* **Detections:** 70/72 Engines flagged as malicious.
* **Behavioral Indicators:**
    * **Network:** Attempts to connect to a specific kill-switch domain.
    * **Filesystem:** Massive file renaming and creation of `.wnry` extensions.
    * **Registry:** Modified startup keys to ensure execution upon login.

---

## 🛡️ Prevention Methods
To mitigate the risks identified in this analysis, the following should be implemented:
* **Regular Backups:** (Critical for Ransomware)
* **Endpoint Protection:** Deploying EDR/AV solutions.
* **Patch Management:** Keeping software updated to prevent worm propagation.
* **User Awareness:** Training to identify suspicious attachments.

---

## 🏁 Final Outcome
This task successfully demonstrates basic malware awareness and the ability to interpret automated detection reports to provide actionable security insights.
