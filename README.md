# Awesome IOCs with stars

<a href="https://en.wikipedia.org/wiki/Indicator_of_compromise"><img src="media/header.svg" width="100%" alt="Network graph with one node flagged as an indicator of compromise"></a>

Forensic artifacts, such as file hashes, domains, IP addresses and detection signatures, that identify malicious activity on a system or network.

## Contents

* [IOCs](#iocs)
  * [Indicators](#indicators)
  * [Snort and Suricata Signatures](#snort-and-suricata-signatures)
  * [YARA Signatures](#yara-signatures)
* [Tools](#tools)
  * [IOC Tools](#ioc-tools)
  * [IOC Formats](#ioc-formats)

## IOCs

### Indicators

* [Neo23x0/signature-base](https://github.com/Neo23x0/signature-base) ⭐ 3,043 | 🐛 18 | 🌐 YARA | 📅 2026-09-08 - YARA rules and IOCs behind the LOKI and THOR Lite scanners, curated for a low false-positive rate and updated frequently.
* [eset/malware-ioc](https://github.com/eset/malware-ioc) ⭐ 1,985 | 🐛 0 | 🌐 YARA | 📅 2026-09-17 - Indicators from ESET research publications, one directory per report and actively updated.
* [aptnotes/data](https://github.com/aptnotes/data) ⭐ 1,814 | 🐛 32 | 📅 2024-12-16 - Index of public reports on APT campaigns sorted by year, useful for tracing indicators back to the original vendor reporting.
* [volexity/threat-intel](https://github.com/volexity/threat-intel) ⭐ 373 | 🐛 0 | 🌐 YARA | 📅 2026-09-28 - IOCs from Volexity public threat research blog posts, organized by year and post.
* [Cisco-Talos/IOCs](https://github.com/Cisco-Talos/IOCs) ⭐ 293 | 🐛 8 | 🌐 Python | 📅 2026-09-30 - IOCs from Cisco Talos.
* [citizenlab/malware-indicators](https://github.com/citizenlab/malware-indicators) ⭐ 285 | 🐛 2 | 🌐 YARA | 📅 2020-10-04 - Indicators from Citizen Lab investigations into targeted attacks on civil society, one directory per report.
* [botherder/targetedthreats](https://github.com/botherder/targetedthreats) ⭐ 190 | 🐛 4 | 🌐 Python | 📅 2021-11-11 - Network indicators from reports on the targeting of civil society, published as CSV, JSON and generated Snort rules.
* [PaloAltoNetworks/Unit42-Threat-Intelligence-Article-Information](https://github.com/PaloAltoNetworks/Unit42-Threat-Intelligence-Article-Information) ⭐ 118 | 🐛 0 | 🌐 Python | 📅 2026-08-05 - IOCs and supporting data for Palo Alto Networks Unit 42 threat research articles, so indicators can be traced back to their write-up.
* [hvs-consulting/ioc\_signatures](https://github.com/hvs-consulting/ioc_signatures) ⭐ 35 | 🐛 0 | 🌐 YARA | 📅 2026-04-08 - IOCs, CSV context and YARA rules from HvS-Consulting incident response work, organized by threat actor or campaign for threat hunting.
* [cystack/stealer-fingerprints](https://github.com/cystack/stealer-fingerprints) ⭐ 20 | 🐛 0 | 🌐 Python | 📅 2026-10-06 - Fingerprints of infostealer log formats (banner strings, field signatures, YARA rules) for 30+ families including RedLine, Vidar, Lumma and StealC, for identifying which stealer produced a leaked log.
* [trilwu/apttrail](https://github.com/trilwu/apttrail) ⭐ 4 | 🐛 0 | 🌐 Python | 📅 2026-08-15 - APT indicators that carry the actor they belong to, its MITRE ATT\&CK group ID, when they first appeared and the report that published them.
* [DomainTools-Investigations/Malware-and-Scams](https://github.com/DomainTools-Investigations/Malware-and-Scams) ⭐ 3 | 🐛 0 | 📅 2026-09-10 - IOCs from DomainTools for malware and scams.
* [DomainTools-Investigations/Nation-State-Threats](https://github.com/DomainTools-Investigations/Nation-State-Threats) ⭐ 0 | 🐛 0 | 📅 2026-08-12 - IOCs from DomainTools for nation-state threats.
* [CIRCL OSINT Feed](https://www.circl.lu/doc/misp/feed-osint/) - CIRCL's public MISP feed of indicators from open-source reporting, ready to subscribe to from a MISP instance.
* [CyberBriefing IOC API](https://cyberbriefing.info) - Vendor-operated REST API that puts active IOCs from public feeds (AlienVault OTX, Abuse.ch URLhaus, ThreatFox, CISA KEV, Tor exit nodes, OpenPhish) behind one query interface; free tier requires an API key.
* [Extuno Malicious Package Database](https://extuno.com/malicious-db) - Vendor-operated database of malicious browser extensions and packages across 12 ecosystems (Chrome, Firefox, VS Code, npm, PyPI, WordPress and others), aggregated from OSV, OpenSSF and vendor feeds, for checking software supply-chain exposure; free web lookup and JSON endpoint.
* [ThreatCluster Public IOC Feed](https://threatcluster.io/feeds) - Vendor-operated feed of indicators extracted from clustered public reporting, available as TXT, CSV and JSON.
* [ThreatView Feeds](https://threatview.io/) - Free daily blocklists of malicious IPs, domains, URLs and file hashes, plus a C2 hunt feed of command-and-control servers with beacon configs; included in MISP's default feed list.

### Snort and Suricata Signatures

* [Emerging Threats Open](https://rules.emergingthreats.net/open/) - Free Proofpoint Emerging Threats ruleset for Snort and Suricata, a common baseline for network intrusion detection.
* [Snort Downloads](https://www.snort.org/downloads) - Official Snort rule sets, many of which also work with Suricata.

### YARA Signatures

* [Yara-Rules/rules](https://github.com/Yara-Rules/rules) ⭐ 4,911 | 🐛 29 | 🌐 YARA | 📅 2024-04-17 - Community-compiled YARA ruleset classified by threat type, a broad starting point for hunting.
* [elastic/protections-artifacts](https://github.com/elastic/protections-artifacts) ⭐ 1,496 | 🐛 10 | 🌐 YARA | 📅 2026-10-06 - YARA rules and EQL behavior rules used by Elastic Security for endpoint, with coverage mapped to MITRE ATT\&CK.
* [reversinglabs/reversinglabs-yara-rules](https://github.com/reversinglabs/reversinglabs-yara-rules) ⭐ 946 | 🐛 3 | 🌐 YARA | 📅 2025-11-03 - Detection-focused YARA rules from ReversingLabs threat analysts, written with the stated aim of zero false positives.
* [advanced-threat-research/Yara-Rules](https://github.com/advanced-threat-research/Yara-Rules) ⭐ 631 | 🐛 0 | 🌐 YARA | 📅 2025-03-18 - YARA rules that accompany Trellix Advanced Threat Research (formerly McAfee ATR) blog posts and investigations.
* [InQuest/yara-rules](https://github.com/InQuest/yara-rules) ⭐ 389 | 🐛 2 | 🌐 Python | 📅 2022-05-11 - YARA rules from InQuest research, intended for hunting rather than production detection; many are referenced from the [InQuest blog](http://blog.inquest.net).
* [intezer/yara-rules](https://github.com/intezer/yara-rules) ⭐ 131 | 🐛 0 | 🌐 YARA | 📅 2025-02-02 - YARA rules from Intezer malware research.
* [x64dbg/yarasigs](https://github.com/x64dbg/yarasigs) ⭐ 88 | 🐛 0 | 🌐 YARA | 📅 2019-05-23 - YARA signatures for identifying packers, compilers and crypto constants, useful during reverse engineering.

## Tools

### IOC Tools

* [ninoseki/mitaka](https://github.com/ninoseki/mitaka#downloads) ⭐ 1,875 | 🐛 5 | 🌐 TypeScript | 📅 2026-09-17 - Browser extension that looks up a selected IOC across many OSINT and scanning services from the context menu.
* [Neo23x0/yarGen](https://github.com/Neo23x0/yarGen) ⭐ 1,816 | 🐛 14 | 🌐 Python | 📅 2026-01-10 - Generates YARA rules from malware samples while filtering out strings common in goodware.
* [pedramamini/ThreatIngestor](https://github.com/pedramamini/ThreatIngestor) ⭐ 930 | 🐛 15 | 🌐 Python | 📅 2026-05-26 - Extendable framework that extracts and aggregates IOCs from threat feeds and passes them to other tools.
* [pedramamini/iocextract](https://github.com/pedramamini/iocextract) ⭐ 584 | 🐛 2 | 🌐 Python | 📅 2024-08-28 - Extracts IOCs from text, including defanged URLs, IP addresses and hashes.

### IOC Formats

* [MISP Malware Information Sharing Platform & Threat Sharing format](https://github.com/MISP/misp-rfc) ⭐ 55 | 🐛 11 | 🌐 HTML | 📅 2026-08-06 - Specifications for the MISP core format and related formats, used to exchange indicators between MISP and other platforms.
* [MITRE Malware Attribute Enumeration and Characterization (MAEC™)](https://maecproject.github.io/) - Schema for encoding malware behaviors, capabilities and attributes.
* [OASIS Structured Threat Information Expression (STIX™)](https://oasis-open.github.io/cti-documentation/) - A structured language and serialization format for exchanging cyber threat intelligence.
* [YARA](https://virustotal.github.io/yara/) - Pattern-matching language and tool for identifying and classifying malware, used by most signature collections in this list.

## Related Lists

* [Awesome Malware Analysis](https://github.com/rshipp/awesome-malware-analysis#readme) ⭐ 14,253 | 🐛 25 | 📅 2024-06-07 - Tools and resources for analyzing malware.
* [Awesome Threat Intelligence](https://github.com/hslatman/awesome-threat-intelligence#readme) ⭐ 10,703 | 🐛 142 | 📅 2026-05-31 - Threat intelligence sources, formats and platforms.
* [Awesome Incident Response](https://github.com/meirwah/awesome-incident-response#readme) ⭐ 9,433 | 🐛 87 | 📅 2026-07-15 - Tools and resources for security incident response.
* [Awesome YARA](https://github.com/pedramamini/awesome-yara#readme) ⭐ 4,285 | 🐛 1 | 📅 2026-06-15 - YARA rules, tools and resources.
* [Awesome Detection Engineering](https://github.com/infosecB/awesome-detection-engineering#readme) ⭐ 1,354 | 🐛 15 | 📅 2026-10-01 - Designing, building and operating detection controls.

## Contributing

Contributions are welcome. Read the [contribution guidelines](CONTRIBUTING.md) before opening a pull request.

## Footnotes

Archived, unmaintained and superseded sources are listed in [archived.md](archived.md).

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-10-07._
