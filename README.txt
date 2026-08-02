MPH COACH VERSION 1.0

WHAT THIS VERSION DOES
- Cashier enters only a cashier number.
- The app automatically loads that cashier's most recent performance date.
- The app compares the cashier to the warehouse average for that same date.
- All four sliders work: Ring Time, Tender Time, Inactive Time, Terminal Secure.
- The app shows a positive Biggest Win and Today's Focus.
- Reset returns the sliders to the cashier's latest real numbers.

FILES
1. index.html — replace the file in GitHub.
2. Code.gs — replace the code in Google Apps Script.

INSTALLATION
A. GOOGLE APPS SCRIPT
1. Open the Google Sheet.
2. Open Extensions > Apps Script.
3. Replace all existing code with Code.gs.
4. Save.
5. Open Deploy > Manage deployments.
6. Edit the existing Web App deployment.
7. Select New version and deploy.
8. Copy the Web App URL ending in /exec.

B. GITHUB
1. Open index.html in a text editor.
2. Find:
   const API_URL = "PASTE_YOUR_GOOGLE_APPS_SCRIPT_WEB_APP_URL_HERE";
3. Replace the placeholder with your /exec URL.
4. In GitHub, replace the entire existing index.html with this file.
5. Commit directly to the main branch.
6. Refresh the GitHub Pages site.

TEST
1. Enter a cashier number that exists in HISTORY.
2. Click LOAD MY COACH.
3. Confirm the latest performance date appears.
4. Move each slider and confirm MPH and numbers update.
5. Click RESET TO LATEST NUMBERS.

NOTE
The HISTORY tab must use this order:
A Performance Date
B Upload Date
C Cashier Number
D Inactive Time
E Tender Time
F Ring Time
G Terminal Secure
H Non-Sales Time
I Total Time
J Import Timestamp
