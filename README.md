# Purview-hack

## The different activities that the hack team need to complete are:

1. Create the Purview Account
2. Create an Azure key vault
3. Create an spn account and store the credentials in the AKV
4. Scanning ADLS, combination of key vault and MI.
5. Scanning Synapse SQL Pool - using MI.
6. Getting lineage from adf (This will require rerunning the ADF pipeline. Edit the ADF pipeline to shorten the runtime)
7. Adding a custom classification and using it during a scan
8. Bulk upload of glossary and attaching it to the data
9. ADLS sub-folder scan (scoped scan) - combination of key vault and MSI.
10. Add the purview account to Synapse workspace and try to search for files/folders
11. Stretch objective - scan the entire resource group. 





### Hints: &feature.ext.datasource={"azureSynapse":"true"}
### SQL Script Hint:

CREATE USER [Purview_MI] FROM EXTERNAL PROVIDER
GO
EXEC sp_addrolemember 'db_owner', [Purview_MI]
GO
