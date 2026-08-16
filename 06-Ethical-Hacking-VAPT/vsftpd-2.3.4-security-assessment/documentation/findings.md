# Findings

## Finding F-001 — Remote Code Execution / Unauthorized System Access

### Severity

**Critical**

### Affected Service

- Service: FTP
- Software: vsFTPd
- Version: 2.3.4
- Environment: Isolated cybersecurity laboratory

### Finding Summary

The laboratory target was running vsFTPd 2.3.4, a version associated
with a known backdoor vulnerability.

The vulnerability was successfully validated within the authorized
laboratory environment.

### Validation Result

The security testing process resulted in a Meterpreter session on the
target system.

The obtained session was subsequently assessed and determined to have
root-level privileges.

### Access Obtained

The validated access provided a high level of control over the
laboratory target.

Root-level access represents the highest local privilege level on a
typical Linux system and demonstrates significant potential impact if
the same weakness were present on an exposed production system.

### Security Impact

Successful exploitation of this weakness could potentially allow an
attacker to:

- Execute unauthorized commands.
- Access files available to the compromised privilege level.
- Modify system configuration.
- Disrupt services.
- Establish additional unauthorized access.
- Compromise the confidentiality, integrity, and availability of
  the affected system.

### Evidence

Evidence supporting this finding will be added to the repository
after review and sanitization.

### Detection Opportunities

Potential detection sources include:

- FTP service logs
- Network monitoring
- Unexpected outbound connections
- Unexpected processes
- Authentication and service activity
- Host-based security monitoring
- SIEM correlation

### Remediation

The vulnerable vsFTPd version should be removed or upgraded to a
supported and secure version.

Additional remediation recommendations will be documented separately.

### Lab Limitation

This finding was validated only against an intentionally vulnerable
system within an isolated laboratory environment.

No production or third-party systems were targeted.
