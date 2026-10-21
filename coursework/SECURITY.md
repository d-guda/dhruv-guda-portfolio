# Educational security labs

Web security lab deliberately retains SQL injection and MD5 password hashing to demonstrate insecure design. Registration also uses those weak hashes. Successful login returns a demonstration message, not a session or authorization boundary.

1. Use an isolated local machine or disposable environment you control. Test only systems you own or have explicit permission to test.
2. The included command-line server binds to `127.0.0.1`. Do not change it to a public interface, forward its port, tunnel it, or deploy it.
3. Use synthetic accounts and disposable passwords only. The seeded `demo@juice-sh.op` / `demo-password` account is public lab data, not a real secret.
4. Running the app creates `web-security-lab/login-lab/users.db`. Keep it private and ignored. To reset the lab, stop the server, then delete that generated database and any associated `users.db-shm` or `users.db-wal` files locally.
5. Do not apply the vulnerable query or hashing patterns to production systems. See the [OWASP references](web-security-lab/SOURCES.md) for parameterization and modern password-hashing guidance; a remediated implementation is not included.

Loopback binding limits network reachability. It does not make vulnerable code safe or prevent another local process from reaching it. Do not run untrusted pages or software alongside the lab.

## Reporting an unexpected exposure

If you find personal information or real credentials in a copy of this collection, stop sharing that copy and contact its repository owner privately. Revoke or rotate exposed real credentials; removing a file alone does not clear repository history. See [GitHub's sensitive-data guidance](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/removing-sensitive-data-from-a-repository).

The intentional training weaknesses are documented educational behavior. No production security guarantees or supported deployment are provided.
