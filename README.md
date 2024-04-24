
<br />
<div align="center">
  <a href="https://github.com/socfortress/Wazuh-Rules">
  </a>

  <h3 align="center">Advanced Wazuh Detection Rules</h3>

  <p align="center">
    Have Wazuh deployed and ingesting your logs but looking for some better detection rules? Look no further. The objective for this repo is to provide the Wazuh community with rulesets that are more accurate, descriptive, and enriched from various sources and integrations.
  </p>
</div>


<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-this-repo">About This Repo</a>
      <ul>
        <li><a href="#supported-rules-and-integrations">Supported Rules and Integrations</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About This Repo

The objective for this repo is to provide the Wazuh community with rulesets that are more accurate, descriptive, and enriched from various sources and integrations.

Here's why:
* Detection rules can be a tricky business and we believe everyone should have access to a strong and growing ruleset.
* Wazuh serves as a great EDR agent, however the default rulesets are rather laxed (in our opinion). We wanted to start building a strong repo of Wazuh rules for the community to implement themselves and expand upon as new threats arise.
* Cybersecurity is hard enough, let's work together :smile:


<p align="right">(<a href="#readme-top">back to top</a>)</p>


### Supported Rules and Integrations

Below are the current rules and integrations currently contained within this repo. Integrations, such as Office365, Trend Micro, etc. will have scripts provided within their respective folders for use. Feel free to build upon these scripts and contribute back :smile:

* [Sysmon for Windows](https://github.com/socfortress/Wazuh-Rules/tree/main/Windows_Sysmon)
* [Sysmon for Linux](https://github.com/socfortress/Wazuh-Rules/tree/main/Sysmon%20Linux)
* [Office365](https://github.com/socfortress/Wazuh-Rules/tree/main/Office%20365)
* [Microsoft Defender](https://github.com/socfortress/Wazuh-Rules/tree/main/Office%20Defender)
* [Sophos](https://github.com/socfortress/Wazuh-Rules/tree/main/Sophos)
* [MISP](https://github.com/socfortress/Wazuh-Rules/tree/main/MISP)
* [Osquery](https://github.com/socfortress/Wazuh-Rules/tree/main/Osquery)
* [Yara](https://github.com/socfortress/Wazuh-Rules/tree/main/Yara)
* [Suricata](https://github.com/socfortress/Wazuh-Rules/tree/main/Suricata)
* [Packetbeat](https://github.com/socfortress/Wazuh-Rules/tree/main/Packetbeat)
* [Falco](https://github.com/socfortress/Wazuh-Rules/tree/main/Falco)
* [Modsecurity](https://github.com/socfortress/Wazuh-Rules/tree/main/Modsecurity)
* [F-Secure](https://github.com/socfortress/Wazuh-Rules/tree/main/F-Secure)
* [Domain Stats](https://github.com/socfortress/Wazuh-Rules/tree/main/Domain%20Stats)
* [Snyk](https://github.com/socfortress/Wazuh-Rules/tree/main/Snyk)
* [Autoruns](https://github.com/socfortress/Wazuh-Rules/tree/main/Windows%20Autoruns)
* [Sigcheck](https://github.com/socfortress/Wazuh-Rules/tree/main/Windows%20Sysinternals%20Sigcheck)
* [Powershell](https://github.com/socfortress/Wazuh-Rules/tree/main/Windows%20Powershell)
* [Crowdstrike](https://github.com/socfortress/Wazuh-Rules/tree/main/Crowdstrike)
* [Alienvault](https://github.com/socfortress/Wazuh-Rules/tree/main/Domain%20Stats)
* Tessian - WIP



<!-- GETTING STARTED -->
## Getting Started

Feel free to implement all of the rules that are contained within this repo, or pick and choose as you see fit. See our Installation section below for a bash script that can be ran on your Wazuh Manager to quickly put these rules to work!

### Prerequisites

Wazuh-Manager Version 4.x Required.

[Wazuh Install Docs](https://documentation.wazuh.com/current/index.html)

### Installation

_You can either manually download the .xml rule files onto your Wazuh Manager or make use of our wazuh_trident_rules.sh script_

> :warning: **USE AT OWN RISK**: If you already have custom rules built out, there is a good chance duplicate Rule IDs will exists. This will casue the Wazuh-Manager service to fail! Ensure there are no conflicting Rule IDs and your custom rules are backed up prior to running the wazuh_trident_rules.sh script!


1. Become Root User
2. Run the Script
   ```sh
   curl -so ~/wazuh_trident_rules.sh https://raw.githubusercontent.com/RemiOS0456/Wazuh-Rules/main/wazuh_trident_rules.sh && bash ~/wazuh_trident_rules.sh
   ```


<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

Security is best when we work together! Huge thank you to those supporting and those future supporters!

* [Wazuh Team](https://documentation.wazuh.com/current/index.html)
* [Taylor Walton](https://www.youtube.com/channel/UC4EUQtTxeC8wGrKRafI6pZg)
* [Juan Romero](https://github.com/juaromu)
* [SOCFortress](https://www.socfortress.co)
