# Security Policy

## Supported Versions

This security policy applies to all public projects under my GitHub repositories. Security updates are provided for the following versions:

| Version | Status | Support Level |
| :--- | :--- | :--- |
| Latest stable | ✅ Supported | Active security updates & patches |
| Previous major | ⚠️ Limited | Critical vulnerabilities only |
| End-of-life (EOL) | ❌ Unsupported | No security updates |

> 🔒 **Best Practice:** Always keep your dependencies up to date and use the latest stable version of this project.

---

## Reporting a Vulnerability

We take security vulnerabilities seriously. Your efforts to responsibly disclose issues are appreciated.

### How to Report

**DO NOT** open a public GitHub issue. Instead, report privately via:

| Method | Contact |
| :--- | :--- |
| **Email (Primary)** | [support@basantmandal.in](mailto:support@basantmandal.in) |
| **Security-Specific** | [security@basantmandal.in](mailto:security@basantmandal.in) |

### What to Include

Provide as much detail as possible:

```markdown
- **Project:** [Repository name & version]
- **Description:** Clear explanation of the vulnerability
- **Impact:** What could an attacker do?
- **Steps to Reproduce:** Specific commands or actions
- **Environment:** OS, dependencies, configuration
- **Proposed Fix:** (optional, but helpful)
- **Disclosure Timeline:** Any specific requests (e.g., delay public disclosure)
```

### Response Timeline

| Timeframe | Action |
| :--- | :--- |
| **24-72 hours** | Acknowledgment of receipt |
| **5-7 days** | Initial assessment & severity rating |
| **10-14 days** | Fix developed & tested |
| **15-30 days** | Patch released & public disclosure |

> ⚠ **Note:** Complex vulnerabilities may require additional time. We will communicate regularly throughout the process.

---

## What to Expect

Once you report a vulnerability:

1. **Acknowledgment:** We will confirm receipt within 48 hours
2. **Validation:** We will verify the issue and assess its severity
3. **Fix:** We will develop and test a patch
4. **Release:** We will publish a security update
5. **Disclosure:** We will publicly disclose with credit (if you wish)

### Confidentiality

We will **not** share your report publicly or with third parties until:

- A fix has been released, or
- You have given explicit consent, or
- The legally required disclosure period has passed

---

## Scope

This security policy applies to:

- ✅ All public repositories under [basantmandal](https://github.com/basantmandal)
- ✅ Source code, Docker configurations, and documentation
- ✅ Official Docker images and releases
- ❌ Third-party dependencies (report to their respective maintainers)
- ❌ Hosting infrastructure or VPS provider issues

---

## Security Best Practices for Users

To keep your deployment secure:

### Environment Configuration

```bash
# Never commit secrets to version control
echo ".env" >> .gitignore

# Use strong, unique passwords
openssl rand -base64 32  # Generate secure password
```

### Network Security

- Expose services only to `127.0.0.1` (localhost) when possible
- Use SSH tunneling for database access
- Implement firewall rules on your VPS:

```bash
# Example: Allow SSH only, block public DB ports
ufw default deny incoming
ufw allow 22/tcp
ufw enable
```

### Regular Updates

```bash
# Update dependencies and rebuild
git pull origin main
```

---

## Contact Information

| Purpose | Contact |
| :--- | :--- |
| **Vulnerability Reports** | [support@basantmandal.in](mailto:support@basantmandal.in) |
| **Security Questions** | [support@basantmandal.in](mailto:support@basantmandal.in) |

---

## Acknowledgment

We follow industry best practices for responsible disclosure and thank the security community for helping keep open-source projects safe.

---

<div align="center">
  <b>Basant Mandal</b><br>
  <i>Full Stack Developer</i><br><br>

  <a href="https://www.basantmandal.in/"><img src="https://img.shields.io/badge/Website-000?style=flat-square&logo=ko-fi&logoColor=white" alt="Website"></a>
  <a href="https://www.linkedin.com/in/basantmandal/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:support@basantmandal.in"><img src="https://img.shields.io/badge/Email-support%40basantmandal.in-ea4335?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>
  
  <br>

  ---
  > *Copyright © 2026 Basant Mandal. All rights reserved.*
</div>
