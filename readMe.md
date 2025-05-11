# This is for OCI ATP, Since we are using here Gemini API, "run-sql" action is not available, So we will be writing the code to manually fetch the SQL, Format it and execute it in Database.

1. Make Sure Policy and ACL is created, For step check out file : Prerequestities.md

2. Create AI Profile and use Authentication Key :

Google Gemini
You will need a Google AI Studio account and an API key in order to use Google Gemini.

https://ai.google.dev/  # AI Studio Account
https://aistudio.google.com/app/apikey  #API Key

For more information on other options check : https://apexapps.oracle.com/pls/apex/r/dbpm/livelabs/run-workshop?p210_wid=3831&p210_wec=&session=106018010204687

3. Test the AI profile : refer file : ProfileCreation.sql

4. In our case "run-sql" is not working and According to Oracle's documentation, the supported actions for this function include:

'showsql'
'explainsql'
'narrate'
'chat'
The 'run_sql' action is not among the supported options.

So we will be using custom code to fetch the SQL from API , format it and execute and display the results in Database.

Check DB-AI-SQL_V1 and DB-AI-SQL_V2 for the code.
