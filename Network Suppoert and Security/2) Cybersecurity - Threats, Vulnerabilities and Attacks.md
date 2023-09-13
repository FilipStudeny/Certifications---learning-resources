# Cybersecurity - Threats, Vulnerabilities and Attacks

# Common Threats
## Threat Domains 
A threat domain is considered to be an area of control, authority, or protection that attackers can exploit to gain access to a system.

There are many ways that attackers can uncover vulnerabilities and exploit systems within a domain.

Attackers can exploit systems within a domain through:

- Direct, physical access to systems and networks
- Wireless networking that extends beyond an organization’s boundaries
- Bluetooth or near-field communication (NFC) devices
- Malicious email attachments
- Less secure elements within an organization’s supply chain
- An organization’s social media accounts
- Removable media such as flash drives
- Cloud-based applications


## Types of Cyber Threats 

- Software attacks 
    -   A successful denial-of-service (DoS attack)
    -   A computer virus
- Software errors
    -   A software bug
    -   An application going offline
    -   A cross-site script or illegal file server share
- Sabotage
    -   An authorized user successfully penetrating and compromising an organization’s primary database
    -   The defacement of an organization’s website
- Human error
    -   Inadvertent data entry errors
    -   A firewall misconfiguration
- Theft
    -   Equipment is stolen
- HW failures
    -   Hard drive crashes
- Utility interruption
    -   Electrical power outages
    -   Water damage resulting from sprinkler failure
- Natural disasters
    -    Severe storms such as hurricanes or tornados
    -   Earthquakes
    -   Floods
    -   Fires
     
## Internal vs External Threats 
- **Internal threats** - From within company
- **External threats** - From outside

## User Threats and Vulnerabilities 
A user domain includes anyone with access to an organization’s information system, including employees, customers, and contract partners.

**Most common user threats**

- **No awareness of security** - Users must be aware of and understand an organization’s sensitive data, security policies and procedures, technologies, and countermeasures that are implemented in order to protect information and information systems.
- **Poorly enforced security policies** - All users must be aware of and understand an organization’s security policies, as well as the consequences of non-compliance.
- **Data theft** - Data stolen by users.
- **Unauthorized downloads and media**
- **Unauthorized virtual private networks (VPNs)**
- **Unauthorized websites**
- **Destruction of systems, applications or data**

## Threats to Devices 
- Any devices left powered on and unattended pose the risk of someone gaining unauthorized access to network resources.
- Downloading files, photos, music, or videos from unreliable sources.
- Exploit of security vulnerabilities within software installed on an organization’s device.
- Security teams must try to keep up to date with the daily discovery of new viruses, worms, and other malware that pose a threat to their devices.
- Users who insert unauthorized USB drives, CDs, or DVDs run the risk of introducing malware, or compromising data stored on their device.
- Policies are in place to protect an organization’s IT infrastructure. A user can face serious consequences for purposefully violating such policies.
- Using outdated hardware or software makes an organization’s systems and data more vulnerable to attack.

## Threats to the Local Area Network 
Examples of threats to the LAN include:
- Unauthorized access to wiring closets, data centers and computer rooms
- Unauthorized access to systems, applications and data
- Network operating system or software vulnerabilities and updates
- Rogue users gaining unauthorized access to wireless networks
- Exploits of data in transit
- Having LAN servers with different hardware or operating systems makes managing and troubleshooting them more difficult
- Unauthorized network probing and port scanning
-Misconfigured firewalls

## Threats to the Private Cloud 
The private cloud domain includes any private servers, resources, and IT infrastructure available to members of a single organization via the internet. 

This domain still poses significant security threats, including:
- Unauthorized network probing and port scanning
- Unauthorized access to resources
- Router, firewall or network device operating system or software vulnerabilities
- Router, firewall or network device configuration errors
- Remote users accessing an organization’s infrastructure and downloading sensitive data

## Threats to Applications
The application domain includes all of the critical systems, applications, and data used by an organization to support operations. Increasingly, organizations are moving applications such as email, security monitoring, and database management to the public cloud.

Common threats to applications include:
- Someone gaining unauthorized access to data centers, computer rooms, wiring closets or systems
- Server downtime during maintenance periods
- Network operating system software vulnerabilities
- Data loss
- Client-server or web application development vulnerabilities

## Threat Complexity 

### **Advanced persistent threat (APT)**
Continuous attack that uses elaborate espionage tactics involving multiple actors and/or sophisticated malware to gain access to the target’s network.
Attackers remain undetected for a long period of time, with potentially devastating consequences.

### **Algorithm attacks**
Takes advantage of algorithms in a piece of legitimate software to generate unintended behaviors. For example, algorithms used to track and report how much energy a computer consumes can be used to select targets or trigger false alerts. They can also disable a computer by forcing it to use up all its RAM or by overworking its central processing unit (CPU).

## Backdoors and Rootkits 
### Backdoors
Backdoor programs, such as **Netbus** and **Back Orifice**, are used to gain unauthorized access to systems by bypassing the normal authentication procedures.

Aauthorized users unknowingly run a **remote administrative tool program (RAT)** on their computer that installs a backdoor. The backdoor gives   administrative control over a target computer.

### Rootkits
Malware designed to modify the operating system to create a backdoor that attackers can then use to access the computer remotely.

Most rootkits take advantage of software vulnerabilities to gain access to resources that normally shouldn’t be accessible (privilege escalation) and modify system files. 

Rootkits can also modify system forensics and monitoring tools, making them very hard to detect. In most cases, a computer infected by a rootkit has to be wiped and any required software reinstalled.

## Threat Intelligence and Research Sources 
The United States Computer Emergency Readiness Team (US-CERT) and the U.S. Department of Homeland Security sponsor a database of **common vulnerabilities and exposures (CVE)**. These CVEs have been widely adopted as a way to describe and reference known vulnerabilities.

Each **CVE** entry contains a standard identifier number, a brief description of the security vulnerability, and any important references to related vulnerability reports. The CVE list is maintained by a not-for-profit, the MITRE Corporation, on its public website.

- **The Dark Web** - Encrypted web content that is not indexed by conventional search engines and requires specific software, authorization, or configurations to access. 
- **Indicator of Compromise (IOC)** - IOCs such as malware signatures or malicious domain names provide evidence of security breaches and details about them.
- **Automated Indicator Sharing (AIS)** - Automated Indicator Sharing (AIS), a Cybersecurity and Infrastructure Security Agency (CISA) capability, enables the real-time exchange of cybersecurity threat indicators using a standardized and structured language.  Structured Threat Information Expression (STIX) and Trusted Automated Exchange of Intelligence Information (TAXII) are standards used in AIS.

# Deception

## Social Engineering 
Social engineering is a non-technical strategy that attempts to manipulate individuals into performing risky actions or divulging confidential information.

Social engineering exploits human nature by taking advantage of people’s willingness to help or preying on their weaknesses, such as greed or vanity.

- **Pretexting** - This type of attack occurs when an individual lies to gain access to privileged data
- **Something for something (quid pro quo)** - Quid pro quo attacks involve a request for personal information in exchange for something, like a gift. 
- **Identity fraud** - This is the use of a person’s stolen identity to obtain goods or services by deception.

### Social Engineering Tactics 
- **Authority** - Attackers prey on the fact that people are more likely to comply when instructed by someone they perceive as an authority figure.
- **Intimidation**
- **Consensus** - Often called ‘social proof,’ consensus attacks work because people tend to act in the same way as other people around them, thinking that something must be right if others are doing it.
- **Scarcity** - A well known marketing tactic, scarcity attacks work because attackers know that people tend to act when they think there is a limited quantity of something available.
- **Urgency** 
- **Familiarity** - People are more likely to do what another person asks if they like this person.
- **Trust** - 

## Shoulder Surfing and Dumpster Diving 
**Shoulder surfing** - is a simple attack that involves observing or literally looking over a target’s shoulder to gain valuable information such as PINs, access codes, or credit card details. 

**Dumpster diving** — the process of going through a target's trash to see what information has been thrown out. 

## Impersonation and Hoaxes 
**Impersonation** - Pretending to be someone else to trick someone into doing something they would not ordinarily do.

**Hoaxes** - A hoax is an act intended to deceive or trick someone.

## Piggybacking and Tailgating 
Piggybacking or tailgating occurs when a criminal follows an authorized person to gain physical entry into a secure location or a restricted area. Criminals can achieve this by:

- Giving the appearance of being escorted into the facility by an authorized person
- Joining and pretending to be part of a large crowd that enters the facility
- Targeting an authorized person who is careless about the rules of the facility

## Other Methods of Deception 
- **Invoice scam** - Fake invoices are sent with the goal of receiving money from a victim by prompting them to put their credentials into a fake login screen. 
- **Watering hole** - Attacker observes or guesses what websites an organization uses most often and infects one or more of them with malware.
- **Typo squatting** - This type of attack relies on common mistakes such as typos made by individuals when inputting a website address into their browser. The incorrect URL will bring the individuals to a legitimate-looking website owned by the attacker.
- **Prepending** - Attackers can remove the ‘external’ email tag used by organizations to warn the recipient that an email has originated from an external source.
- **Influence campaigns** - Fake news, disinformation campaigns, and social media posts.


# Cyber Attacks
## Malware 
Malware is any code that can be used to steal data, bypass access controls or cause harm to or compromise a system.

### Viruses
A virus is a type of computer program that, when executed, replicates and attaches itself to other files, such as legitimate programs, by inserting its own code into the file. 

Viruses can be spread through removable media such as USB flash drives, internet downloads, and email attachments. The simple act of opening a file or executing an infected program can trigger a virus. Once a virus is active, it will usually infect other programs on the computer or other computers on the network. Viruses mutate to avoid detection.

> For example: Melissa virus

### Worms
A worm is a malicious software program that replicates by independently exploiting vulnerabilities in networks. Unlike a virus, which requires a host program to run, worms can run by themselves.

Worms share similar patterns: they exploit system vulnerabilities, they have a way to propagate themselves, and they all contain malicious code (payload) that causes damage to computer systems or networks.

### Trojan horse
A Trojan horse is malware that carries out malicious operations by masking its true intent. It might appear legitimate but is, in fact, very dangerous. Trojans exploit the privileges of the user who runs them.

Unlike viruses, Trojans do not self-replicate but often bind themselves to non-executable files, such as image, audio, or video files, that act as a decoy to harm the systems of unsuspecting users.

## Logic Bombs 
A logic bomb is a malicious program that waits for a trigger, such as a specified date or database entry, to set off malicious code. Until this trigger event happens, the logic bomb will remain inactive.

Once activated, a logic bomb implements malicious code that causes harm to a computer in various ways. 

## Ransomware
This malware is designed to hold a computer system or the data it contains captive until a payment is made.

## Denial of Service Attacks 
Denial of service (DoS) attacks are a type of network attack that is relatively simple to conduct, even for an unskilled attacker. These attacks are a major risk as they usually result in some sort of interruption to network services, causing a significant loss of time and money.

- **Overwhelming quantity of traffic** - This is when a network, host, or application is sent an enormous amount of data at a rate which it cannot handle. 
- **Maliciously formatted packets** - A packet is a collection of data that flows between a source and a destination computer or application over a network, such as the internet. When a maliciously formatted packet is sent, the receiver will be unable to handle it.

##  Domain Name System 
There are many essential technical services needed for a network to operate — such as routing, addressing, and domain naming. These are prime targets for attack.

- **Domain reputation** - Domain reputation is used to classify emails as spam or potential security threats.
- **DNS spoofing** - DNS spoofing or DNS cache poisoning is an attack in which false data is introduced into a DNS resolver cache — the temporary database on a computer’s operating system that records recent visits to websites and other internet domains.

    These attacks exploit a weakness in the DNS caching software that causes DNS servers to redirect traffic for a legitimate domain to the IP address of an illicit server.
- **Domain hijacking** - Attacker gains control of a target’s DNS information, they can make unauthorized changes to it. 
- **Uniform resource locator (URL) redirection** - A uniform resource locator (URL) is a unique identifier for finding a specific resource on the Internet. Redirecting a URL commonly happens for legitimate purposes.

## Layer 2 Attacks 
> Layer 2 refers to the data link layer in the Open Systems Interconnection (OSI) data communication model.

In its simplest terms, the MAC address identifies the intended receiver of an IP address sent over the network, and ARP resolves IP addresses to MAC addresses for transmitting data. 

### **Spoofing**
Spoofing, or poisoning, is a type of impersonation attack that takes advantage of a trusted relationship between two systems.

- MAC address spoofing occurs when an attacker disguises their device as a valid one on the network and can therefore bypass the authentication process. 
- ARP spoofing sends spoofed ARP messages across a LAN. This links an attacker’s MAC address to the IP address of an authorized device on the network.
- IP spoofing sends IP packets from a spoofed source address in order to disguise the packet origin.

### **MAC Flooding**
MAC flooding compromises the data transmitted to a device. An attacker floods the network with fake MAC addresses, compromising the security of the network switch.

# Man-in-the-Middle and Man-in-the-Mobile Attacks 
Attackers can intercept or modify communications between two devices to steal information from or to impersonate one of the devices.

- **Man-in-the-Middle (MitM)** - A MitM attack, also known as an on-path attack, happens when a cybercriminal takes control of an intermediate device without the user’s knowledge. 
- **Man-in-the-Mobile (MitMo)** - MitMo is a type of attack used to take control over a user’s mobile device. When infected, the mobile device is instructed to exfiltrate user-sensitive information and send it to the attackers.

## Zero-Day Attacks 
A zero-day attack, or zero-day, threat exploits software vulnerabilities before they become known or before they are disclosed by the software vendor.

## Keyboard Logging 
Keyboard logging or keylogging refers to recording or logging every key struck on a computer’s keyboard.

# Wireless and Mobile Device Attacks
## Grayware and SMiShing 

- **Grayware** - Any unwanted application that behaves in an annoying or undesirable manner. It may still pose a risk to the user by, for example, tracking your location or delivering unwanted advertising.
- **SMiShing** - Fake text messages prompt you to visit a malicious website or call a fraudulent phone number, which may result in malware being downloaded onto your device or personal information being shared. 

## Rogue Access Points 
A rogue access point is a wireless access point installed on a secure network without explicit authorization.

> Also known as a criminal’s access point

An **evil twin attack** describes a situation where the attacker’s access point is set up to look like a better connection option. Once you connect to the evil access point, the attacker can analyze your network traffic and execute MitM attacks.

## Radio Frequency Jamming 
Jamming radio signals

## Bluejacking and Bluesnarfing 
Bluetooth is a short-range, low-power protocol that transmits data in a personal area network (PAN) and uses pairing to establish a relationship between devices such as mobiles, laptops and printers.

- **Bluejacking** uses wireless Bluetooth technology to send unauthorized messages or shocking images to another Bluetooth device.
- **Bluesnarfing** occurs when an attacker copies information, such as emails and contact lists, from a target’s device using a Bluetooth connection.

## Attacks Against Wi-Fi Protocols 
**Wired Equivalent Privacy (WEP)** and Wi-Fi Protected Access (WPA) are security protocols that were designed to secure wireless networks.

**WEP** was developed to provide data transmitted over a wireless local area network (WLAN) with a level of protection comparable to what is usually expected of a traditional wired network. It added security to wireless networks by encrypting the data.

WEP’s initialization vector (IV) can be hijacked and used to gain access into network.

To address this and replace WEP, WPA and then WPA2 were developed as improved security protocols. Unlike with WEP, an attacker cannot recover WPA2’s encryption key by observing network traffic. However, they can still use a packet sniffer to analyze the packets going between an access point and a legitimate user.

# Application Attacks

## Cross-Site Scripting 
Cross-site scripting (XSS) is a common threat to many web applications:

1. Cybercriminals exploit the XSS vulnerability by injecting scripts containing malicious code into a web page.
2. The web page is accessed by the victim, and the malicious scripts unknowingly pass to their browser. 
3. The malicious script can access cookies, session tokens, or other sensitive information about the user, which is sent back to the cybercriminal.
4. Armed with this information, the cybercriminal can impersonate the user.

## Code Injection 
Injection attacks seek to exploit weaknesses in databases.
- **XML injection attack** - Can corrupt the data on the XML database and threaten the security of the website.
- **SQL injection attack** - SQL injection attack on websites or any SQL database by inserting a malicious SQL statement in an entry field.

    This attack takes advantage of a vulnerability in which the application does not correctly filter the data entered by a user for characters in an SQL statement. 
- **Dynamic link library (DLL)** - 
A dynamic link library (DLL) file is a library that contains a set of code and data for carrying out a particular activity in Windows. Applications use this type of file to add functionality that is not built-in, when they need to carry out this activity.

    DLL injection allows a to trick an application into calling a malicious DLL file, which executes as part of the target process.
- **Lightweight Directory Access Protocol (LDAP)** - Open protocol for authenticating user access to directory services.

    An LDAP injection attack exploits input validation vulnerabilities by injecting and executing queries to LDAP servers, giving cybercriminals an opportunity to extract sensitive information from an organization’s LDAP directory.  

## Buffer Overflow 
Buffers are memory areas allocated to an application. A buffer overflow occurs when data is written beyond the limits of a buffer. By changing data beyond the boundaries of a buffer, the application can access memory allocated to other processes. This can lead to a system crash or data compromise, or provide escalation of privileges.

## Remote Code Executions - RCE
Remote code execution allows to take advantage of application vulnerabilities to execute any command with the privileges of the user running the application on the target device.

Privilege escalation exploits a bug, design flaw, or misconfiguration in an operating system or application to gain access to resources that are normally restricted.

## Other Application Attacks 
- **Cross-site request forgery (CSRF)** - CSRF describes the malicious exploit of a website where unauthorized commands are submitted from a user’s browser to a trusted web application.
- **Race condition attack** - Also known as a time of check (TOC) or a time of use (TOU) attack, a race condition attack happens when a computing system that is designed to handle tasks in a specific sequence is forced to perform two or more operations simultaneously.
- **Improper input handling attack** - Data inputted by a user that is not properly validated can affect the data flow of a program and cause critical vulnerabilities in systems and applications that result in buffer overflow or SQL injection attacks.
- **Error handling attack** - Attackers can use error messages to extract specific information such as the hostnames of internal systems and directories or files that exist on a given web server — as well as database, table and field names that can be used to craft SQL injection attacks.
- **API attack** - An API delivers a user response to a system and sends the system’s response back to the user.
- **Replay attack** - This describes a situation where a valid data transmission is maliciously or fraudulently repeated or delayed by an attacker, who intercepts, amends and resubmits the data to get the receiver to do whatever they want.
- **Directory traversal attack** - Directory traversal occurs when an attacker is able to read files on the webserver outside of the directory of the website. 
- **Resource exhaustion attacks** - These attacks are computer security exploits that crash, hang or otherwise interfere with a targeted program or system. Rather than overwhelming network bandwidth like a DoS attack, resource exhaustion attacks overwhelm the hardware resources available on the target’s server instead.

## Spam
pam, also known as junk mail, is simply unsolicited email. In most cases, it is a method of advertising.

## Phishing
Phishing is a form of fraudulent activity often used to steal personal information.

- **Phishing** - Phishing occurs when a user is contacted by email or instant message — or in any other way — by someone masquerading as a legitimate person or organization. The intent is to trick the recipient into installing malware on their device or into sharing confidential information, such as login credentials or financial information.
- **Spear phishing** - A highly targeted attack, spear phishing sends customized emails to a specific person based on information the attacker knows about them — which could be their interests, preferences, activities, or work projects.

## Vishing, Pharming and Whaling 
- **Vishing** - Often referred to as voice phishing, this type of attack sees criminals use voice communication technology to encourage users to divulge information, such as their credit card details.
- **Pharming** - This type of attack deliberately misdirects users to a fake version of an official website. Tricked into believing that they are connected to a legitimate site, users enter their credentials into the fraudulent website.
- **Whaling** - Phishing attack that targets high profile individuals, such as senior executives within an organization, politicians and celebrities.