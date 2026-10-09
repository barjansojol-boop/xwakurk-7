# Xwakurk Basic School — multiple files in one ZIP

## Included files
- `index.html` — school homepage and sign-up form
- `styles.css` — responsive visual design
- `script.js` — student/teacher sign-up and English, Sorani Kurdish, Arabic translations
- `config.js` — teacher password setting
- `assets/school-logo.jpg` — school logo
- `README.md` — these instructions

## Teacher password
**Demo teacher password:** `XwakurkTeach2026!`

Change it in `config.js` before publishing:
`TEACHER_PASSWORD: "XwakurkTeach2026!"`

Keep in mind: if you publish this static website publicly on GitHub, a password placed in `config.js` is visible to anyone who views the site's source. This is a demo gate, not secure teacher-only access. For real teacher access, use a backend/server-side authentication and authorization system; do not publish the real teacher password in a public repository.

## How sign-up works in this starter
- No email field.
- Users choose Student sign-up or Teacher sign-up.
- Each account uses a name and a password.
- Teacher sign-up also asks for the teacher access password above.
- The demo stores accounts in local browser storage on the current device/browser. Accounts are **not shared across browsers/devices** and this is **not safe for real student records**. Password hashes in browser storage do not make the client-side system secure.

## Upload to GitHub Pages
1. Extract this ZIP file.
2. Create a repository at https://github.com/ (for example, `xwakurk-basic-school`).
3. Upload `index.html`, `styles.css`, `script.js`, `config.js`, `README.md`, and the `assets` folder. Keep the same structure.
4. Go to repository **Settings → Pages**.
5. Select **Deploy from a branch**, branch `main`, folder `/(root)`, then Save.
6. Wait for GitHub Pages to publish the site.

Official guide: https://docs.github.com/en/pages

## Before using for a real school
GitHub Pages is static hosting and cannot securely enforce a teacher password. For real multi-user accounts shared across devices, replace the demo storage with a backend such as Supabase or Firebase and enforce teacher permissions server-side. Do not store private student data until access controls are configured and tested.
