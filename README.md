# Modern Public Mission: School Website (Prototype)

Static website for Modern Public Mission, Midoora, Awantipora (J&K). No build step: the whole site is `index.html`.

## Files
- `index.html`: the website (pages, parent portal, office console)
- `vercel.json`: Vercel settings (security headers)
- `robots.txt`, `.gitignore`

## Deploy on Vercel
1. Create a new GitHub repository and upload these files to the root.
2. On vercel.com choose **Add New, Project** and import the repository.
3. Framework Preset: **Other**. Leave Build Command and Output Directory empty. Click **Deploy**.
4. Every later commit to the repository redeploys automatically.

## Edit school details
Open `index.html` and find `const C={` near the top of the `<script>`:
phone, WhatsApp number (digits with country code), email, address, hours, academic year, principal.
Set `formEndpoint` to a Formspree or Getform URL to receive application, visit and contact forms by email.

## Demo logins (prototype only)
- Parent: `MPM1001` / `demo123` (or `MPM1002`)
- Office: `admin` / `office123`

## Important
- Passwords are checked in the browser, and Office edits are saved only in that browser (localStorage). This is for review only.
- Before real use, add a backend (for example Supabase or Firebase) for secure accounts and shared data, and obtain school approval and parent consent for camera feeds.
- Replace demo names, numbers, illustrations and text with school-approved content.
