# WineStoreAngularWebApiProject
BusinessLayer,DataLayer,WebApiLayer,MVC5 Angular2 UI, MSSQL2014, VS2017
Softwares needed - Visual Studio 2017, MSSQLServer 2014
Required installations for Angular 2 - NodeJs 3.6 after, IIS7, EntityFrame work 6
Installation guide : Restore the MSSQL DB .Bak file attached in MSSQL2014 WineStore
* Open the angular solution project from VS 2017 and start setting up the Angular 2 environment.
Set WineStore app as start up project and Index.Html as startup page.
* Need to Host the WebApi Project in IIS7, by publishing it in release mode.
To check Web api works, Just set WebApp project as start up project and run it. Give url as api/wineinfo/findall
JSON result would be displayed.
once it works. rebuild and publish it inorder to host it in IIS7. once files are are there then take your IP config address and paste the APiURL in ANgular project inorder to make it work correctly.

Technologies Used.
C#, MVC5, Angular2, WebApi REST, Entity framework 6, LINQ, 3 Layered architecture Business layer, DataModel layer, WebApi, Angular MVC layer, Visula studio 2017, MSSQLSERVER 2014, Operator Map, Observable pattern try.

Project flow.
* DB WineStore created in MSSQLSERVER 2014
* Visual studio 2017, created entity framework 6 database fist approach, added edmx file to datamodel layer creating entities.
* create business logic layer and create interface inorder to implement loosely coupled architecture.
* Implement LINQ Query to fetch records from DB using Edmx file created datamodel layer by adding namespace in Business logic layer.
* create Web api project to implement GET operation to consume LINQ query implemented by mentioening prefix and required URL in APIcontroller class of web api project. api/wineinfo/findall
* once implementing api project, publish it in IIS7 to make it accessible to angular UI.
* create MVC5 UI framework to consume Webapi to showcase the results.
* firstly, create entity set class, then create service class in typescript file.
* consume the web api URL in service class stype script file.
* Write the component class to invoke service type script and other business logic included in it.
* Design componenet.HTML page as to show case the table view of data fetched from DB.
* Finally register all the service, component, html pages in app.module.ts, and add selector of component to app.component.ts.
* set the winestore as startup project and run making index page start up project

