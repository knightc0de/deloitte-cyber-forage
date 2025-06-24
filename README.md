# 🛡️ Deloitte Virtual Internship Cyber Sim — Blue Teaming 

> “In cyber, every log tells a story — and  just read between the lines.”

Hey there! I recently took on the **Deloitte Australia Cyber Security Virtual Internship** via [Forage](https://www.theforage.com/) — real-world simulation that tested my defensive skills as a **Blue Teamer**.

It wasn’t just a slide deck or quiz. It was a threat-hunting mission 

---


A **mini bootcamp** to see how you think, act, and defend.

---

##  The Challenge: Detecting a Silent Breach at “Daikibo Industrials”

I was dropped into the shoes of a Security Operations Center (SOC) analyst at Deloitte.  
The scenario? A possible internal leak of sensitive industrial data. The dashboard was behind a VPN, yet the data leaked out.

###  mission:
-  Determine if the dashboard was externally accessible  
-  Analyze the `web_activity.log` file for anomalies  
-  Identify  what caused the breach  

---

## Reading-logfile Format 
![](/imgs/img1.png)


**What I did:**
-  Scanned for suspicious IP and user behavior  
-  Mapped request timing  automation  
-  Checked login patterns vs access anomalies  
-  Compared human vs bot-like activity  

---
# Scanning given Web_activity.log
### A massive chunk of HTTP activity segmented by static internal IPs. The format captured everything from login attempts to API requests, mapped against timestamps and status codes. 
![](/imgs/img2.png)
> I booted it into my Vim code editor 

#   Analyzing Every IP's Request Pattern
![](/imgs/img3.png)

## 🚨 Suspect Spotted: Scripted Access Detected
> No CSS, no JavaScript, no frontend files  
One user stood out like a glitch in the Matrix:  
 User ID:`dBCm2JjBU815PB8zPDvKqv`

 ## Normal login… then suddenly  
 ![](/imgs/im04.png)
 
### Precise API hits, on the hour  
🤖 This was no human. This was scripted access — silent, persistent, and efficient.

 Insider script abuse. Silent and persistent
---

#  Key Findings

**Q1: Was the dashboard accessible from outside?**  
🟢 No — it was behind a VPN.

**Q2: Who triggered the breach behavior ?**  
 User `dBCm2JjBU815PB8zPDvKqv` — behavior consistent with scripted scraping and machine-like querying frequency, accessing factory endpoints without UI resource calls.

---

##  Skills Unlocked

I leveled up in:

-  Threat Hunting — spotting malicious patterns in logs  
-  Behavioral Analysis — human vs machine behavior  
-  SOC Mindset  
-  Authentication Flow Analysis — tracking credential misuse  

---

## 📜 Certificate

🎉 Successfully completed the **Deloitte Cyber Simulation** on Forage.  

---

