# README #

### springML Inc Repository ###

Google Dataflow Jobs
--------------------


Following two classes take care of Google cloud dataflow jobs

SFReferenceDataJob - Will fetch the reference data from SF (Oppurtunity) and populate bigQuery
AdDataJob - Will fetch the raw data from GCS and SF reference data from bigquery. Enrich the data and populate bigQuery with the enriched data


SFReferenceDataJob
------------------

This requires the following inputs

1. Google cloud project
2. Google cloud Staging location
3. BigQuery output table
4. SF UserId 
5. SF Password

On completion of the job, bigquery table SFDCReferenceData.SFRef will be populated with SF Reference data


AdDataJob
---------

This requires the following inputs

1. Google cloud project 
2. Google cloud Staging location
3. Ad Raw data (CSV)
4. BigQuery Reference data table
5. BigQuery output table

On completion of the job bigquery table SFDCReferenceData.EnrichedSample will be populated withenriched data.





