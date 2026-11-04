# Outreach Builder

Writes personalised first lines and short outreach emails from lawyer bios, then exports a CSV for Access Recruitment CRM.

Everything runs in your phone's browser. Your Anthropic API key is saved only in that browser. It is never stored in this repository.

## Turn on the web page (one time)

1. On your phone, open Chrome and go to github.com/leecwalker83-ship-it/outreach-builder. Sign in.
2. Tap the three dots at the top right of Chrome and tick "Desktop site". The GitHub app does not show these settings, so use the browser.
3. Tap "Settings" in the row of tabs near the top of the repository page.
4. In the left menu, tap "Pages".
5. Under "Build and deployment", set Source to "Deploy from a branch".
6. Under "Branch", choose "main", leave the folder as "/ (root)", and tap "Save".
7. Wait 1 to 3 minutes, then refresh. A box at the top shows your link: https://leecwalker83-ship-it.github.io/outreach-builder/
8. Open the link and add it to your home screen: Chrome menu, then "Add to Home screen".

This repository is public, so GitHub Pages works on a free account. If you ever make it private, the page stops working unless you pay for GitHub Pro. To make it public again: Settings, scroll to "Danger Zone", "Change repository visibility", "Make public", then confirm.

A public repository means anyone can see the code. No key or candidate data is in the code. Your key and the people you add stay in your phone's browser only.

## Get an Anthropic API key

1. Go to console.anthropic.com and sign in.
2. Add credit under "Billing". Each person costs roughly 2 to 5 US cents to write.
3. Go to "API Keys", tap "Create Key", name it "Outreach Builder", and copy it.
4. In the page, paste it in step 1 and tap "Save key", then "Test key".

## Use it

1. Step 2: upload a CSV, or paste bios with a line of three dashes (`---`) between each bio, then add names and emails.
2. Step 3: tap "Write emails". Each person appears as a card. Use Edit, Regenerate or Delete. Your edits are saved.
3. Step 4: tap "Download CSV". The file goes to your Downloads folder.

Rows marked "generic" had nothing specific in the bio. Rows marked "check wording" broke a writing rule twice; read them before sending.

Your list stays on the page until you tap "Clear everyone", even if you close the browser. Clearing Chrome's site data also removes it, along with the key.

## CSV columns for upload

The first row must have column names. These names work, in any order: First Name, Last Name, Email, Firm, Title, Office, Bio. A single "Name" column also works.

## Rename export columns

Open index.html on GitHub, tap the pencil icon, and find CSV_COLUMNS near the top of the script. Change only the text on the right of each line, such as "Email Subject", to match your CRM import template. Tap "Commit changes". The page updates within a few minutes.

The partner and associate closings, the model and other settings are just below CSV_COLUMNS.
