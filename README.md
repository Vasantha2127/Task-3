# Task-3
Installation of Nessus Essentials:

I began by downloading and installing Nessus Essentials on my Kali Linux system. To do this, I visited the Tenable official website and selected the appropriate version for Kali. After downloading the installer package, I ran the following command to install it:

sudo dpkg -i Nessus-<version>.deb

Once installed, I started the Nessus service using:

sudo systemctl start nessusd

Then, I accessed the Nessus web interface by navigating to https://localhost:8834 in my browser. On first launch, I created a local Nessus account, selected Nessus Essentials, and entered my email to receive an activation code. After entering the code, Nessus downloaded its required plugins and initialized the setup, which took several minutes.

Setting the Scan Target:

After completing the setup, I logged into the Nessus dashboard. From there, I created a new scan. I chose the "Basic Network Scan" template. In the configuration settings, I set the target IP address to my local machine IP

Launching the Full Vulnerability Scan:

Once the scan was configured, I launched it directly from the Nessus dashboard. The scan took about 30 to 45 minutes to complete, as it performed a deep inspection of various services, ports, and configurations on my system. During this time, I monitored the scan progress through the Nessus interface.

Waiting for Completion:

I waited for the scan to complete while ensuring that no services were interrupted. Once the scan finished, Nessus displayed a summary report with the number of vulnerabilities found, categorized by severity: Critical, High, Medium, Low, and Informational.

Reviewing the Scan Report:

I clicked on the completed scan report to explore the results in detail. Nessus provided a list of identified vulnerabilities along with severity ratings and affected services. 
