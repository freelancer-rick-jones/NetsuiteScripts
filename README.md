# NetsuiteScripts
Random Netsuite Scripts from various setups, deployments and updates.<br/>
<br/>
Files: <br/>
SuiteScript Version 1.0:<br/>
<b>DD_Restlet.js</b> - A simple restlet that takes a URL, opens it, gathers the data in text format and returns it the body of the url back as text. Primarily used to get JSON from an API endpoint.<br/>
<b>Data_All_Scripts_Transfer.js</b> - This scheduled script handles the incoming data from in json/application format. The data is processed here to be placed into a custom record (customrecord_dd_update), filtering by inactivating the fields you dont wish to update using the map variable below. Due to Netsuites Governancing of how many iterations you can provide, multiple calls to the script are required until its completed. With this in mind, scripts are checked repeatedly for governance compliance and rescheduling the scripts completed.<br/>
<b>Data_conversion_script_reworked.js</b> - Conversion only script already in Data_All_Scripts_Transfer.js<br/>
<br/>
SuiteScript Version 2.x:<br/>
<b>Export_List_UE_IF_Loader.js</b> - UE Script Item Fulfilment data search and display
