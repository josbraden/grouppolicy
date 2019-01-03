# GroupPolicy

A repo for Group Policy related stuff.

Installers are included if you want to install the ADMX files yourself. Otherwise, the ADMX and ADML files are located in the PolicyDefinitions directory, which is ready to be used as a central store.

## Creating the Central Store

From Microsoft: https://support.microsoft.com/en-us/help/3087759/how-to-create-and-manage-the-central-store-for-group-policy-administra

To take advantage of the benefits of .admx files, you must create a Central Store in the SYSVOL folder on a Windows domain controller. The Central Store is a file location that is checked by the Group Policy tools by default. The Group Policy tools use all .admx files that are in the Central Store. The files that are in the Central Store are replicated to all domain controllers in the domain.

To create a Central Store for .admx and .adml files, create a new folder that is named PolicyDefinitions in the following location (for example) on the domain controller:

\\contoso.com\SYSVOL\contoso.com\policies\PolicyDefinitions
