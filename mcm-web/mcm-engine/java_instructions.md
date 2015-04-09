Get started with mcm-engine
-------------------------------------
This is a starter application for Java with Cloudant NoSQL DB service.

The sample is a Favorites Organizer application, that allows users to organize and manage their favorites and supports different types in each category. This sample demonstrates how to access the Cloudant NoSQL DB service that binds to the application, using Cloudant Java APIs.

1. [Install the cf command-line tool](https://www.ng.bluemix.net/docs/#starters/BuildingWeb.html#install_cf).
2. [Download the starter application package](https://console-classic-20150401-223754.ng.bluemix.net:443/rest/../rest/apps/5c64e00c-aff4-4e82-8972-7db16c56d2f3/starter-download).
3. Extract the package and 'cd' to it.
4. Connect to Bluemix:

		cf api https://api.ng.bluemix.net

5. Log into Bluemix:

		cf login -u amangalv@in.ibm.com
		cf target -o amangalv@in.ibm.com -s ThingsMax
		
6. Compile the JAVA code and generate the war package using ant.
7. Deploy your app:

		cf push mcm-engine -p JavaCloudantDB.war -m 512M

8. Access your app: [mcm-engine.mybluemix.net](http://mcm-engine.mybluemix.net)
