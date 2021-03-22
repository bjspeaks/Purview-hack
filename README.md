# Purview-hack

## The different activities that the hack team need to complete are:

#### (complete steps 1 -4 in an hour)
1. Create the Purview Account
2. Create an Azure key vault
3. Create an spn account and store the credentials in the AKV
4. Scanning ADLS, combination of key vault and MI.

#### (complete steps 5-10 in 1.5 hours)
6. Scanning Synapse SQL Pool - using MI.
7. Getting lineage from adf (This will require rerunning the ADF pipeline. Edit the ADF pipeline to shorten the runtime)
8. Adding a custom classification and using it during a scan
9. Bulk upload of glossary and attaching it to the data

Sample Template: https://github.com/tayganr/purviewlab/tree/main/assets

10. ADLS sub-folder scan (scoped scan) - combination of key vault and MSI.

#### (complete step 12 & 13 in 0.5 hours)

11. Add the purview account to Synapse workspace and try to search for files/folders
12. Stretch objective - scan the entire resource group. 




###### Hints: &feature.ext.datasource={"azureSynapse":"true"}
###### SQL Script Hint:

CREATE USER [Purview_MI] FROM EXTERNAL PROVIDER
GO
EXEC sp_addrolemember 'db_owner', [Purview_MI]
GO
