
<br>
<br>
<br>

<div align="center">
   
|WV-Scanner|Multi WV Scanner Vulnerability Tool|for web application|
|----------------|--------------|-------------|
| `L`| `=`| `Local File Inclusion (LFI)`|
| `O`| `=`| `Open Redirection (OR)`|
| `X`| `=`| `Cross Site Scripting (XSS)`|
| `S`| `=`| `Structured Query Language Injection (SQLi)`|
|    |    | `Carriage Return Line Feed Injection (CRLF)`|

> **WV-Scanner** is an easy-to-use tool that finds web issues like `LFI` - `OR` - `SQLi` - `XSS` - `CRLF`. <br><br> *`Made by`* - [`Mohsin Ahmad , Muhammad Umair Khan , Mustafa Kamal`]

</div>

<hr>

<br>
<br>
<br>


| Features                          | About                                                                       |
|-----------------------------------|-----------------------------------------------------------------------------|
| `LFI Scanner`                     | Detect Local File Inclusion vulnerabilities.                                |
| `OR Scanner`                      | Identify Open Redirect vulnerabilities.                                     |
| `SQL Scanner`                     | Detect SQL Injection vulnerabilities.                                       |
| `XSS Scanner`                     | Identify Cross-Site Scripting vulnerabilities.                      
|
| `CRLF Scanner`                    | Detect Carriage Return Line Feed Injection vulnerabilities.                    |
| `Multi-threaded Scanning`         | Improved performance through multi-threading.                      
|
| `Customizable Payloads`           | Adjust payloads to suit specific targets.                            
|
| `Success Criteria`                | Modify success detection criteria for specific use cases.                              |
| `User-friendly CLI`               | Simple and intuitive command-line interface.                          |
| `Save Vulnerable URLs`            | Option to save vulnerable URLs to a file for future reference.                          |
| `HTML Report Generation`          | Generates a detailed HTML report of found vulnerabilities.                    |
<br>
<hr>
<br>
<br>

| Language                          | Packages                                                                     |
|-----------------------------------|-----------------------------------------------------------------------------|
| ***Python***| `Python 3.x` `webdriver_manager` `selenium` `aiohttp` `beautifulsoup4` `colorama` `rich` `requests` `gitpython` `prompt_toolkit` `pyyaml` `Flask`|

<br>
<hr>
<br>

## Installation With WSL Terminal (Windows Subsystem for Linux)

### Clone the repository

```bash
git clone https://github.com/mohsinkhan34/WV-Scanner.git
```
```bash
cd WV-Scanner
```

### Install the requirements

```bash
pip3 install -r requirements.txt

```
### If you Showing This Error You Must Create Virtual Environment

```
pip install -r requirements.txt
error: externally-managed-environment

× This environment is externally managed
╰─> To install Python packages system-wide, try apt install
    python3-xyz, where xyz is the package you are trying to
    install.

    If you wish to install a non-Kali-packaged Python package,
    create a virtual environment using python3 -m venv path/to/venv.
    Then use path/to/venv/bin/python and path/to/venv/bin/pip. Make
    sure you have pypy3-venv installed.

    If you wish to install a non-Kali-packaged Python application,
    it may be easiest to use pipx install xyz, which will manage a
    virtual environment for you. Make sure you have pipx installed.

    For more information, refer to the following:
    * https://www.kali.org/docs/general-use/python3-external-packages/
    * /usr/share/doc/python3.13/README.venv

note: If you believe this is a mistake, please contact your Python installation or OS distribution provider. You can override this, at the risk of breaking your Python installation or OS, by passing --break-system-packages.
hint: See PEP 668 for the detailed specification.

```
### ✅ Recommended Way (Safe):

#### 1. Create a virtual environment:

```bash
python3 -m venv WV-Scanner
```

#### 2. Activate it:

```bash
source WV-Scanner/bin/activate
```
Your prompt will now show something like `(venv)` to indicate you're in a virtual environment.

#### 3. Install packages from `requirements.txt`:

```bash
pip install -r requirements.txt
```
---
### ✅ If you don’t have `venv`:

Install the required package:

```bash
sudo apt install python3-venv
```
### ⚠️ If You Still Want to Use System Environment (Not Recommended):
```
You can bypass the restriction with this command:

```bash
```
pip install --break-system-packages -r requirements.txt
```
But **this can break your system**, so use it only if you absolutely know what you're doing.
```
### Run the Script

```bash
python3 WebScanner.py
```


| Input Information         |                                                                                         |
|---------------------------|-----------------------------------------------------------------------------------------|
| Input URL/File            | Provide a single URL or an input file containing multiple URLs for scanning.            |
| Payload File              | Select or provide a custom payload file for the specific type of vulnerability scanning.|
| Success Criteria          | Define patterns or strings indicating a successful exploitation attempt.                |
| Concurrent Threads        | Set the number of threads for multi-threaded scanning.                                  |
| View and Save Results     | Display results in real-time during the scan, and save vulnerable URLs for future use.  |

----

| Customization              |                                                                                          |
|----------------------------|------------------------------------------------------------------------------------------|
| Custom Payloads            | Modify or create payload files for different vulnerability types to target specific apps.|
| Success Criteria           | Adjust the tool's success patterns to more accurately detect successful exploitations.   |
| Concurrent Threads         | Control the number of threads used during the scan for performance optimization.         |


----

### Chrome Installation

```bash
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
```

```bash
sudo dpkg -i google-chrome-stable_current_amd64.deb
```

- If you encounter any errors during installation, use the following command:

```bash
sudo apt -f install
```

```bash
sudo dpkg -i google-chrome-stable_current_amd64.deb
```

----

### Chrome Driver Installation

```bash
wget https://storage.googleapis.com/chrome-for-testing-public/128.0.6613.119/linux64/chromedriver-linux64.zip
```
```bash
unzip chromedriver-linux64.zip
```
```bash
cd chromedriver-linux64 
```
```bash
sudo mv chromedriver /usr/bin
```
<hr>

<br>

<br>
