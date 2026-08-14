# Signing Up for an IBM MaaS360 Free Trial

## Start the free trial

1. Open IBM's [MaaS360 free-trial page](https://www.ibm.com/products/maas360/resources).
2. Select **Start your 30-day trial** and sign in with an existing IBMid or create one.
3. Enter the requested contact and organization details, accept the trial terms, and submit the form.
4. Open the welcome email from IBM and save it. It contains important account and sign-in information.
5. Follow the supplied link, sign in, and replace any temporary password when prompted.

IBM currently describes the offer as a 30-day trial. The form and available features may change over time.

## Basic account and MFA setup

Use a clear organization name and an email account that will remain available throughout the lab. Store the account name, administrator username, and portal link securely.

Protect the IBMid with multi-factor authentication (MFA). From the IBM profile, open **ID and password**, choose the authenticator or TOTP option, and scan the displayed QR code with IBM Verify or another supported authenticator app. Enter the generated code to confirm setup. A backup sign-in method helps prevent lockout. See IBM's [IBMid MFA guidance](https://www.ibm.com/support/pages/how-enable-multi-factor-authentication-ibmid).

## Quick Start options

The first MaaS360 sign-in opens the **Quick Start** wizard. It can guide the administrator through:

- Apple enrollment
- Android Enterprise
- Security policies
- Corporate email
- Device enrollment

A step can be skipped and resumed later from the portal home page. IBM provides a full [Quick Start overview](https://www.ibm.com/docs/en/maas360?topic=portal-configuring-quick-start-first-time).

![MaaS360 cloud administration flow](../images/IBM-MaaS360-cloud-admin-diagram.png)

## Initial security policy

Quick Start offers **Basic**, **Intermediate**, and **Strict** security levels, or the option to configure a policy later. For a lab, begin with the level that matches the test goal, review its settings, and test it on one device before wider use. Policies can be edited later from **Security > Policies**. IBM explains the [Quick Start security levels](https://www.ibm.com/docs/en/maas360?topic=time-selecting-security-policies-from-quick-start).

## Accessing the Admin Portal

Use the login link in the welcome email and sign in with the IBMid, password, and MFA method. After Quick Start, the MaaS360 Admin Portal provides access to devices, users, security policies, apps, reports, and setup options.

![MaaS360 Admin Portal setup view](../images/17-MaaS360-Android-Enterprise-Connected.png)

## Key takeaway

The trial setup creates the administrator account, protects access with MFA, and uses Quick Start to prepare the first device-management and security choices. Save the welcome email and test policies carefully before enrolling additional devices.

> **Lab note:** No signup or MFA screenshots are stored in this repository. The images above show the lab's cloud administration flow and the MaaS360 portal after setup. Trial availability, screens, and options can vary by region and date.

[Return to the documentation index](README.md)

