---
title: How to create a "scrubbed" dump when requested by support agent
description: This article provides information on how to create a "scrubbed" dump (backup) of your database and code from the Adobe Commerce Admin when requested to provide one by an Adobe Commerce support agent. This dump excludes your media files to speed up the process and to result in a much smaller file. All sensitive data is hashed when making the database backup.
exl-id: ad088bd2-3f92-416e-89f0-d037d53cd6a9
---
# How to create a "scrubbed" dump when requested by support agent


## Affected products and versions

Adobe Commerce (all deployment methods) 2.3.x, 2.4.x.

## Create a "scrubbed" dump

Create a "scrubbed" dump from the Admin:

1. In the Commerce Admin, go to **System** > **Support** > **Data Collector**.
1. Click **New Backup**.
1. After a few minutes, click **Refresh Status** (may take longer, repeat every 5 minutes until completed).
1. Relocate the generated dump files from the `/var/support` directory to the Adobe Commerce root directory.

You can then provide to Support the direct download link to the dump files (your store address and the file name as displayed).

If you have issues creating dumps from the Admin, consider using CLI commands as described in [Run the support utilities](https://experienceleague.adobe.com/en/docs/commerce-operations/configuration-guide/cli/run-support-utilities) in our developer documentation.

## Related reading

* [Create full database backup for Adobe Commerce on cloud infrastructure](/help/how-to/general/create-database-dump-on-cloud.md) in our support knowledge base.
