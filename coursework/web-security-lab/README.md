# Web Security Lab

A local JavaScript/SQLite login application demonstrating account registration, database persistence, credential comparison, and an intentional SQL-injection bypass. The accompanying [web security analysis PDF](reports/juice-shop-dom-xss.pdf) documents the training observations.

> **Educational lab — intentionally vulnerable.** SQL injection and MD5 password hashes remain for controlled study. Use only in an isolated environment you own or are explicitly authorized to test. Never enter real credentials or deploy publicly. See [security guidance](../SECURITY.md).

## Run locally

Install Node.js 24.x. No external package installation is required. From this folder:

```bash
cd login-lab
node --test server.test.js
node server.js
```

Open <http://127.0.0.1:4174>. The server binds to loopback. Create a synthetic account using a disposable password, then log in. Stop with `Ctrl+C`. The generated `users.db` is ignored by Git.

## Intentional vulnerability

In your local copy, enter `' OR 1=1 -- @` as the login email with any nonempty disposable password. The concatenated SQL query can return the seeded demo account. This demonstrates the flaw only in this training application.

Registration uses a parameterized insert, but both registration and login use weak MD5 password hashes. Successful login returns a demonstration message, not an authenticated session. No completed secure variant is included.

## Source and evidence

- [Server](login-lab/server.js), [browser behavior](login-lab/app.js), and [automated tests](login-lab/server.test.js).
- Five existing tests cover validation, persistence, registration/login behavior, and the intentional bypass; all passed in the recorded local check.
- [Local lab screenshot](screenshots/login-lab.png) and [Juice Shop training screenshot](screenshots/juice-shop-dom-xss.png).
- [Sources](SOURCES.md) and [third-party attribution](../THIRD-PARTY-NOTICES.md).
