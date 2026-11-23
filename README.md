# Blood Donation Management System with Donor Loyalty Program

## Project Structure
- `index.html`: Single-page application views (Home, Login, Register, Donor, Recipient, Search, Admin)
- `style.css`: Responsive UI styling
- `firebase-config.js`: Firebase project initialization
- `auth.js`: Firebase Authentication helpers
- `db.js`: Firestore CRUD operations, batch verification, and 90-day eligibility logic
- `app.js`: UI rendering, form validation, and event handling
- `firestore.rules`: Role-based Firestore security rules
- `manifest.json`: Web App Manifest

## Deployment Notes
1. Upload all files to the root of your GitHub repository and enable GitHub Pages (or deploy to Firebase Hosting / Netlify / Vercel).
2. In Firebase Console -> Authentication -> Settings -> Authorized domains, add your live domain (e.g., `bca1503524-art.github.io`).
3. To create an Admin account, register normally and manually change that user's `role` field from `"donor"` or `"recipient"` to `"admin"` in Firestore (`users/{uid}`).
