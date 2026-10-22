# Whisk with Love - Online Bakery Catalog & Zero-Cost Order Tracker

A lightweight, zero-compute static website for **Whisk with Love** artisanal bakery. 
Designed to be hosted for free on **GitHub Pages**, **Cloudflare Pages**, or **AWS S3 static hosting**.

## Features
- **100% Free Hosting:** Pure HTML5/CSS3/Vanilla JS (No server or compute instances needed).
- **Interactive Shopping Cart:** Automatically aggregates quantities and totals.
- **Customer & Birthday Intake:** Gathers Customer Name, Mobile Number, and Date of Birth with the prompt: *"Need mobile number and dob for exciting customised offers"*.
- **Google Sheets Automated Database:** Automatically generates unique Customer IDs (e.g. `WWL-CUST-1001`) per distinct mobile number and logs order history via Google Apps Script.
- **Instant WhatsApp Checkout:** Seamlessly redirects to your verified WhatsApp Business account (`https://wa.me/message/743QZMFPNMQWC1`) with an itemized message.

## Quick Setup & Deployment

### 1. Host on GitHub Pages (Free URL & Free SSL)
1. Create a new repository on GitHub (e.g., `whisk-with-love`).
2. Push `index.html` to the repository.
3. In your repo: Go to **Settings** > **Pages** > Select Branch: `main` > Click **Save**.
4. Your website is instantly live at `https://<your-username>.github.io/whisk-with-love/`!

### 2. Connect to Google Sheets Tracker
1. Open your Google Sheet: [Whisk with Love - Customer & Orders Tracker](https://docs.google.com/spreadsheets/d/1JdRxHmvpbj3ZiyPoFnzZKDP-dp33OdC2HTR4NhLQB74/edit).
2. Go to **Extensions** > **Apps Script** and paste the Webhook script from the prompt.
3. Click **Deploy** > **New Deployment** > Select **Web app** (`Execute as: Me`, `Who has access: Anyone`).
4. Copy the deployment URL and replace `YOUR_GOOGLE_APPS_SCRIPT_WEB_APP_URL_HERE` inside `index.html` (line 332).
