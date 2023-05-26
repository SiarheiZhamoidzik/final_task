# Welcome!

Here is results of DQE Mentoring program final task.
Gol is to implement following checks in accordance with requirements to data:
Flights: Completeness by empty/non empty fields
Flights: Validity by Time Range for DepTime and CRSDepTime
Airports: Uniqueness by PK
FLights: Consistency check for Unique Carrier

final_task.ipynb - jupyter notebook file with results. 
It containts:
- Functions: 
	to_pandas_df_converter() 	- used to read csv or parquet files and convert it into pandas dataframe
	check_for_empy_fields() 	- used to verify completeness by empty/non empty fields
	check_validity_by_range() 	- used to verify validity by Time Range for DepTime and CRSDepTime
	check_uniqueness()			- used to verify uniqueness by PK for Airports
	check_consistency()			- used to verify consistency of Unique Carrier
	check_pk_completeness()		- not required check, which could be used to verify if all PK from src table exist in tgt table

Cells with code of required functions includes example of execution. This examples are done for data requested in task.
Last cell is execution of all these functions for all tables in accordance with requirements.

Check_list.xlsx - file with checklist (required checks are highlighted in bold)

total_result_<date>.xlsx - file with results of execution

script_to_execute_notebook.txt - script to be executed in command prompt to run the notebook. 
Note: in order to execute script on local machine in the same folder with script there should be data for analyses.
Hierarchy of folders should be the following (the same as in bucket):
Data
	source
	raw
		airports
		carriers
		flights
