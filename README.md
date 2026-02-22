# WM_Project_Documentation

# Customer Portal page
-Any customer who gets onboarded to Acorn to customer portal
-Portal helps Acorn to feed the data
-We can see dashboards data for analytics
-SELECT * FROM UAT_ELEMENT.ELEMENTS.TBL_DSH_RPT_BILL_ACCRUAL_DATA --Actual Final value data This is the major table pointing to dashboard 

SBS Stands for "Strategic Buisness Elements"

=> These are fields that we have to fill in order to get information about data
-CLient ID
-Client Name
-Client Type
-Status
-Email
 
=>Which Data present Where   
Acorn                        Scehma             DM           INT                sql server
Dashboard -> SP-> Flatten -> Billable         fct_billable  Billable_component  Acorn
                             Accrual Data     Fct_accrual   accrual_component
          
=>Similarly MAS have same flow


# Dimension table data :
-dim_derived_service_type
-dim_equipment
-dim_material 
-dim_disposal_site
-dim_client  
-dim_client_location                    

Note:
The things that your doing in tools or changing data, we have to maintain the record for that

# Location Management Screen:
-RMT Location Creation
-Location Merge Process
-Location Split process
-Default Merge Process

=>Merge Only when location_id and location_code are same 

=>Centrally build and Locally build are national customers
Market Area customer are locally customer


#S3 Data 
there are three buckets where data is loaded into Snowflake
1)eadm-elements-thumbnails-dev(image related data)
2)eadm-sbselements-dev(This folder for main data)
3)elements-s3



Fastlane is holding land fills data
it has its own billing system,billing is happening in MAS. Hence, MAS has its billing data  
