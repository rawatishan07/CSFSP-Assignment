# Assignment 02: Linux Shell Scripting & Automation

**Course:** ETCCCP105 - Computer Science Fundamentals & Career Pathways 
<br>
**University:** K.R. Mangalam University, School of Engineering & Technology
<br>
**Author:** Ishan Rawat

---

## 1. Project Overview

This repository contains the shell scripts and supporting evidence for **Assignment Number 02: Basics of Linux and Open-Source Tools**. The project's goal is to demonstrate practical, hands-on experience with Linux shell commands and the use of shell scripting to automate common tasks

This repository specifically fulfills the requirements for Step 3 (Shell Script Development) and Step 4 (GitHub Repository Submission)  of the assignment.

The full assignment report, which includes:
* Linux (WSL/VirtualBox) installation documentation 
* The detailed table of 20 shell commands
* A reflection on challenges and learnings 

...is compiled in the main PDF/DOCX report and submitted separately on the university LMS.

## 2. Shell Scripts

This repository contains three functional shell scripts as required. Each script includes header comments, meaningful variable names, and explanatory comments for key steps.

### Script 1: `backup_script.sh` (Backup a Directory)

* **Description:** This script automates the backup of a specified directory. It creates a `.tar.gz` archive of the source directory and appends a timestamp to the filename to ensure unique backups.
* **Usage:**
    ```bash
    ./backup_script.sh /path/to/source_directory /path/to/backup_destination
    ```
    * **Example Output:** `/path/to/backup_destination/backup_2025-11-16_16-30-00.tar.gz`

### Script 2: `monitor_usage.sh` (CPU/Memory Monitoring)

* **Description:** This script monitors the system's CPU and memory usage.It captures a snapshot of the current usage (using commands like `top` or `free`) and appends this information along with a timestamp to a log file (`system_usage.log`). This script is intended to be run manually for a quick snapshot or as a cron job for regular logging.
* **Usage:**
    ```bash
    ./monitor_usage.sh
    ```
    * **Output:** Data is appended to `system_usage.log` in the same directory.

### Script 3: `download_file.sh` (Automated Download Task)

* **Description:** This script uses `wget` to download a file from a specified URL and save it to a predefined directory (`./downloads/`). It checks if the download directory exists and creates it if it doesn't.
* **Usage:**
    ```bash
    ./download_file.sh <URL_to_download>
    ```
    * **Example:** `./download_file.sh https://example.com/somefile.zip`

## 3. How to Run the Scripts

To run any of the scripts in this repository:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/](https://github.com/)[Your_Username]/linux-shell-assignment.git
    cd linux-shell-assignment
    ```

2.  **Make the script executable:**
    Before running a script for the first time, you must give it execute permissions using `chmod`.
    ```bash
    chmod +x backup_script.sh
    chmod +x monitor_usage.sh
    chmod +x download_file.sh
    ```

3.  **Run the script:**
    Follow the usage instructions for each script as detailed above.
    ```bash
    ./script_name.sh [arguments]
    ```

## 4. Evidence of Execution (Screenshots)

This repository also contains screenshots demonstrating the successful execution and output of each script, as required by the assignment.

* **`backup_output.png`**: Shows the `backup_script.sh` being executed and the resulting timestamped `.tar.gz` file.
* **`monitor_output.png`**: Shows the contents of the `system_usage.log` file after running `monitor_usage.sh`.
* **`download_output.png`**: Shows the `download_file.sh` successfully downloading a file into the `downloads` directory.

---
