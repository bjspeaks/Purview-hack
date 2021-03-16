# Purview-hack

## The different activities that the hack team need to complete are:

1. Setup a purview account
2. create an Azure key vault
3. create an spn account and store the credentials in the AKV
4. scanning ADLS, combination of key vault and MI.
5. Scanning Synapse SQL Pool - using MI.
6. Getting lineage from adf (This will require rerunning the ADF pipeline. Edit the ADF pipeline to shorten the runtime)
7. Adding a custom classification and using it during a scan
8. Bulk impupload of glossary and attaching it to the data
9. Synapse Table scan - combination of key vault and MI.
10. Stretch objective - scan the entire resource group. 





# Hints: &feature.ext.datasource={"azureSynapse":"true"}
