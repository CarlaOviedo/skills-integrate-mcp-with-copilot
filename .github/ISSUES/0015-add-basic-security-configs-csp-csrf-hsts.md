**Add basic security configs (CSP, CSRF, HSTS, session hardening)**

Description
-----------
Improve the security posture with sensible defaults: Content Security Policy (CSP), CSRF protection, HSTS, and secure session cookie settings.

Acceptance criteria
-------------------
- Add CSP and HSTS headers or configuration.
- Enable CSRF protection for non-API forms and document exceptions if needed.
- Harden session cookie configuration (secure, httpOnly, sameSite) in production configuration.

Labels: security, infra
Estimate: small
