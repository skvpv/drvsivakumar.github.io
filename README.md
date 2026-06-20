# Dr. V. Sivakumar — Academic Website

Single-file static site (`index.html`) for GitHub Pages.

## Deploy
1. Upload `index.html`, `.nojekyll`, and `README.md` to the repo root.
2. Settings ▸ Pages ▸ Source = "Deploy from a branch", Branch = `main`, Folder = `/ (root)`.

## CV is request-only (IMPORTANT)
The "Request CV" button opens a form that EMAILS you the visitor's details
(name, email, affiliation, purpose). The CV is NOT downloadable from the site.

### Activate the email form (one-time)
The form posts to **FormSubmit** (no signup). In `index.html`, find:
`CV_REQUEST_ENDPOINT = "https://formsubmit.co/ajax/sivakumarvit2013@gmail.com";`
1. Submit the form once on your live site. FormSubmit emails you an activation link — click it.
2. After that, every request is delivered to your inbox.

**Hide your email (recommended):** after activation, FormSubmit gives you a random alias
like `https://formsubmit.co/ajax/abc123…`. Replace the email in `CV_REQUEST_ENDPOINT`
with that alias so your address isn't visible in the page source.

**Alternative (Web3Forms):** create a free access key at web3forms.com and switch the
endpoint to `https://api.web3forms.com/submit`, adding `access_key` to the JSON body —
this keeps your email private without exposing it at all.
