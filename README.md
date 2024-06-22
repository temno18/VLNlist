# SecWordVault

SecWordVault is a specialized repository featuring wordlists designed for testing SQL injection vulnerabilities related to parameters and integers.

#### Tutorial: Running SQL Injection Vulnerability Tests with SecWordVault and Gobuster

1. **Requirements:**

   - Gobuster installed on your system. If not installed, download it from [Gobuster GitHub repository](https://github.com/OJ/gobuster).
   - SecWordVault repository cloned or downloaded to your local machine. Ensure you have the necessary wordlists specific to SQL injection parameters and integers.

2. **Setting Up:**

   - Clone or download the SecWordVault repository from [SecWordVault GitHub repository](https://github.com/your-username/SecWordVault).

     **Clone Using HTTPS (recommended):**
     ```bash
     git clone https://github.com/temno18/SecWordVault.git
     ```

     **Clone Using SSH (if SSH keys are set up):**
     ```bash
     git clone git@github.com:your-username/SecWordVault.git
     ```

     **Download ZIP:**
     - Download and extract the ZIP archive from [SecWordVault GitHub page](https://github.com/your-username/SecWordVault/archive/refs/heads/main.zip).

3. **Running Gobuster with SecWordVault:**

   - Open your terminal or command prompt.
   - Navigate to the directory where Gobuster is installed or extracted.
   - Use the following command structure to run Gobuster with SecWordVault wordlists:

     ```bash
     gobuster sql -u <TARGET_URL> -w <PATH_TO_WORDLIST>
     ```

     Replace `<TARGET_URL>` with the URL of the target website or application where you want to test for SQL injection vulnerabilities.

     Replace `<PATH_TO_WORDLIST>` with the path to the specific SQL injection wordlist from SecWordVault included in your cloned repository. For example:

     ```bash
     gobuster sql -u http://example.com -w /path/to/secwordvault/sql_injection_wordlist.txt
     ```

4. **Analyzing Results:**

   - Gobuster will begin scanning the specified URL with each payload from the SQL injection wordlist.
   - Monitor the terminal for any indications of successful injections or vulnerabilities detected.
   - Note down any URLs or parameters that return abnormal responses, as these may indicate potential vulnerabilities.

#### Contributing

Feel free to contribute new wordlists or improvements to existing ones by forking this repository, making your changes, and submitting a pull request.

#### License

This project is licensed under the [MIT License](LICENSE).
