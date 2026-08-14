# MaaS360 Troubleshooting Guide

## Start with four basic steps

1. **Identify:** Read the device status or error and note what is failing.
2. **Fix:** Correct the enrollment, policy, security setting, or app configuration.
3. **Refresh:** Sync the device and allow time for MaaS360 to receive the update.
4. **Verify:** Check the result in MaaS360 and directly on the device.

## Common enrollment problems

If a device does not enroll, confirm that it has internet access, the enrollment request is still valid, and the correct user and platform were selected. Remove an incomplete management profile before retrying. Company-owned Android Device Owner enrollment normally requires a new or factory-reset device.

![Windows 11 MDM enrollment](../images/02-MaaS360-Win11-MDM-Enrollment.png)

## Policy not applying

- Confirm that the device is enrolled, online, and recently synced.
- Check that the correct policy is published and assigned to the device or user.
- Make sure the setting is supported by the device, OS version, and ownership type.
- Sync again, wait briefly, and verify the setting on the device.

![Windows endpoint policy verified](../images/04-MaaS360-Win11-Endpoint-Policy-Verification.png)

## Device showing non-compliant

Open the device's compliance details and identify the failed rule. Correct the issue—for example, restore enrollment, update the OS, or enable encryption. Sync the device and confirm that MaaS360 changes the status back to compliant.

![Compliance baseline verified](../images/15-MaaS360-Compliance-Baseline-Verified.png)

## BitLocker or firewall status issues

- Confirm that the Windows edition and device support the required security feature.
- Check BitLocker encryption and Windows Defender Firewall directly on the endpoint.
- Confirm that the related MaaS360 policy is assigned and has reached the device.
- Restart or sync the test device if its reported status is outdated.
- Protect the BitLocker recovery key and verify that it is available before making changes.

| BitLocker verified | Firewall verified |
|---|---|
| ![BitLocker fully encrypted](../images/06-MaaS360-BitLocker-Fully-Encrypted.png) | ![Firewall service running](../images/10-MaaS360-Firewall-Service-Running.png) |

## Android 14 enrollment error

The lab encountered an issue with the older **Device Admin** enrollment method on Android 14. Newer Android devices should use **Android Enterprise**. For a company-owned device, use Device Owner enrollment and begin during initial setup; a factory reset may be required. Also confirm that Managed Google Play shows as connected in MaaS360.

![Android Enterprise connected](../images/17-MaaS360-Android-Enterprise-Connected.png)

## Cisco Secure Client / VPN issues

- Confirm that Cisco Secure Client was added and assigned to the iOS device.
- Check that the VPN policy uses the correct app and connection details.
- Confirm that the management profile remains installed and the device can sync.
- Verify that the VPN server address and required certificates or sign-in details are correct.
- Test the connection on the device; an assigned policy alone does not prove that the VPN is reachable.

![Cisco AnyConnect VPN policy applied](../images/20-MaaS360-iOS-Cisco-AnyConnect-VPN-Policy-Applied.png)

## Final takeaway

Troubleshooting is most reliable when one issue is changed at a time. Record the original error, apply a focused fix, refresh the device, and verify the result in both MaaS360 and on the endpoint.

> **Lab note:** This guide reflects an isolated learning environment. Production changes should follow the organization's testing, approval, and recovery procedures.

[Return to the documentation index](README.md)

