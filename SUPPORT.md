# Support for ZapisAxis

Thank you for using ZapisAxis! This guide provides resources and steps to get help with installation, usage, or troubleshooting.

## Table of Contents

- [Documentation](#documentation)
- [Troubleshooting](#troubleshooting)
- [Community Support](#community-support)
- [Contacting Maintainers](#contacting-maintainers)
- [Contributing to Support](#contributing-to-support)

## Documentation

The primary source of information for ZapisAxis is the [README.md](README.md) file, which includes:

- Installation instructions
- System requirements
- Usage guide
- Database structure
- Security features
- Backup and recovery procedures

For contributing or reporting issues, see the [Contributing Guide](CONTRIBUTING.md) and [Security Policy](SECURITY.md).

## Troubleshooting

Here are common issues and their solutions:

- **MySQL Connection Error**:
  - Ensure XAMPP is running and MySQL is active.
  - Verify the database `zapisaxisfms` exists in phpMyAdmin.
  - Check MySQL credentials in the application configuration.

- **Login Failure**:
  - Use the default credentials (username: `admin`, password: `admin`) for first-time access.
  - If locked out, use the [Recovery form](README.md#usage) to answer security questions.
  - Check the `users` table in the database for correct credentials.

- **Export Feature Not Working**:
  - Ensure you have write permissions in the selected export directory.
  - Verify that the table you’re exporting has data.
  - Check for missing dependencies (e.g., ClosedXML for Excel exports).

- **Application Crashes**:
  - Ensure .NET Framework 4.7.2 or higher is installed.
  - Check for sufficient disk space and memory.
  - Review error logs in the application directory (if enabled).

If your issue persists, check the [GitHub Issues page](https://github.com/VoxDroid/ZapisAxis/issues) for similar reports or open a new issue.

## Community Support

Join our community to ask questions, share tips, or help others:

- **GitHub Issues**: Post questions or bug reports at [https://github.com/VoxDroid/ZapisAxis/issues](https://github.com/VoxDroid/ZapisAxis/issues).
- **GitHub Discussions**: Participate in discussions at [https://github.com/VoxDroid/ZapisAxis/discussions](https://github.com/VoxDroid/ZapisAxis/discussions) (if enabled).
- **Search Existing Issues**: Many common questions have already been answered.

When posting, include:
- A clear description of the issue or question.
- Steps to reproduce the problem.
- Screenshots or error messages.
- Your environment (e.g., Windows version, XAMPP version).

## Contacting Maintainers

For direct support or sensitive issues (e.g., security vulnerabilities), contact the maintainers:

- **Email**: [izeno.contact@gmail.com](mailto:izeno.contact@gmail.com)
- **Response Time**: We aim to respond within 48 hours, though complex issues may take longer.

Please avoid sharing sensitive information (e.g., database credentials) in public channels.

## Contributing to Support

You can help improve ZapisAxis support by:

- Answering questions in GitHub Issues or Discussions.
- Improving documentation in the README or other guides.
- Adding troubleshooting tips to this SUPPORT.md file.
- Writing tutorials or creating video guides.

See the [Contributing Guide](CONTRIBUTING.md) for details on how to contribute.

---

<div align="center">
  <p><strong>Developed by <a href="https://github.com/VoxDroid">VoxDroid</a></strong></p>
  <p>Enjoying ZapisAxis? Consider supporting the project!</p>
  <a href="https://ko-fi.com/O4O6LO7Q1" target="_blank">
    <img src="https://ko-fi.com/img/githubbutton_sm.svg" alt="Support on Ko-fi" style="border: 0;">
  </a>
</div>

---

Thank you for being part of the ZapisAxis community!

---