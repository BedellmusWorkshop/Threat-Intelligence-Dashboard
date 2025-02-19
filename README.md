# Threat-Intelligence-Dashboard
Installed necessary packages:

sudo apt update && sudo apt install tcpdump python3-flask

# Capturing DNS Queries

sudo tcpdump -i any port 53 -n -w dns_capture.pcap

![Screenshot 2025-02-14 163619](https://github.com/user-attachments/assets/7b8ce632-4691-4878-bc4b-314bb238a5f6)

 Step 2 : Analyze the File

 ![Pasted image 20250218191635](https://github.com/user-attachments/assets/1ddf2278-1b75-49d9-aa2c-ff66fa9ddb94)

# Run tcpdump -r dns_capture.pcap -nn -vvv port 53 | grep -Eo '([0-9]{1,3}\.){3}[0-9]{1,3}' | sort -u > extracted_ips.txt

![Pasted image 20250218191301](https://github.com/user-attachments/assets/1ef56a65-2b64-4e24-8c8d-a03d8a27b83c)


### Write a script using an api to virustotal to check the ips


![VirusTotal](https://github.com/user-attachments/assets/98ba661d-8536-4cef-95c7-6db302038a54)

Step 3: Create a Dashboard to Display the Data


![Pasted image 20250218192539](https://github.com/user-attachments/assets/138c868a-c587-496c-8ee7-99907248bfe5)

Step 4: Run the Dashboard

Run: python3 dashboard.py

![Pasted image 20250218193943](https://github.com/user-attachments/assets/997a67ec-370e-403e-8264-29f8711a7be4)



