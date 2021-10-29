---
title: Data products
---

## Data access

RECCAP2-ocean data products are available at through an FTP server hosted at MPI BGC Jena. The cryptic link to this server was shared internally and is also available upon request from [Jens Daniel Müller](mailto:jensdaniel.mueller@usys.ethz.ch){:target="\_blank"}.

Following two approaches to download files from the FTP server were previously tested:

<u>Download via FileZilla</u>

1.  Paste FTP link in field "Host"

2.  Leave all other fields blank

3.  Click "Quickconnect"

<u>Download via terminal</u>

Use following command:

`wget -bm -nH -nv --cut-dirs=5 -P path_to_download_folder -o path_to_download_folder/YYYYMMDD_download_log.txt --user=ftp --password="email_address" link_to_ftp`

, in which you replace:

`path_to_download_folder`: path to a folder in which to store the downloaded files

`YYYYMMDD`: date of download as label for log file

`link_to_ftp`: cryptic link to FTP server shared internally




## Data Policy

RECCAP2-ocean authors have agreed upon shared principles with respect to data policy, which can be found [here](documents/DATA_POLICY_RECCAP2-ocean.pdf){:target="\_blank"}.
