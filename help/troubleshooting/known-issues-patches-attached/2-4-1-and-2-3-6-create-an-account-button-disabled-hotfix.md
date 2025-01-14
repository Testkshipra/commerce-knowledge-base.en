---
title: Adobe Commerce 2.4.1 and 2.3.6 create an account button disabled hotfix
description: This article provides a hotfix for the issue when you struggle to create a new account after inputting an incorrect value to any field on the form. For example, when you enter an email address in the wrong format or leave the first name or last name fields empty or do not enter a value that meets password requirements. A permanent fix will be included in the Q1 releases (2.4.2, 2.4.1-p1, and 2.3.6-p1).
exl-id: e6e65ede-8156-4e2b-b369-b18395bb3dbf
feature: Customer Service
role: Developer
---
# Adobe Commerce 2.4.1 and 2.3.6 create an account button disabled hotfix

This article provides a hotfix for the issue when you struggle to create a new account after inputting an incorrect value to any field on the form. For example, when you enter an email address in the wrong format or leave the first name or last name fields empty or do not enter a value that meets password requirements. A permanent fix will be included in the Q1 releases (2.4.2, 2.4.1-p1, and 2.3.6-p1).

## Issue

The **Create an Account** button on the **Create New Account** page remains disabled if a shopper has entered invalid data. This prevents shoppers from re-attempting to create an account after making an error.

<u>Steps to reproduce</u>:

1. Go to **Create New Customer Account**.
1. Fill in the form fields. In the **Password** field, input values that do not meet the password requirements. For example:
    * The passwords in the **Password** and the **Confirm Password** fields do not match.
    * The passwords in the **Password** and the **Confirm Password** fields are not long enough.
1. Click the **Create an Account** button.

<u>Expected results</u>:

* **Create an Account** button should stay active/enabled.
* The user should be able to create a new account.

<u>Actual results</u>:

* **Create an Account** button stays disabled, even after filling in all required fields with valid/correct data.
* The customer is not able to create a new account.

## Patch

The patch is attached to this article. To download it, scroll down to the end of the article and click the file name or click the following link: [Download MC-38509-composer.patch](assets/MC-38509-composer.patch.zip)

## Compatible Adobe Commerce versions:

The patch was created for:

* Adobe Commerce on cloud infrastructre 2.3.6 and 2.4.1.
* Adobe Commerce on-premises 2.3.6 and 2.4.1.

The patch is not compatible with any other Adobe Commerce versions and editions.

## How to Apply the Patch

See [How to apply a composer patch provided by Adobe](/help/how-to/general/how-to-apply-a-composer-patch-provided-by-magento.md) for instructions.

## Related reading

* [GitHub Adobe Commerce  > Submitting invalid create account form leaves the submit button disabled](https://github.com/magento/magento2/issues/30513)
* [Adobe Commerce User Guide > Getting Started > Creating an Account](https://experienceleague.adobe.com/en/docs/commerce-admin/start/commerce-account/commerce-account-create)
