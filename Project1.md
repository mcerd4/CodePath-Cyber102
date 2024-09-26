## Project: Catch Me If You Can!

### Project Overview  
In this project, I analyzed a Business Email Compromise (BEC) scam targeting a company through phishing emails. Using Wireshark to inspect `.pcap` files, I identified fraudulent emails and uncovered the malicious actor responsible for the attack.

---

**Skills/Tools Used**  
- `.pcap` file analysis
- Email content extraction
- SMTP filtering in Wireshark
- Identification of fraudulent emails and actors

---

### Process:

1. **Analyze `.pcap` Files**  
   I used Wireshark to open and inspect packet capture (`.pcap`) files containing network traffic data related to email communications.

2. **Filter for SMTP Traffic**  
   `smtp`
   To isolate email-related traffic, I applied the SMTP filter.
   
4. **Filter SMTP requests**  
   `smtp.request`
   Filters packets that are SMTP requests, which include email headers, sender, and recipient details.
   
5. **Identify Legitimate vs. Fraudulent Emails**  
   By analyzing the content and metadata of each email, I searched the filtered packets for suspicious subject lines often associated with phishing. I found the following:
   
        "I can destroy everything!"
        "I seen everything!"
        "Your life about to get ruined!"

7. **Trace the Source IP Address**
   `10.6.1.104`  
   Once I identified the phishing emails by their subject lines, I examined the sender information in the email headers. The source IP address responsible for sending all the phishing emails was found to be:
   
---

**Outcome**  
I successfully mitigated the scam by analyzing network traffic and email data.
This project emphasizes my ability to use network analysis tools like Wireshark in cybersecurity investigations, especially for identifying phishing and email-based attacks.
