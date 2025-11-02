# Incident Response Playbook — [Detection Name]

**Detection Purpose:**  
Describe the detection (e.g., multiple failed SSH logins from the same IP).

---

## 1️⃣ Identification
**Trigger Conditions:**
- >10 failed logins from same IP within 5 minutes
- IP reputation flagged as malicious in VirusTotal

**Data Source:** Splunk export / `enriched_alerts.csv`

---

## 2️⃣ Containment
- Block IP at firewall or security group level.
- Isolate affected account or host.

---

## 3️⃣ Eradication
- Remove malicious access keys or sessions.
- Verify system integrity and patch if needed.

---

## 4️⃣ Recovery
- Reinstate clean configurations.
- Monitor post-incident traffic and authentication patterns.

---

## 5️⃣ Lessons Learned
- Tune alert thresholds.
- Integrate automatic IOC enrichment into workflow.
- Update detection logic for similar future attacks.
