---
title: Error after logging in to the Commerce Admin
description: This article provides a solution for the issue where you receive an error message saying that the requested URL was not found on this server.
exl-id: f52b383b-87f2-4216-9bf4-e765db31ca6b
feature: Admin Workspace
role: Developer
---
# Error after logging in to the Commerce Admin

This article provides a solution for the issue where you receive an error message saying that the requested URL was not found on this server.

## Details

The requested URL /magento2index.php/admin/admin/dashboard/index/key/0c81957145a968b697c32a846598dc2e/ was not found on this server.

Note the lack of a slash character between `magento2` and `index.php` in the URL.

## Solution

The base URL is not correct. The base URL must:

* Start with `http://` or `https://`
* End with a slash ( `/` )
* Match the case of the `web/unsecure/base_url` record in the `core_config_data` database table

Re-run the installation using a valid value.

## Related reading

[Best practices for modifying database tables](https://experienceleague.adobe.com/en/docs/commerce-operations/implementation-playbook/best-practices/development/modifying-core-and-third-party-tables#why-adobe-recommends-avoiding-modifications) in the Commerce Implementation Playbook
