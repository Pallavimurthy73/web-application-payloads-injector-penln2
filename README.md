Description
-----------
PenIn2 is a web application security testing tool that helps security professionals and researchers examine websites for possible vulnerabilities. It provides testing modules for SQL Injection, Cross-Site Scripting (XSS), directory brute-forcing, Local File Inclusion (LFI), and open ports. The tool also creates JSON and XML reports, making the scan results easier to review and analyze on your device.

Features
--------
1. Comprehensive Vulnerability Scanning: Checks web applications for common security issues, such as SQL Injection, XSS, and Local File Inclusion (LFI).
2. Directory Brute-Forcing: Searches for hidden files and directories with the help of customizable wordlists.
3. Open Port Scanning: Checks commonly used ports to discover services that may need further security assessment.
4. Flexible Payload Handling: Uses categorized payload files to support vulnerability testing across different modules.
5. Automated Report Generation: Produces audit reports in JSON and XML formats for documentation and further review.
6. Lightweight and Cross-Platform: Supports Windows, Termux, and other environments that can run Python.
7. Concurrent Testing: Uses multithreading to run scans more efficiently and reduce execution time when testing larger targets.

# PenIn2 Pentesting Tool

## Description
PenIn2 is a security assessment utility created to help security researchers examine web applications for potential weaknesses. Its available modules cover SQL Injection, Cross-Site Scripting (XSS), directory brute-forcing, Local File Inclusion (LFI), and open port scanning.

## Features

- SQL Injection detection
- Cross-Site Scripting (XSS) vulnerability testing
- Directory brute-forcing using custom wordlists
- Local File Inclusion (LFI) detection
- Open port scanning for common ports
- Comprehensive reports in JSON and XML formats

## Prerequisites
- Python 3.x
- Required Python libraries:
  - `requests`
  - `urllib3`
  - `socket`
  - `urllib`
  - `concurrent.futures`

Install dependencies using the following command: `pip install -r requirements.txt`

## How to Use
1. Organize Payload Files:  
   Keep each payload file in the folder assigned to its module:
   - SQL Injection payloads: Place in the `sqlpayloads` folder.
   - XSS payloads: Place in the `xss_payloads` folder.
   - LFI payloads: Place in the `lfi_payloads` folder.
   - Wordlists for directory brute-forcing: Place in the `wordlists` folder.  
   These folders are already included in the project structure. Add the relevant files to their corresponding folders.

2. Extract the Zip File:  
   Download and extract the `PenIn2.zip` file into a folder of your choice. This will create a directory containing the project files and the payload folders.

3. Run the Tool:  
   Open a terminal or command prompt and navigate to the extracted directory:
   `cd path/to/extracted/folder`

Execute the tool based on your environment:
- For Windows:  
  ```bash
  python t6.py
  ```
- For Termux/Linux:  
  ```bash
  python tm.py
  ```

4. Verify the Setup:  
   Confirm that the required payload files are available in their respective folders. If any are missing, the related testing modules may not work as expected.

Folder Structure
----------------
- sqlpayloads: Contains payloads for SQL Injection testing.
- xss_payloads: Contains payloads for Cross-Site Scripting (XSS) testing.
- lfi_payloads: Contains payloads for Local File Inclusion (LFI) testing.
- wordlists: Wordlists for directory brute-forcing.

License
-------
This project is licensed under the MIT License with Credit Restriction. See the LICENSE file for details.

