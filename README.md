# JE Drycleaning — Single-file Site (FULL VERSION)

This `index.html` contains the complete React + Tailwind app with:
- Paystack payments (inline checkout) — set your public key in the PAYMENT block
- Pay on Delivery
- Google Sheets order logging (Apps Script Web App URL)
- Optional Email notifications via EmailJS

## Deploy (GitHub Pages)
1) Create a new public repo and upload `index.html`.
2) Settings → Pages → Source: Deploy from a branch → main / (root).
3) Open the GitHub Pages URL.

## Netlify Drop
Go to https://app.netlify.com/drop and drop a folder with `index.html`.

## Configure
Open `index.html` and set:
```js
const PAYMENT = { paystackPublicKey: "pk_test_xxxxx" };
const INTEGRATIONS = {
  sheetUrl: "https://script.google.com/macros/s/XXXX/exec",
  emailjs: { publicKey: "...", serviceId: "...", templateId: "...", toEmail: "owner@example.com" }
};
```
