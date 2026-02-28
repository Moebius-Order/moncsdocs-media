# Security Policy

## Overview

This security policy applies to the **MON CS DOCS Media** repository. We are committed to maintaining the security and integrity of all media assets used by the MON CS DOCS platform.

This repository contains images, diagrams, illustrations, and related visual resources. While it does not host executable code, we maintain security standards to protect against malicious content, unauthorized modifications, and intellectual property violations.

## Supported Versions

Security updates are applied to the current `main` branch. Media assets are versioned alongside the main moncsdocs repository. Deprecated or replaced assets may be removed rather than patched.

| Version | Supported          |
| ------- | ------------------ |
| main    | :white_check_mark: |
| < 1.0   | :x:                |

## Reporting a Vulnerability

If you discover a security issue related to media assets in this repository, please report it through one of the following channels:

### Primary Channels

1. **Private Vulnerability Reporting** (Recommended)
   - Use GitHub's private vulnerability reporting feature
   - Navigate to the "Security" tab → "Report a vulnerability"
   - This creates a private security advisory visible only to repository maintainers

2. **Email**
   - Primary: [security.mon@moebiusorder.com](mailto:security.mon@moebiusorder.com)
   - Alternate: [mcdocs@moebiusorder.com](mailto:mcdocs@moebiusorder.com)

3. **Web Form**
   - Submit via: [mcdocs.moebiusorder.com/report](https://mcdocs.moebiusorder.com/report)

4. **GitHub Issue** (For non-sensitive security improvements only)
   - Use for security enhancements or policy clarifications
   - Do NOT use for active vulnerabilities or sensitive disclosures

### What to Include

When reporting a vulnerability, please provide:

- **Asset Path**: Full path to the affected media file(s)
- **Description**: Clear explanation of the security concern
- **Impact Assessment**: Potential harm to users or platform integrity
- **Evidence**: Screenshots, file metadata, or technical analysis
- **Discovery Method**: How you identified the issue
- **Suggested Remediation**: Recommendations for fixing or replacing the asset

### Reportable Issues

Please report:

- **Malicious Content**: Embedded scripts, exploits, or malware in image files
- **Privacy Violations**: Assets containing personally identifiable information (PII)
- **Intellectual Property Issues**: Copyright violations or unauthorized use of third-party assets
- **Metadata Exposure**: Sensitive information in EXIF or file metadata
- **Supply Chain Concerns**: Compromised source files or suspicious modifications
- **Access Control Issues**: Unauthorized access to private or restricted media

### Out of Scope

The following are generally out of scope:

- Vulnerabilities in the MON CS DOCS platform infrastructure (not in this repository)
- Issues with third-party hosting, CDN, or delivery mechanisms
- General quality concerns or artistic feedback unrelated to security
- Social engineering attempts or phishing unrelated to repository content
- Denial of service against GitHub or CDN infrastructure

## Response Process

### Timeline

- **Acknowledgment**: We will acknowledge receipt of your report within **48 hours**
- **Initial Assessment**: Triage and severity assessment within **5 business days**
- **Status Updates**: Regular updates every **7 days** until resolution
- **Resolution**: Critical issues will be addressed within **30 days** when feasible

### Severity Classification

We use the following severity levels:

- **Critical**: Active malicious content threatening user safety or system integrity
- **High**: Significant security or privacy risk with clear exploitation path
- **Medium**: Moderate risk requiring specific conditions to exploit
- **Low**: Limited impact or theoretical vulnerability
- **Informational**: Security improvements or best practice recommendations

### Remediation Actions

Depending on severity, we may:

1. **Remove**: Delete the affected asset immediately
2. **Replace**: Substitute with a secure alternative
3. **Sanitize**: Strip metadata or re-encode to remove embedded threats
4. **Quarantine**: Move to private storage pending investigation
5. **Update Documentation**: Revise usage guidelines to prevent recurrence

### Coordinated Disclosure

- We practice **responsible disclosure** and will work with you to coordinate public release
- Security fixes will be deployed before public disclosure whenever possible
- We request a **90-day disclosure window** for critical vulnerabilities
- Credit will be given to researchers who report valid vulnerabilities (unless anonymity is requested)

## Security Measures

This repository implements the following security controls:

### GitHub Security Features

- **Private Vulnerability Reporting**: Enabled for confidential security disclosures
- **Secret Scanning**: Detection of accidentally committed credentials
- **Push Protection**: Prevents commits containing detected secrets
- **Dependency Graph**: Tracks any tooling dependencies
- **Branch Protection**: Main branch requires pull request reviews

### Access Controls

- **Limited Write Access**: Only authorized maintainers can commit directly
- **Code Owners**: Designated reviewers for all media contributions
- **Two-Factor Authentication**: Required for all maintainers with write access
- **Audit Logging**: All repository activities are logged and monitored

### Asset Validation

All media contributions undergo:

- **Format Verification**: Ensure files match declared MIME types
- **Malware Scanning**: Automated scanning for embedded threats
- **Metadata Review**: Inspection for sensitive or unnecessary metadata
- **Size Limits**: Enforcement of maximum file sizes to prevent abuse
- **License Verification**: Confirmation of proper attribution and licensing

### Content Integrity

- **Immutable History**: Git tracking provides full audit trail
- **Hash Verification**: SHA checksums for all committed assets
- **Regular Audits**: Periodic review of all media assets
- **Provenance Tracking**: Documentation of asset sources and creators

## Security Best Practices for Contributors

When contributing media assets:

- **Strip Metadata**: Remove EXIF data, location information, and personal identifiers
- **Use Safe Formats**: Prefer PNG, SVG, WebP over formats with scripting capabilities
- **Optimize Files**: Compress images appropriately to reduce attack surface
- **Verify Sources**: Only contribute assets you created or have permission to use
- **Check Licenses**: Ensure all assets comply with CC BY-SA 4.0 requirements
- **Document Origin**: Provide attribution and source information in commit messages
- **Avoid Executable Content**: No embedded scripts, macros, or active content

## Vulnerability Disclosure Policy

When a vulnerability is confirmed:

1. **Immediate Action**: Affected assets are removed or quarantined
2. **Investigation**: Root cause analysis and impact assessment
3. **Remediation**: Secure replacement assets are prepared
4. **Deployment**: New assets are published to replace vulnerable ones
5. **Notification**: Security advisory is published with details and attribution
6. **Communication**: Relevant parties are notified (sponsors, platform users, security lists)

### Public Disclosure

Security advisories are published at:
- GitHub Security Advisories: [https://github.com/Moebius-Order/moncsdocs-media/security/advisories](https://github.com/Moebius-Order/moncsdocs-media/security/advisories)
- Release Notes: Referenced in relevant version updates
- Website: [https://mcdocs.moebiusorder.com/security](https://mcdocs.moebiusorder.com/security)

## Intellectual Property Protection

This repository contains assets subject to:

- **Copyright**: Original works © 2026 Moebius Order
- **License**: CC BY-SA 4.0 for contributed content
- **Trademarks**: MON CS DOCS and Moebius Order branding

Unauthorized use, modification, or redistribution outside license terms may be subject to takedown:

### DMCA Takedown Process

To report copyright infringement:

1. Submit DMCA notice to [security.mon@moebiusorder.com](mailto:security.mon@moebiusorder.com)
2. Include all required elements per 17 U.S.C. § 512(c)(3)
3. We will review and respond within 5-10 business days

### Counter-Notice Process

If your content was removed:

1. Submit counter-notice to the same email address
2. Provide evidence of authorization or fair use
3. We will review and restore if appropriate

## Hall of Fame

We recognize security researchers who responsibly disclose vulnerabilities:

- This section will list contributors who have helped improve MON CS DOCS media security
- Recognition is provided unless anonymity is requested
- Acknowledgment is included in security advisories and release notes

## Contact

For security-related questions or concerns:

- **Security Team**: [security.mon@moebiusorder.com](mailto:security.mon@moebiusorder.com)
- **General Inquiries**: [mcdocs@moebiusorder.com](mailto:mcdocs@moebiusorder.com)
- **Report Form**: [mcdocs.moebiusorder.com/report](https://mcdocs.moebiusorder.com/report)
- **Community**: [https://t.me/moncsdocs](https://t.me/moncsdocs) (for non-sensitive discussions only)

## Additional Resources

- **Main Repository**: [moncsdocs](https://github.com/Moebius-Order/moncsdocs)
- **Contributing Guidelines**: [CONTRIBUTING.md](CONTRIBUTING.md)
- **License**: [LICENSE](LICENSE)
- **Platform Security**: Infrastructure security managed separately by Moebius Order

---

**Last Updated**: February 28, 2026

© 2026 Moebius Order. This security policy is licensed under CC BY-SA 4.0.
