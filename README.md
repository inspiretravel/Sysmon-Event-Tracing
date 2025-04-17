#  Sysmon-Event-Tracing

 🔍 Enhanced Sysmon Configuration for Windows Monitoring
This project aims to strengthen visibility into Windows system activities by using an optimized Sysmon configuration. By collecting detailed logs based on native Windows internals, this setup supports improved threat detection and faster incident response.

---------------------------------------------------------------------------------------------------------------



## 📌 Why Use This?
Gain deeper insights into process creations, network connections, registry changes, and more

Collect high-fidelity logs essential for threat hunting and forensic investigations

Strengthen your blue team capabilities with minimal overhead

---------------------------------------------------------------------------------------------------------------





## 🚀 Getting Started
Download and install Sysmon if you haven’t already.

Import the provided XML configuration file:
sysmonconfig-export.xml


- Install : Run with administrator rights
```
sysmon.exe -accepteula -i sysmonconfig-export.xml
```

- Update existing configuration : Run with administrator rights
```
sysmon.exe -c sysmonconfig-export.xml
```

Uninstall : Run with administrator rights
```
sysmon.exe -u
```

Validate logging through the Windows Event Viewer under: Applications and Services Logs > Microsoft > Windows > Sysmon > Operational

---------------------------------------------------------------------------------------------------------------


## 📁 Files Included
sysmon-config.xml: The tuned configuration file for enhanced logging

## 🛡️ Use Case
This configuration is ideal for:

  -SOC analysts and incident responders

  -Blue team lab setups

  -SIEM data enrichment (e.g., Elastic, Sentinel, Splunk)

  ---------------------------------------------------------------------------------------------------------------

## 📖 Resources

[SwiftOnSecurity](https://github.com/SwiftOnSecurity/sysmon-config?tab=readme-ov-file)

[More advanced sysmon log by HackerHurricane](https://www.malwarearchaeology.com/cheat-sheets)

