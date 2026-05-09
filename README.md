# Certificate CSV Generator

A single-page web app to generate session-specific certificate CSV files from your Main Certificate File.

## ✨ Features

- Upload your **Main Certificate File** (any size)
- Select the session: **Sunday Afternoon / Sunday Evening / Monday / Tuesday**
- Each session applies its own column structure and constant values — exactly matching the original template files
- Auto-splits output into **Part 1, Part 2, …** if the file exceeds your chosen size limit (default 2 MB)
- Download individual parts or all at once
- Runs 100% in the browser — no server, no data ever leaves your device

## 🚀 How to Publish on GitHub Pages

1. Create a new GitHub repository (e.g. `certificate-csv-generator`)
2. Upload `index.html` to the root of the repo
3. Go to **Settings → Pages**
4. Under **Source**, select `Deploy from a branch` → `main` → `/ (root)`
5. Click **Save**
6. Your app will be live at `https://<your-username>.github.io/certificate-csv-generator/`

## 📋 Session Column Mappings

| Session | Columns |
|---|---|
| Sunday Afternoon | Name, CountryCode, Phone, AllowBroadcast, AllowSMS, certlink, notes, datetime, brname, faqdoc, bonus |
| Sunday Evening | Name, CountryCode, Phone, AllowBroadcast, AllowSMS, certlink, notes, message, bns, link |
| Monday | Name, CountryCode, Phone, AllowBroadcast, AllowSMS, certlink, wel, linkedinpage, message |
| Tuesday | Name, CountryCode, Phone, AllowBroadcast, AllowSMS, brname, certlink, ylink, message, dmus |

All constant values (URLs, messages, brname, etc.) are pre-filled from the original template files.

## 🛠 Usage

1. Open the app in any browser
2. Drag & drop or click to upload your **Main Certificate File**
3. Click the session button for that day
4. (Optional) Adjust the **max file size** per part
5. Click **Generate CSV Files**
6. Download your files!

## 📁 Files

| File | Description |
|---|---|
| `index.html` | The entire app (single file, no dependencies except CDN PapaParse) |
| `README.md` | This file |
