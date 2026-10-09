# SC-500 Cloud Security Portfolio

A collection of production-ready Kusto Query Language (KQL) scripts developed for threat hunting, incident response, and security monitoring within Microsoft Sentinel and Microsoft Defender XDR.

## 🛡️ Featured Threat Hunting Queries

### 1. MFA Fatigue / Voice Hammering Detection (`Identity_Threat_Hunting.kql`)
* **Objective:** Identifies potential multi-factor authentication (MFA) fatigue attacks where an attacker attempts to overwhelm a user with consecutive push notifications until they accidentally hit approve.
* **Logic:** Analyzes `SigninLogs` to flag users who experience 3 or more consecutive failed MFA prompt challenges within a 24-hour window, followed immediately by a successful login event.

---

## 🛠️ How to Deploy

1. Open your **Microsoft Sentinel** workspace or **Microsoft Defender XDR** portal.
2. Navigate to **Logs** -> **New Query**.
3. Copy the script from `Identity_Threat_Hunting.kql` and execute the search.
4. (Optional) Map the query rules directly into a Sentinel analytics rule to configure real-time SecOps alerting.

## 📚 Certifications & Training
* Completed alignment study paths for **Microsoft Exam SC-500: Microsoft Azure Security Technologies**.
