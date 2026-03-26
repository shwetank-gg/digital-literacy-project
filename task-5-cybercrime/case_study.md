# &#x20;Report on WannaCry Ransomware (Crime of ransom attack)



## &#x20;1. What the Crime Was

WannaCry was a crypto-ransomware worm that combined two dangerous elements:

\- Ransomware: Encrypting files and demanding payment in Bitcoin which made it untraceable .

\- Worm capability: Self-propagating across networks without user interaction.



It infected more than 200,000 computers in over 150 countries, which made it one of the largest ransomware attacks in history.





## 2\. How It Typically Happened (Step-by-Step)

#### 

#### Step 2a: Exploiting Eternal  blue

\- WannaCry used the Eternal  blue exploit, a vulnerability in SMB v1 (Server Message Block protocol) on Windows systems.

\- Eternal  blue allowed attackers to send specially crafted packets to port 445, establishing remote code execution.



#### &#x20;Step 2b: Installing a Backdoor (Double  pulsar)

\- After exploiting Eternal  blue, WannaCry checked for and took advantage of Double  pulsar, another leaked NSA tool.

\- Double  pulsar acted as a backdoor implant, making it easier to load and execute the ransomware payload on compromised systems.



#### Step 2c: Propagation Across Networks

\- Infected machines scanned local and external networks for other vulnerable systems.

\- It spread automatically, requiring no phishing emails or user clicks.

#### 

#### &#x20;Step 2d: Encryption of Files

\- Once inside, WannaCry created persistence via registry keys.

\- It encrypted a wide range of file types (documents, images, databases, etc.) using a hybrid cryptographic model:

&#x20; - AES (symmetric) for speed.

&#x20; - RSA (asymmetric) for securing keys.

\- Original files were deleted, leaving only encrypted versions with the .WNCRYT extension.



#### &#x20;Step 2e: Ransom Demand

\- Victims saw their wallpaper changed and a Wanna decrypter popup and demand $300 in Bitcoin.

\- A countdown timer threatened permanent loss of files if payment wasn’t made within 7 days.



#### &#x20;Step 2f: Poor Key Distribution

\- WannaCry used only three hardcoded Bitcoin addresses for all victims.

\- This made it impossible for attackers to track who had paid, meaning many victims never received decryption keys even after payment.







#### &#x20;Step 2g. The Kill Switch

\- WannaCry contained a hardcoded domain name. If the malware could connect to it, execution stopped.

\- A British researcher, Marcus Hutchins, discovered this domain was unregistered.

\- By registering the domain, he inadvertently activated the kill switch, halting spread of the initial strain.







#### &#x20;Step 2h. Patch Availability

\- Microsoft had released MS17-010 patch in March 2017, two months before the attack.

\- Many organizations failed to apply it, leaving systems exposed to Eternal  blue.





## 

## &#x20;4. Who Was Targeted

\- WannaCry did not target specific industries—it spread indiscriminately to any unpatched Windows system.

\- However, large organizations with outdated infrastructure were hit hardest.



&#x20;

## &#x20;5. Consequences of the attack

\- UK’s National Health Service (NHS) was severely impacted:

&#x20; - Hospitals had to cancel appointments and surgeries.

&#x20; - Doctors lost access to patient records.

&#x20; - Ambulances were diverted from affected facilities.

\- Globally, shipping companies, telecom providers, and government agencies were disrupted.

\- Financial losses were estimated in the hundreds of millions of dollars.

