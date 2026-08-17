# Domain 1: General Security Concepts (Weight 12%) 

# Security Controls
- Anything that reduces the risk of a security threat or protects an organization's systems, data, or people

## Control Categories
### Technical controls: 
Protecting systems using technology
- E.g: Firewalls, anti-virus, Encryption

### Managerial controls: 
Policies created by management that explain to people the best way to manage their computers or data
- Administrative controls associated with security design and implementation
- E.g: Security policies, standard operating procedures

### Operational controls: 
Using people to implement and set these controls instead of systems
- E.g: Security guards, security awareness training, backup procedures

### Physical controls: 
Controls that limits someone's access to a building, a room, or a device
- Locks
- CCTV cameras
- Security guards
- Fences

## Control types
Control categories are who or what implements the control. Control types are what is the control's purpose.

### Preventive control type
Stops an attack before it happens
E.g:
- Firewall
- Follow security policy
- Guard shack checks all identification
- Enable door locks (Physical devices preventing access to a room)

### Deterrent control types
This control type does not directly prevent access but it discourages an intrusion attempt. In simpler terms it makes the attacker think twice before attacking
E.g:
- Application splash screens that provides security information and restricts people who are not authorized to gain access in the system
- Threat of demotion/dismissal
- Front reception desk
- Posted warning signs

### Detective control types
This control type detects that something has happened
E.g:
- Collect and review system logs
- Review login reports
- Regularly patrol the property
- Enable motion detectors

### Corrective control types
Fixes the problem after an incident 
E.g: 
- Restoring from backups can mitigate a ransomware infection
- Create policies for reporting security issues
- Contact law enforcement to manage criminal activity
- Use a fire extinguisher 

### Compensating control types
- Provides an alternative when the ideal control can't be used
E.g:
- Firewall blocks a specific application instead of patching the app
- Implement a separation of duties
- Require simultaneous guard duties
- Generator used after power outage

### Directive control type
- Tells people what they should do 
E.g:
- Store all sensitive files in a protected folder
- Create compliance policies and procedures
- Train users on proper security policy
- Post a sign for "Authorized Personnel Only"

In case you are confused think of it like this:
- Category = What kind of vehicle is it? (SUV, sedan, Truck)
- Type: What is the vehicle used for (Transporting people, towing, racing)

<img width="1109" height="429" alt="Screenshot (11)" src="https://github.com/user-attachments/assets/29f00d11-927d-417c-bdcc-f17bb97311fc" />

# The CIA Triad (Confidentiality, Integrity, Availability)
- The most important security concept. These are the three goals of security 

## Confidentiality 
- Keep information secret so only authorized people can access it
E.g: 
- Passwords
- Encryption
- Access control
- Example: Your bank account should only be visible to you and the bank, not everyone on the internet

## Integrity
- Ensure that information is accurate and has not been altered without authorization
E.g:
- Hashing: Map data of an arbitrary length to data of a fixed length
- Digital signatures: Takes a hash and encrypts it with an asymmetric encryption algorithm
- Certificates: To be able to identify devices or people
- Non-repudiation: Provides proof of integrity
- Example: If you transfer R500 to a friend, integrity ensures it doesn't get changed to R5,000 while being processed.

## Availability
- Make sure systems and data are available when authorized users need them
E.g:
- Backups
- Redundant servers
- Disaster recovery plans
- Example: An online banking website should still work when you need to check your balance

# Non-repudiation 

## Proof of integrity 
- Proof of integrity means that any data that we receive we can verify that it is exactly the same as the data we sent. Verifying that it has not been altered.
- In cryptography we use a hash to protect this data. A hash is a short string of text that we can create based on data that is contained within the plane text.
- If the data changes the hash changes

## Proof of origin 
- Using these hashes we can provide proof of integrity.
- We can also add an additional level of integrity called proof of origin where we can verify the person that sent the data to us. Sometimes you will see this refer to as Authentication.

# IAAA Framework (Identification, Authentication, Authorization, Accountability)
### Identification
- This is who you claim to be

### Authentication
- Proving that you are who you say you are

### Authorization 
- What access do you have based on your identification and authentication

### Accounting
- Login time, data, and logout time

## Authorization Models
- After the authentication process we authorize the device to have access to resources within our network using the authorization models
- There is a big list of different authorization models

# Gap Analysis 
- Gap Analysis is used to compare where you are now (the current state) with where you want to be (the desired future state). The "gap" is the difference between those two states, and the analysis helps identify what needs to change to close it.

# Zero Trust 
- Zero trust is an approach to network security where you have to authenticate or prove yourself each time you want to gain access to a particular resource.

## Ways to start implementing zero trust within a network
### Planes of operation
- Taking security devices and breaking them to smaller components
- Data Plane:
   - The Part of the device performing the security process
   - Switch, router, firewall
- Control Plane:
   - This is where we manage all the actions occurring in the data plane
   - This is where we configure policies and rules 
   - Determines how networks should be forwarded
 
# Physical Security
## Barricade 
- Prevents access to certain areas

## Access control vestibules
- This is where there is a room you must pass through to gain access to other accessibility

## Fence
- Build a perimeter ( Usually very obvious.)
- Transparent/opague, Robust, Prevent climbing

## Video surveillance
- CCTV

## Guards and access badges
- Security guard

# Deception and Disruption
- Disruption is preventing or interrupting an attacker's ability to operate
- Deception is used to mislead attackers or make them reveal themselves

## Types/forms of Deception technology: Honey-Something deliberately made attractive to an attacker. 
### Honeypot
- A way to attract the attackers to your system and keep them involved in the system to see what type of security techniques they're trying to use
- In simpler terms it is fake systems designed to attract attackers

### Honeynet
- A network containing multiple honeypots
- Consists of workstations, servers, and firewalls

### Honeyfile
- A fake file designed to attract an attacker
- Files that have fake information or they may be files that appear to be very important
- If someone gains access to the files you may want to have alerts

### Honeytokens 
- A piece of information or credential that can alert defenders when its used
- Tracks the malicious actors

# Change Management
- When making a change to an application or operating system the change is usually based in a single computer. But making a change within a company one single change could affect thousands of systems. So when making a change you need to go through a formal process to make sure that the change is going to work properly.
- The company should set policies that employees must follow

## In order to have a safe change process, the company must follow the following change approval process: 
- Complete the request forms
- Determine the purpose of the change
- Identify the scope of the change
- Schedule a date and time of the change
- Determine affected systems and the impact
- Analyze the risk associated with the change
- Get approval from the change control board
- Get end-user acceptance after the change is complete

# Technical change management 
- Technical change management refers to the implementation of the change management discussed in the previous points
- Change management is often concerned with what needs to change and technical change is who will implement the change management

# Public Key Infrastructure (PKI)
- Refers to policies, procedures, hardware, software, people that is responsible for creating, distributing, managing, storing, revoking, and performing other processes associated with digital certificates

## Symmetric encryption
- Means that anytime you decrypt something you use the same key that you used to encrypt that information (A single, shared key)

## Asymmetric encryption
- Means that you use two different keys to encrypt and decrypt
- when creating these keys you will assign one of them as the private key and the other as a public key
- Private key:
  - The private key is the one that one person/device has access to
- Public key
  - The public key is the one that anyone has access to. Anyone can see or use this key
 
## The key pair
- Building both the public and the private key at the same time

## Key escrow
- When dealing with a single person who happens to have their own public and private key pair, it is up to the individual to manage those

# Encrypting Data 
- Encryption is very important for protecting data on storage devices.

## Database encryption 
- It is important not to encrypt everything in the database only sensitive content

## Transport encryption
- Protect data traversing the network
- Encryption in the application
- VPN (Encrypts all data transmitted over the network)

## Encryption algorithms
- The formula used to encrypt and decrypt
- It is important for both parties to use the same encryption algorithm

## Cryptographic keys
- You have to have a proper key in encryption and decryption
- That key is what determines the output

## Key lengths
- Larger keys tend to be more secure
- 128-bit or larger symmetric keys are commons
