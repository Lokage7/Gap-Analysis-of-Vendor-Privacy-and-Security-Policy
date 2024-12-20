# Gap Analysis of Vendor Privacy and Security Policy

## Overview
This repository documents the project to perform a gap analysis on Best Buy's Information Security Policy. The objective was to ensure alignment with PCI DSS 4.0 requirements.

## Key Findings
### **Compliant Controls**
- **Data Retention**: Data rendered unrecoverable (Requirement 9.4.6).
- **Third-Party Audits**: TPSPs reviewed annually (Requirement 12.8.4).
- **Encryption**:
  - In-Transit: TLS 1.2 secure (Requirement 4.2.1).
  - At Rest: 128-bit key strength (Requirement 3.5).
- **Incident Response**: IR plan reviewed annually (Requirements 12.10.1, 12.10.2).

### **Non-Compliant Controls**
- **Vulnerability Scanning**: Internal and external scans not conducted quarterly (Requirements 11.3.1, 11.3.2).
- **Patching**: Critical patches not implemented within 30 days (Requirement 6.3.3).
- **Weak Protocols**: Weak protocols not fully mitigated (Requirement 1.2.6).

### **Detailed Gap Table**

| **Requirement**    | **Control**                          | **Status**      | **Comments**                                       |
|---------------------|--------------------------------------|-----------------|---------------------------------------------------|
| 6.3.3              | Critical Patching                   | Non-Compliant   | Patches not implemented within 30 days.          |
| 11.3.1, 11.3.2     | Vulnerability Scans (Internal/Ext.) | Non-Compliant   | Not conducted quarterly.                         |
| 1.2.6              | Weak Protocol Mitigation            | Non-Compliant   | Weak protocols require additional mitigation.    |

# Recommendations

## Critical Recommendations
1. **Implement Quarterly Vulnerability Scans** (Requirements 11.3.1, 11.3.2)
   - Schedule scans every three months.
   - Assign responsibility to the IT Security Team.

2. **Enhance Patching Process** (Requirement 6.3.3)
   - Implement a policy for critical patches within 30 days of release.
   - Track patching progress with automated tools.

3. **Mitigate Weak Protocols** (Requirement 1.2.6)
   - Update configurations to disable weak protocols.
   - Conduct periodic protocol reviews.

## Additional Recommendations
- Clarify processes for rendering data unrecoverable (Requirement 9.4.6).
- Maintain logs of all pentesting and vulnerability scans for audit purposes.

## Conclusion
Overall, the Vendor Privacy and Security Policy is well-aligned with PCI DSS 4.0, with a few gaps requiring immediate attention.

## Key Highlights
- Framework: PCI DSS 4.0
- Scope: Access control, data protection, incident response, and third-party management
- Tools: Google Docs


