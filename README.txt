
India Car Data - Ready to Upload ZIP
-----------------------------------

Files included:
1) index.html
   - This is your website file (dark futuristic).
   - Open it in a text editor and replace the CSV_URL placeholder with your Google Sheets CSV link.
     Search for the string:https://docs.google.com/spreadsheets/d/e/2PACX-1vS4A9uRSbnibvXSQQlaHLCFBNUN9vIIs7aYp4kor5dm7EEcrExSHflbp4gNGjIlRTtRThJIJ1SpdNbe/pub?output=csv
     Replace the whole string inside quotes with your published CSV link:
       const CSV_URL = "https://docs.google.com/spreadsheets/d/e/2PACX-.../pub?output=csv";

   - Option A: Replace the CSV URL locally and then upload to GitHub.
   - Option B: Upload the file to GitHub as-is, then edit the file in the GitHub web editor to paste the CSV URL.

2) india_car_brands_sample.csv
   - Import this file to Google Sheets to get started:
     Drive -> New -> Google Sheets -> File -> Import -> Upload the CSV.
   - After importing, in Google Sheets: File -> Share -> Publish to web -> select CSV -> Publish
     Copy the CSV link (it will end with output=csv or similar).

3) README.txt (this file)

Thorough steps (Mac) to go live using GitHub Pages:
--------------------------------------------------
A) Prepare Google Sheet (get CSV URL)
  1. Open Google Drive, create a new Google Sheet, and import india_car_brands_sample.csv.
  2. In Google Sheets: File -> Share -> Publish to web.
  3. Choose "Entire Document" and "Comma-separated values (.csv)" and click Publish.
  4. Copy the published CSV link.

B) Edit index.html locally (optional)
  1. Open index.html (this file) with TextEdit (make sure to enable "Display HTML files as code")
     OR open with VS Code (recommended).
  2. Find: PASTE_YOUR_CSV_URL_HERE
  3. Replace with your Google Sheets CSV URL, for example:
       const CSV_URL = "https://docs.google.com/spreadsheets/d/e/2PACX-1v.../pub?output=csv";
  4. Save the file.

C) Create a GitHub repo and upload
  1. Go to https://github.com and sign in or create an account.
  2. Click "New repository".
  3. Name it (e.g., india-car-data). Set to Public (free).
  4. Upload the files:
     - Click "Add file" -> "Upload files" and drag index.html (and optionally india_car_brands_sample.csv).
     - Commit the changes.
  5. In the repo, go to Settings -> Pages (or Code and automation -> Pages) -> Source -> select "main branch / (root)", then Save.
  6. GitHub will provide a URL like:
       https://yourusername.github.io/india-car-data/
     It may take a minute to become active.

D) Edit on GitHub (if you didn't edit locally)
  1. In the repo file list, click index.html, then click the pencil icon to edit.
  2. Replace the placeholder CSV URL with your published Google Sheets CSV link.
  3. Commit the changes. The live site will reflect the CSV data.

E) Verify
  1. Open your GitHub Pages URL.
  2. If the page says "Put your Google Sheets CSV URL..." then the CSV URL is not set or the sheet isn't published.
  3. If it loads entries, you're done!

Notes & troubleshooting
-----------------------
- If the page shows "Failed to load CSV", double-check the published CSV URL and that you used "Publish to web" (not just Share).
- If logos don't load, it's okay; placeholder images will appear.
- To update data: edit the Google Sheet and re-publish (or it may auto-update).

If you'd like, tell me your GitHub username and I can prepare a short list of exact clicks to create the repo and upload the files step-by-step.
