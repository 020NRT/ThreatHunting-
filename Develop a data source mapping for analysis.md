## Data Source Mapping for Phishing Analysis

The purpose of data source mapping is to show which OSINT sources are used and what type of information can be collected from each source.

| Data Source | Data Collected | Purpose in Phishing Analysis |
|---|---|---|
| VirusTotal | URL reputation, security detections, domains, IP addresses, and related indicators | Check whether a URL or domain is malicious and collect related IOCs |
| Shodan | IP addresses, open ports, services, hosting information | Analyze the infrastructure connected to suspicious IP addresses |
| WHOIS | Domain registration information, registrar, creation date, and other available domain data | Investigate the registration details of suspicious domains |

### Data Flow

Phishing URL → VirusTotal → Related Domain/IP → Shodan → WHOIS

### Example

For this project, a phishing URL was analyzed using VirusTotal. VirusTotal was used to check its reputation and collect related threat information.

The associated IP address can be analyzed using Shodan to identify open ports, services, and hosting information. WHOIS can be used to collect available registration information about the domain.

### Conclusion

Each data source provides different information. VirusTotal helps identify malicious indicators, Shodan provides information about network infrastructure, and WHOIS provides domain registration information. Combining these sources helps to better understand phishing infrastructure.
