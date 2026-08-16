# Remediation

## Immediate Remediation

The affected vsFTPd 2.3.4 installation should be removed or upgraded
to a supported, trusted version.

## Service Management

If FTP functionality is not required, the service should be disabled
and removed.

If FTP is required, the organization should use a supported and
properly maintained implementation.

## Network Controls

Access to FTP services should be restricted to authorized networks
and systems.

Firewall rules should prevent unnecessary exposure of FTP services
to untrusted networks.

## Monitoring

Organizations should monitor for:

- Unexpected FTP connections
- Suspicious service activity
- Unexpected processes
- Unauthorized outbound connections
- Changes to critical system files
- Privilege escalation indicators

## Credential Security

Credentials associated with affected services should be rotated when
there is evidence that unauthorized access may have occurred.

## Verification

After remediation:

1. Confirm the vulnerable software version is no longer present.
2. Confirm the FTP service configuration.
3. Verify network exposure.
4. Perform vulnerability validation again.
5. Review system and security logs.
6. Confirm that the previously observed access path is no longer
   available.

## Long-Term Controls

Recommended controls include:

- Software inventory
- Vulnerability management
- Patch management
- Network segmentation
- Least privilege
- Host monitoring
- Centralized logging
- SIEM correlation
- Regular security assessments
