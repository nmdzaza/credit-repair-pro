# credit-repair-pro

> **Built for Credit Repair Business Owners** — Automate your client workflow: generate dispute letters as PDFs, send them via email, and notify clients when their case is complete. All powered by Claude.

---

## What Is credit-repair-pro?

**credit-repair-pro** is a Claude plugin designed specifically for **credit repair business owners and professionals**. It automates the most time-consuming parts of running a credit repair service — analyzing client credit reports, drafting dispute letters as ready-to-send PDFs, emailing those documents directly to credit bureaus and creditors, and sending your clients a professional update message once everything is done.

Stop doing it manually. Let Claude handle the workflow while you focus on growing your business.

---

## Who Is This For?

- Credit repair business owners managing multiple clients
- Credit coaches and financial consultants
- Paralegals and consumer law professionals
- Anyone running a credit repair service who wants to automate client workflows

---

## Core Business Features

### 📄 PDF Dispute Letter Generation
Claude automatically drafts customized dispute letters for each client based on their credit report errors and exports them as **professional, ready-to-send PDF documents**. Each PDF includes:
- Client name and contact info
- Bureau-specific formatting (Experian, Equifax, TransUnion)
- Supporting argument language based on FCRA / FDCPA law
- Date, signature line, and reference numbers

### 📧 Automated Email Sending
Once dispute letters are drafted, credit-repair-pro sends them automatically:
- Emails dispute PDFs directly to the correct credit bureau(s)
- Emails creditors and collection agencies with negotiation letters
- Sends a copy to your client for their records
- Supports custom sender name and business email branding

### 💬 Client Completion Notifications
When a client's dispute round is complete, Claude automatically sends them a **professional status message** via email (or SMS if configured), letting them know:
- Which items were disputed and with which bureaus
- What to expect next and the timeline
- Any action they need to take on their end
- A summary of their dispute packet (PDF attached)

---

## Installation

### Requirements
- A Claude account (claude.ai)
- Access to Claude plugin/integration settings
- SMTP email credentials (Gmail, Outlook, or custom business email) for sending automated emails

### Steps to Install

1. **Download this plugin**
   - Click the green **Code** button at the top of this page
   - Select **Download ZIP**
   - Unzip the folder on your computer

2. **Open Claude**
   - Go to [claude.ai](https://claude.ai) and log in to your account

3. **Add the Plugin**
   - Navigate to **Settings > Integrations** (or the Plugins panel)
   - Click **"Add Plugin"** or **"Upload Plugin"**
   - Select the unzipped `credit-repair-pro` folder or the plugin config file

4. **Configure Your Business Settings**
   - Open `config.json` inside the plugin folder
   - Add your business name, email address, and SMTP credentials
   - Optionally add your logo for branded PDFs

5. **Enable the Plugin**
   - Toggle the plugin **ON** in your Claude settings
   - credit-repair-pro is now active and ready to use with your clients

---

## How to Use credit-repair-pro (Business Workflow)

### Step 1 — Add a Client
```
"Add a new client: [Client Name], email: [client@email.com]"
```
Claude creates a client profile and stores their information for the session.

---

### Step 2 — Upload or Paste the Client's Credit Report
```
"Here is my client's credit report: [paste report text or upload file]"
```
Claude analyzes the report from all three bureaus and identifies all disputable items — late payments, collections, errors, outdated accounts, and more.

---

### Step 3 — Generate Dispute Letters as PDFs
```
"Draft dispute letters for all errors found and export them as PDFs"
```
Claude creates bureau-specific dispute letters for each error, formatted professionally and exported as PDF files ready for sending.

---

### Step 4 — Send Dispute Emails to Bureaus & Creditors
```
"Send the dispute letters to the appropriate credit bureaus and creditors"
```
Claude emails the PDFs to Experian, Equifax, TransUnion, and any creditors involved — using your business email as the sender. Each email is logged for your records.

---

### Step 5 — Follow Up on Open Disputes
```
"Check follow-up status for [Client Name] and send reminder letters if needed"
```
Bureaus have **30 days** to respond. Claude tracks timelines and automatically drafts follow-up letters for any disputes that haven't received a response.

---

### Step 6 — Negotiate with Creditors on Behalf of Client
```
"Draft a pay-for-delete letter to [Creditor Name] for [Client Name]"
```
Claude drafts goodwill letters, pay-for-delete requests, and debt validation letters as PDFs and emails them directly to creditors.

---

### Step 7 — Notify the Client When Complete
```
"Send [Client Name] a completion message summarizing what was done"
```
Claude sends your client a **professional completion notification email** that includes:
- A full summary of all disputes filed
- The attached PDF dispute packet
- Next steps and expected timeline
- Your business contact info for follow-up questions

---

### Step 8 — Build Client's Credit Going Forward
```
"Give [Client Name] a personalized credit-building plan"
```
Claude creates a tailored plan covering secured cards, credit-builder loans, utilization targets, and payment scheduling — which can also be emailed to the client as a PDF guide.

---

## Example Business Commands

| What You Want | What to Say to Claude |
|---|---|
| Add a new client | "Add client: Jane Doe, jane@email.com" |
| Analyze credit report | "Analyze this credit report and find all disputable items" |
| Generate all dispute PDFs | "Draft dispute letters for all errors and export as PDFs" |
| Email bureaus | "Send dispute letters to all three credit bureaus" |
| Email creditor | "Send a pay-for-delete letter to Capital One for Jane" |
| Notify client | "Send Jane a completion email with the dispute summary" |
| Follow up | "Send follow-up letters for any disputes older than 30 days" |
| Build credit plan | "Email Jane a personalized credit-building plan as a PDF" |

---

## Email & PDF Configuration

In the `config.json` file inside the plugin folder, you can customize:

```json
{
  "business_name": "Your Credit Repair Business",
  "business_email": "you@yourbusiness.com",
  "smtp_host": "smtp.gmail.com",
  "smtp_port": 587,
  "smtp_user": "you@yourbusiness.com",
  "smtp_password": "your_app_password",
  "pdf_logo": "assets/logo.png",
  "pdf_footer": "Your Business Name | yourbusiness.com | (555) 000-0000"
}
```

---

## Disclaimer

credit-repair-pro is an informational and automation tool for business use. It is **not** a substitute for professional legal advice. All dispute letters are based on publicly available consumer protection laws (FCRA, FDCPA). Business owners are responsible for reviewing all documents before sending. Results may vary per client.

---

## Contributing

Got ideas or improvements? Pull requests are welcome!

1. Fork this repository
2. Create your feature branch: `git checkout -b feature/my-improvement`
3. Commit your changes: `git commit -m "Add my improvement"`
4. Push to the branch: `git push origin feature/my-improvement`
5. Open a Pull Request

---

## License

This project is open source and available under the [MIT License](LICENSE).

---

## Support

If this plugin is helping your business, please **star this repo** so other credit repair professionals can find it!
