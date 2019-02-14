# OpioidDataMigration
Data Staging/Migration/Archiving/Auditing Using SSIS ForEach Loop Container

The assignment requires taking data about opioid presciptions and claims according to state in the form of Excel files, loading them into a staging area, moving it to a destination table in the timestamp of load date attached, and finally moving the data to an archive area.

The files in the zip consists of the following:

- CreateDatabaseAndStagingTable_2.sql
This is the first sql run to create a database and all the necessary tables.

- Opioid_StagingWarehousingArchiving.dtsx

This is the SSIS project package which holds the control flow, which first runs the above file, reads the excel source files in a ForEach Loop and loads the data into staging and archiving area tables, and stores metadata in an audit table.

- h4_Toad_model.txp

A pictoial description of the dataflow done with Toad Data Modeler 

- hw4_Explanation.docx

More explanations with annotated screenshot that descibe the entire project
