# CVE-2023-5360（CVSS v3.1：9.8)
Unauthenticated File Upload Vulnerability Addressed in Royal Elementor Addons and Templates 1.3.79

# Exploit
Step 1: Going to Home page, view source (Ctrl + U) and find `var WprConfig` and get `nonce` value (example: `56d8af27fb`)  
Step 2: Run script python with `nonce` value in step 1

```sh
python CVE-2023-5360.py http://localhost 56d8af27fb
```
# Ref
https://blog.wpscan.com/unauthenticated-file-upload-vulnerability-addressed-in-royal-elementor-addons-and-templates-1-3-79/