# SecWordVault
SecWordVault is a specialized repository with wordlists for testing SQL injection vulnerabilities related to parameters and integers.


Tutorial: Running SQL Injection Vulnerability Tests with SecWordVault and Gobuster

1. Requirements:

Gobuster installed on your system. If not installed, download it from Gobuster GitHub repository.
Python installed on your system. If not installed, download it from Python.org.
SecWordVault repository cloned or downloaded to your local machine. Ensure you have the necessary wordlists specific to SQL injection parameters and integers.
2. Setting Up:

Clone or download the SecWordVault repository from SecWordVault GitHub repository.
Extract the downloaded files to a convenient location on your machine.
3. Running Gobuster with SecWordVault:

Open your terminal or command prompt.

Navigate to the directory where Gobuster is installed or extracted.

Use the following command structure to run Gobuster with SecWordVault wordlists:

bash
Copy code
gobuster sql -u <TARGET_URL> -w <PATH_TO_WORDLIST>
Replace <TARGET_URL> with the URL of the target website or application where you want to test for SQL injection vulnerabilities.

Replace <PATH_TO_WORDLIST> with the path to the specific SQL injection wordlist from SecWordVault included in your cloned repository. For example:

bash
Copy code
gobuster sql -u http://example.com -w /path/to/secwordvault/sql_injection_wordlist.txt
4. Analyzing Results:

Gobuster will begin scanning the specified URL with each payload from the SQL injection wordlist.
Monitor the terminal for any indications of successful injections or vulnerabilities detected.
Note down any URLs or parameters that return abnormal responses, as these may indicate potential vulnerabilities.
