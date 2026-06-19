# cybersecurity-lab-
Educational cybersecurity lab documenting data hiding techniques (Steganography, Slack Space, NTFS Streams) and password recovery methods (Dictionary &amp; Brute-force attacks).
# Disclaimer
This project, including all scripts and documentation, is provided for educational and research purposes only. The author assumes no responsibility for any misuse of the information contained herein. Users are responsible for ensuring that all activities performed are within their own isolated laboratory environments and comply with all applicable local and international laws. Unauthorized access to computer systems or data is illegal.

## 🛠 Tools & Commands
To reproduce the lab, I used the following tools:

### Steganography (steghide)
- Embed data:
  ```bash
  steghide embed -cf coverfile.jpg -ef secret.txt```


Extract data:
steghide extract -sf stego_file.jpg

### Password Recovery (John the Ripper)
- Convert zip to hash:
  ```bash
```zip2john protected.zip > hash.txt```

Crack the hash:

```john hash.txt --wordlist=/usr/share/wordlists/rockyou.txt```
