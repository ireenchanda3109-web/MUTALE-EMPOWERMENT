MUTALE EMPOWERMENT — REAL APPLICATION SYSTEM

WHAT IT DOES
- Saves applications in a local SQLite database (applications.db).
- Provides a protected admin dashboard at /admin.html.
- Admin can view applications, change status, and export CSV.
- Public applicants receive a unique reference number.
- No payment processing is included.
- The portal is explicitly independent and must not be presented as a government website without authorization.

RUN LOCALLY
1. Install Node.js 18+.
2. Open a terminal in this folder.
3. Run: npm install
4. Set an admin password:
   Linux/macOS: ADMIN_PASSWORD="your-strong-password" npm start
   Windows PowerShell: $env:ADMIN_PASSWORD="your-strong-password"; npm start
5. Open http://localhost:3000
6. Admin dashboard: http://localhost:3000/admin.html

PRODUCTION
- Use HTTPS.
- Set strong ADMIN_PASSWORD and SESSION_SECRET environment variables.
- Put the database on persistent storage.
- Add backups, rate limiting, audit logs, consent/privacy notices, and a data-retention policy.
- Do not collect NRC/phone data unless you have a lawful and legitimate reason to do so.
- If this is a real empowerment programme, connect eligibility decisions to the programme's authorized rules rather than automatically promising an amount.
