# Minor Project One: Password Cracking Lab 

## Project Description
This project demonstrates how weak passwords can be cracked using common password cracking methods such as dictionary attacks and brute-force attacks.

##  Goals
- Understand how password hashing concepts work
- Perform common password cracking methods
- Measure time taken to crack different passwords
- Understand the importance of strong passwords

## Tools Used
1. Kali Linux  
2. Oracle VirtualBox  
3. Hashcat  
4. John the Ripper  

## Environment Setup
- Oracle VirtualBox is used to run Kali Linux in an isolated environment.
- For safety and ethical reasons, all experiments are performed only inside Kali Linux using dummy data.

## Methodology

### 1. Dummy password creation 
- A list of dummy passwords with varying strength levels were created to simulate real-world user behavior. 
- Each password was converted to MD5 hash to simulate how real systems store passwords securely.

## Dictionary attack using John the Ripper
- The rockyou.txt wordlist was used to perform Dictionary attack using John the ripper tool.
- The tool compared the hashed values of Dictionary passwords with stored hashes.Multiple weak passwords were cracked using Dictionary attack.

## Dictionary attack using hashcat 
- Hashcat was executed in a CPU-based virtual environment, due to limited hardware resources performance was constrained.
- A smaller custom wordlist was used to simulate password cracking , and  weak passwords were cracked successfully.

## Brute-force attack using John the Ripper tool
- Brute force was performed using John's incremental mode .Password combinations were generated automatically.
-This attack was comparatively slower than dictionary attack, strong passwords were not cracked within limited execution time.

## Brute-force attack using hashcat
- Brute-force (mask) attack was performed using hashcat,attack attempted all possible character combinations .
- Due to CPU-only execution the attack was slow and strong passwords were not cracked within the observed time. 

## Time analysis
- time command was used to measure time taken by each attack method to crack weak passwords.

## What I Learned
- Practical use of John the Ripper and Hashcat.
- how password hashing works.
- version control using git and github.
- importance of hardware resources in password cracking.
- Learned how to measure and compare time taken for different cracking methods
- Gained awareness of ethical cybersecurity practices by using only dummy data



## Conclusion
This project successfully demonstrated how weak passwords can be cracked using dictionary and brute force attacks. Dictionary attacks proved to be fast and effective against common passwords ,while brute force attack were significantly slower and ineffective against strong passwords.The results highlight the importance of using strong , complex and unpredictable passwords to enhance security.