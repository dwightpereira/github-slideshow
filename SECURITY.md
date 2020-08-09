# Security Policy

## Supported Versions

Here are the versions of your project are
currently being supported with security updates.

| Version | Supported          |
| ------- | ------------------ |
| 5.1.x   | :white_check_mark: |
| 5.0.x   | :x:                |
| 4.0.x   | :white_check_mark: |
| < 4.0   | :x:                |

## Reporting a Vulnerability

Remediation
Upgrade kramdown to version 2.3.0 or later. For example:

gem "kramdown", ">= 2.3.0"
Always verify the validity and compatibility of suggestions with your codebase.

Details
CVE-2020-14001
high severity
Vulnerable versions: < 2.3.0
Patched version: 2.3.0
The kramdown gem before 2.3.0 for Ruby processes the template option inside Kramdown documents by default, 
which allows unintended read access (such as template="/etc/passwd") or unintended embedded Ruby code execution 
(such as a string that begins with template="string://<%= `). NOTE: kramdown is used in Jekyll, GitLab Pages, GitHub Pages, and Thredded Forum..
