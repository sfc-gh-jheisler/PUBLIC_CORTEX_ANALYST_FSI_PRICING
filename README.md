# PUBLIC_CORTEX_ANALYST_FSI_PRICING
PUBLIC_CORTEX_ANALYST_FSI_PRICING

## Access Data from Snowflake Marketplace
Follow below instructions to get the FactSet Tick History data from Snowflake Marketplace.

1) Navigate to Snowsight
2) Click: Data Products
3) Click: Marketplace
4) Search: FactSet Tick History
5) Scroll Down and Click: Tick History
6) Click: Get
7) Make sure the Database name is: tick_history
8) Which roles, in addition to ACCOUNTADMIN, can access this database? PUBLIC
9) Click: Get

## Set Up Environment
run the SET_UP_SQL.sql script to create the objects necessary for our demo.

## Upload Semantic Model
Upload the th_sf_mktplace.yaml file to the stage following these steps: https://docs.snowflake.com/en/user-guide/data-load-local-file-system-stage-ui#upload-files-onto-a-named-internal-stage

1) Sign in to Snowsight.
2) Select Data » Add Data.
3) On the Add Data page, select Load files into a Stage.
4) In the Upload Your Files dialog that appears, select the files that you want to upload. You can upload multiple files at the same time.
5) Select the database schema in which you created the stage, then select the stage.
6) Optionally, select or create a path where you want to save your files within the stage.
7) Select Upload.

## Create a Streamlit Application
Follow these steps to create our base application: https://docs.snowflake.com/en/developer-guide/streamlit/create-streamlit-ui#create-a-streamlit-app-by-using-sf-web-interface

1) Sign in to Snowsight.
2) In the left navigation bar, select Projects » Streamlit.
3) Select + Streamlit.
4) The Create Streamlit App window opens.
5) Enter a name for your app.
6) In the Warehouse dropdown, select the warehouse where you want to run your app and execute queries.
7) In the App location dropdown, select the database and schema for your app.
8) Select Create.
9) Delete the python in the editor pane and copy and past the python from sis_application.py.
10) Click run in top right
