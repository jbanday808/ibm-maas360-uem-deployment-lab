# Lessons Learned

## Enrollment and policy deployment

- Successful enrollment is the foundation for every other management task.
- A policy must be assigned to the correct device or user before it can take effect.
- New settings may need a device sync and a short wait before they appear.
- Clear policy names make deployment and troubleshooting easier.

![Windows endpoint policy verified](../images/04-MaaS360-Win11-Endpoint-Policy-Verification.png)

## Validate settings on the device

A policy shown as assigned in MaaS360 is only part of the result. The setting should also be checked on the endpoint. In this lab, BitLocker encryption, Windows Defender Firewall, and other security controls were verified directly on the Windows device.

![Endpoint security verified](../images/11-MaaS360-Endpoint-Security-Verified.png)

## Compliance monitoring and remediation

Compliance rules provide a repeatable way to find devices that do not meet security requirements. When a check fails, the administrator should review the reason, correct the setting, sync the device, and confirm that it returns to compliance.

![Compliance baseline verified](../images/15-MaaS360-Compliance-Baseline-Verified.png)

## Mobile management takeaways

- **Android:** Android Enterprise and Managed Google Play provide the modern approach for managing work devices and approved apps. Company-owned devices should use Device Owner enrollment instead of the older Device Admin method.
- **iOS:** Enrollment profiles, security policies, managed apps, and VPN settings work together. Apple management certificates must remain current for reliable communication.

| Android Enterprise connected | iOS VPN policy applied |
|---|---|
| ![Android Enterprise connected](../images/17-MaaS360-Android-Enterprise-Connected.png) | ![Cisco AnyConnect VPN policy applied](../images/20-MaaS360-iOS-Cisco-AnyConnect-VPN-Policy-Applied.png) |

## Troubleshooting lessons

1. Confirm that the device is enrolled, online, and recently synced.
2. Check that the correct policy is assigned to the correct platform.
3. Review the device record for a failed rule or status message.
4. Verify basic requirements such as internet access, supported software, and current certificates.
5. Make one change at a time, sync again, and record the result.

## Security best practices

- Start with a clear minimum-security baseline.
- Require encryption, a strong passcode, and an active firewall where supported.
- Use supported enrollment methods and keep operating systems current.
- Give devices and users only the access they need.
- Protect recovery keys and administrative accounts.
- Test policies on a small group before wider deployment.
- Confirm important settings in both MaaS360 and on the device.

## Final takeaway

This lab showed that endpoint management is not only about creating policies. Reliable results come from careful enrollment, clear assignments, device-level validation, ongoing compliance checks, and documented troubleshooting.

> **Lab note:** These lessons came from an isolated learning environment. Production policies should be reviewed, tested, and approved for the needs of the organization.

[Return to the documentation index](README.md)

