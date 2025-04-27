# Security Policy

## Supported Versions

The ZapisAxis project currently supports the latest release version with security updates. We recommend always using the most recent version to ensure you have the latest security fixes and improvements.

| Version | Supported          |
|---------|--------------------|
| Latest  | ✅                 |
| Older   | ❌                 |

## Reporting a Vulnerability

We take security seriously and appreciate your efforts to responsibly disclose any vulnerabilities you find in ZapisAxis. To report a security issue, please follow these steps:

1. **Do Not Open a Public Issue**: Avoid disclosing the vulnerability publicly (e.g., in a GitHub issue) until it has been addressed.
2. **Contact Us Privately**:
   - Email the vulnerability details to [izeno.contact@gmail.com](mailto:izeno.contact@gmail.com).
   - Include a detailed description of the issue, steps to reproduce, potential impact, and any suggested fixes.
   - If possible, provide a proof-of-concept or screenshot to aid in understanding the issue.
3. **Response Time**:
   - We aim to acknowledge your report within 48 hours.
   - We will work with you to validate the issue and determine a fix timeline.
4. **Disclosure**:
   - Once the issue is resolved, we will coordinate with you on how to disclose the vulnerability responsibly.
   - Credit will be given to the reporter in release notes or documentation, unless you prefer to remain anonymous.

## Security Best Practices

To enhance the security of ZapisAxis, we recommend the following:

- **Update Password Storage**: The current version stores passwords in plain text in the `users` table. Consider contributing a patch to implement password hashing (e.g., BCrypt or SHA-256).
- **Secure Database Connections**: Ensure MySQL is configured with secure credentials and access controls when deploying ZapisAxis.
- **Regular Backups**: Use the built-in backup feature (`Settings.cs`) to create regular database backups.
- **Validate Inputs**: All user inputs are sanitized in the current version, but additional validation can be added for robustness.
- **Keep Dependencies Updated**: Regularly update NuGet packages (e.g., MySql.Data, ClosedXML, PdfSharp) to their latest secure versions.

## Known Limitations

- **Plain Text Passwords**: Passwords are stored in plain text in the `users` table, which is a security risk. We plan to address this in future releases.
- **Local Database**: The application relies on a local XAMPP MySQL instance, which may not be suitable for production environments without additional security measures.

If you have suggestions for improving security, please submit them via a pull request or issue, following our [Contributing Guide](CONTRIBUTING.md).

Thank you for helping keep ZapisAxis secure!

---