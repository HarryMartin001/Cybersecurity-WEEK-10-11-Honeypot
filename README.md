# Honeypot Assignment

**Time spent:** **22** hours spent in total

 Create a honeynet using MHN-Admin. Present your findings as if you were requested to give a brief report of the current state of Internet security. Assume that your audience is a current employer who is questioning why the company should allocate anymore resources to the IT security team.

### MHN-Admin Deployment 

 How did you deploy it? Did you use GCP, AWS, Azure, Vagrant, VirtualBox, etc.?What is difference between GCP and AWS?


Google Cloud Platform provides IaaS, PaaS, and serverless computing environments. A comparatively new Google Cloud Platform has all the tools and services required by developers and professionals. Amazon Web Services(AWS): It provides on-demand cloud computing platforms and APIs.
![MHN_Admin_Application](https://user-images.githubusercontent.com/111730072/205549082-ef4da64a-009c-449e-b28b-18f2a9dc82f7.gif)

<img src="mhn-admin.gif">

### Dionaea Honeypot Deployment 
![Animation](https://user-images.githubusercontent.com/111730072/205549529-11413fa2-92b5-43df-a6ed-33fef7946332.gif)

**Summary:** Briefly in your own words, what does dionaea do?


Dionaea with HTTP, and you'll see a Deploy Command appear with a full deployment script below it. You can ignore the script, which is just for reference, but make a note of the Deploy Command, which is the one-line command you'll need to execute inside the honeypot VM you connected to in the last step.
<img src="dionaea-honeypot.gif">

### Database Backup  
![Animation](https://user-images.githubusercontent.com/111730072/205549894-b63e7c5d-e29a-4820-b154-64c18b9bf305.gif)

**Summary:** What is the RDBMS that MHN-Admin uses? What information does the exported JSON file record?


Modern Honey Network (MHN). MHN's architecture is modular and extensible and comes with many options for deploying different types of honey pots. In MHN architecture, there is a single admin VM which is used to deploy, manage and collect information from the honeypots, which are deployed as separate VMs. Thus to run MHN, we'll need to setup at least two VMs: the single Admin VM and at least one Honeypot VM.
*Be sure to upload session.json directly to this GitHub repo/branch in order to get full credit.*

### 

#### X Honeypot

What does this honeypot simulate and do for a security researcher?

<img src="x-honeypot.gif">

### Malware Capture and Identification 

#### X Malware

**Summary:** How did you find it? Which honeypot captured it? What does each malware do?

MD5 Hash: *Run `md5sum` on the file and record the hash here.*

SHA1 Hash: *Run `sha1sum` on the file and record the hash here.*

<img src="x-malware.gif">

## Notes

Describe any challenges encountered 
 Issues encountered

p0f and Elastic Honey did not install due to OS mismatch (seems to need RedHat)
Otherwise, smooth deployments with GCP and MHN
iii. A summary of the data collected: number of attacks, number of malware samples, etc.

mhn-honeypot-1 (Dionea)
Attacks: 1760
Duration live: 8 hours
Protocols: pcap, SipSession, smbd, epmapper
mhn-honeypot-2 (Dionea with HTTP)
Attacks: 847
Duration live: 8 hours
Protocols: SipSession, smbd, pcap, SipCall
