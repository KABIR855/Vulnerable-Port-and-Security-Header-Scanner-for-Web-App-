# Vulnerable-Port-and-Security-Header-Scanner-for-Web-App-

Report By-
S M RAIHAN KABIR
Date: 1st March 2024


Python Script Functionality Overview

Introduction
The provided Python script offers functionality to assess the security posture of a website or IP address. It conducts checks on security headers and open ports, generating a detailed vulnerability report in PDF format.

 Features

1. **Security Headers Check**
   - Retrieves security headers from the target website.
   - Identifies missing security headers.
   - Provides explanations of the importance of each security header.

2. **Open Ports Check**
   - Scans common ports of the target host to identify open ports.
   - Provides descriptions of vulnerabilities associated with each open port.

3. **PDF Report Generation**
   - Generates a comprehensive vulnerability report in PDF format.
   - Includes details on the target host, security headers, missing security headers, and open ports.
   - Presents information in a structured and readable format.

 Implementation Details

- **Libraries Used:**
  - `requests`: For making HTTP requests to retrieve security headers.
  - `socket`: For scanning open ports on the target host.
  - `urllib.parse`: For parsing the input URL.
  - `reportlab`: For generating PDF reports.

- **Security Headers Check:**
  - Utilizes `requests.head()` method to retrieve HTTP headers.
  - Compares obtained headers with a predefined list of security headers.
  - Identifies missing headers and provides relevant explanations.

- **Open Ports Check:**
  - Utilizes socket connections to check the status of common ports.
  - Matches open ports with a predefined dictionary of associated vulnerabilities.
  - Provides vulnerability descriptions for open ports.

- **PDF Report Generation:**
  - Utilizes `reportlab` library to create PDF documents.
  - Constructs the report with information on the target host, security headers, and open ports.
  - Formats the report with appropriate headings, styles, and colors.


 Usage

1. **Input Prompt:**
   - Prompts the user to enter the URL or IP address of the target host.

2. **URL Validation:**
   - Validates the user input and ensures it starts with either "http://" or "https://".

3. **Execution:**
   - Initiates the security headers check and open ports scan.
   - Generates a PDF report summarizing the findings.

4. **Output:**
   - Displays the target host, identifies security headers, missing headers, and open ports during execution.
   - Prints a message confirming the generation of the PDF report.


Security Headers Check
Methodology
Request Headers Retrieval: Utilizes the requests.head() method to retrieve HTTP headers from the target host.
Comparison: Compares the obtained headers with a predefined list of security headers.
Identification: Identifies missing security headers by analyzing the presence of each header in the response.
Explanation: Provides detailed explanations for missing security headers, highlighting potential security risks associated with their absence.
Importance
Prevention of Attacks: Security headers play a vital role in mitigating various common web attacks such as Cross-Site Scripting (XSS), Clickjacking, and Data Injection.
Enhanced Security: Properly configured security headers help bolster the overall security posture of web applications by enforcing security policies and best practices.

Open Ports Check
Methodology
Port Scanning: Utilizes socket connections to scan common ports on the target host.
Port Status: Determines the status of each port, identifying whether it is open or closed.
Vulnerability Mapping: Matches open ports with a predefined dictionary of associated vulnerabilities.
Vulnerability Description: Provides detailed descriptions of vulnerabilities associated with each open port, elucidating potential risks and attack vectors.
Importance
Network Security Assessment: Open port scanning is crucial for identifying potential entry points for attackers and assessing the security of network configurations.
Vulnerability Mitigation: Understanding vulnerabilities associated with open ports enables proactive mitigation efforts, such as applying patches, implementing access controls, or employing network security solutions.



Dependencies

From terminal need to install mentioned packages with below commands:

1. **requests**: Used for making HTTP requests to retrieve security headers.
   ```
   pip install requests
   ```

2. **reportlab**: Utilized for generating PDF reports.
   ```
   pip install reportlab
   ```

These commands will install the necessary packages for the script to execute successfully. Once you've installed these packages, you should be able to run the script without any issues.

Conclusion

The Python script provides a convenient and systematic approach to assess the security vulnerabilities of a web application or server. By generating detailed reports, it assists security professionals in identifying and addressing potential risks effectively.












The End



