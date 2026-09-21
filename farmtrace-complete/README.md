# FarmTrace Complete MVP

Home page contains only landing/login/register. Modules are separate pages.

Routes: /dashboard /fields /crops /activities /inputs /expenses /harvests /history /ask /reports /profile

Each farmer has a separate account and every record is associated with that farmer. Passwords are salted/hashed with Node crypto.scrypt. Data is stored in data/db.json for the demo MVP.

## Run
1. Install Node.js 18+
2. Open this folder in VS Code
3. Terminal: npm install
4. Terminal: npm start
5. Open http://localhost:8080
6. Create a farmer account

For production: replace JSON storage with PostgreSQL, use secure persistent sessions/cookies, HTTPS, rate limiting, password reset/OTP, CSRF protection and server-side validation.

## Added in this version
- Multilingual interface with 15 Indian/local farmer language options: English, Hindi, Marathi, Gujarati, Kannada, Telugu, Tamil, Bengali, Punjabi, Malayalam, Odia, Assamese, Urdu, Konkani and Bhojpuri.
- Language selection is remembered in the browser and is available on the landing, login, registration and private app pages.
- Farmer account registration uses full name, 10-digit mobile number and password; login uses mobile number and password.
- Passwords remain salted/hashed with Node crypto.scrypt and farmer records remain isolated by farmer account.
- Theme selector with Green (default), Deep Green and Fresh Leaf options. The selection is remembered in the browser.
