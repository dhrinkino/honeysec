# HoneySEC

**HoneySec** is a project of interconnected honeypot systems that collects and processes information about login attempts.  
The output consists of aggregated lists of IP addresses that attempted unauthorized access to our infrastructure.

## Usage
⚠️ **Warning**  
It is not recommended to use direct links to files in this GitHub repository.  
Future changes to the repository structure or content may cause such links to break.  

👉 Always use the official links.

| Version   | Dataset | Link |
|-----------|---------|------|
| **raw**   | **ip_all** | https://honeysec.eu/lists/raw/ip_all |
| **raw**   | **ip_2**   | https://honeysec.eu/lists/raw/ip_2 |
| **raw**   | **ip_5**   | https://honeysec.eu/lists/raw/ip_5 |

| Version   | Dataset | Link |
|-----------|---------|------|
| **cidr**  | **ip_all** | https://honeysec.eu/lists/cidr/ip_all |
| **cidr**  | **ip_2**   | https://honeysec.eu/lists/cidr/ip_2 |
| **cidr**  | **ip_5**   | https://honeysec.eu/lists/cidr/ip_5 |

| Version   | Dataset | Link |
|-----------|---------|------|
| **ipset** | **ip_all** | https://honeysec.eu/lists/ipset/ip_all |
| **ipset** | **ip_2**   | https://honeysec.eu/lists/ipset/ip_2 |
| **ipset** | **ip_5**   | https://honeysec.eu/lists/ipset/ip_5 |

| Version   | Dataset | Link |
|-----------|---------|------|
| **mikrotik** | **ip_all** | https://honeysec.eu/lists/mikrotik/ip_all |
| **mikrotik** | **ip_2**   | https://honeysec.eu/lists/mikrotik/ip_2 |
| **mikrotik** | **ip_5**   | https://honeysec.eu/lists/mikrotik/ip_5 |

## Categories

| Dataset   | Description |
|-----------|-------------|
| **ip_all** | Contains all IP addresses that have logged into any of our honeypots at least once. |
| **ip_2**   | Contains IP addresses that logged into a honeypot at least 2 times. This filter helps eliminate false positives, typos, or one-off scanning attempts. (**recommended for most use cases**) |
| **ip_5**   | Contains IP addresses that logged into a honeypot at least 5 times. This dataset is suitable for analysis in environments with limited resources or when working only with the most reliable data. |

## Versions

| Dataset     | Description |
|-------------|-------------|
| **raw**     | Plain list of IP addresses, one per line. |
| **cidr**    | List of IP addresses with a `/32` prefix, one per line. |
| **ipset**   | Configuration in `ipset` command format, adding addresses to the **honeysec** list. |
| **mikrotik**| Ready-to-use commands for Mikrotik RouterOS 7+, creating an `address-list` named **honeysec**. |

## Acknowledgements
We would like to acknowledge the Institute of Computer Technologies and Informatics, Faculty of Natural Sciences, UCM in Trnava, for providing the infrastructure to host one of the probes used for attack collection.
