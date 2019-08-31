# FoodSafe
FoodSafe developed using Blockchain 

Please install Metamask google chrome extension.

Follow the below steps to test the blockchain

Open PowerShell in Administrator Mode
Type "cd %Path Of FoodSafeContract" , E.g. "cd ..\FoodSafe\FoodSafeContract"
Type "truffle compile"
Type "truffle development"
Type "migrate"
Line 14 to 18 can be used for testing the FoodSafe Contract.
var fs
FoodSafe.deployed().then().then(function (retval){fs=retval;}); 
fs.AddNewLocation(1000,"Kissan","Not Secret");   
fs.AddNewLocation(2000,"Sauce","Not Secret");   
fs.GetLocation.call(0).then(function(retval){console.log(retval);}); 
Type "node server.js"
Now open a browser and Type, "http://localhost:3000" ,If everything goes good,This should open something like below, {"contracts":{":FoodSafe":{"assembly":{".code":[{"begin":34,"end":1136,"name":"PUSH","value":"80"}, {"begin":34,"end":1136,"name":"PUSH","value":"40"},{"begin":34,"end":1136,"name":"MSTORE"}, {"begin":281,"end":282,"name":"PUSH","value":"0"},{"begin":264,"end":282,"name":"PUSH","value":"1"}, {"begin":264,"end":282,"name":"PUSH","value":"0"},{"begin":264,"end":282,"name":"PUSH","value":"100"}, {"begin":264,"end":282,"name":"EXP"},{"begin":264,"end":282,"name":"DUP2"},{"begin":264,"end":282,"name":"SLOAD"}, {"begin":264,"end":282,"name":"DUP2"},{"begin":264,"end":282,"name":"PUSH","value":"FF"},{"begin":264,"end":282,"name":"MUL"}, {"begin":264,"end":282,"name":"NOT"},{"begin":264,"end":282,"name":"AND"},{"begin":264,"end":282,"name":"SWAP1"}, {"begin":264,"end":282,"name":"DUP4"},{"begin":264,"end":282,"name":"PUSH","value":"FF"},{"begin":264,"end":282,"name":"AND"}, ...
Now Open another PowerShell terminal.
Type "cd %Path Of FoodSafeClient" , E.g. "cd ..\FoodSafe\FoodSafeClient"
Type npm run start
This will open a browser.
Click on the Metamask extension and sign in using your blockchain Network.
It will prompt to Give access to this site.
Click on "Create New Contract", Metamask popup will open, click on Confirm.
Contract Address will be Auto-populated.
Enter LocationId, LocationName, Secret, Passphrase and click on "Add New Location".
To know the current location, enter the Contract Address and click on "Get the current Location" .
