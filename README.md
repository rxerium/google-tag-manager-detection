# Google Tag Manager Detection
Detect whether a host is tracking you through Google Analytics. 

 ## How does this detection method work?

This detection template sends a GET request to the target URL and checks for Google Tag Manager (indicators in the HTML source, specifically the GTM comment (<!-- Google Tag Manager -->) and requests to www.googletagmanager.com. If both conditions match and the response status is 200, it confirms the presence of GTM.

As of 04/01/25 there are ~360k instances running Google Tag Manager via Shodan (`http.html:"Google Tag Manager"`)
![image](https://github.com/user-attachments/assets/a6429f8f-f45f-40cc-8dff-7b7b2e35388d)


 ## How do I run this template?

1. Download Nuclei from [here](https://github.com/projectdiscovery/nuclei)
2. Copy the template to your local system
3. Run the following command: `nuclei -u https://yourHost.com -t <file.yaml>` 

## References

- https://tagmanager.google.com

## Disclaimer

Use at your own risk, I will not be responsible for illegal activities you conduct on infrastructure you do not own or have permission to scan.

# Contact

If you have any questions feel free to reach out to via [Signal](https://signal.me/#eu/0Qd68U1ivXNdWCF4hf70UYFo7tB0w-GQqFpYcyV6-yr4exn2SclB6bFeP7wTAxQw) or via email: rishi@rxerium.com.
