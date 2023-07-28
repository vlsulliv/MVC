# MVC

Model-View-Controller (MVC) 


![models-views-controllers artchitechure](https://www.tutorialspoint.com/mvc_framework/images/model_view_controller.jpg)

Now that we have already created a sample MVC application, let us understand the folder structure of an MVC project. We will create new a MVC project to learn this.

In your Visual Studio, open File → New → Project and select ASP.NET MVC Application. Name it as MVCFolderDemo.


## Controllers Folder
This folder will contain all the Controller classes. MVC requires the name of all the controller files to end with Controller.

In our example, the Controllers folder contains two class files: AccountController and HomeController.

## MVC Controllers
Models Folder
This folder will contain all the Model classes, which are used to work on application data.

In our example, the Models folder contains AccountModels. You can open and look at the code in this file to see how the data model is created for managing accounts in our example.

## MVC Models
Views Folder
This folder stores the HTML files related to application display and user interface. It contains one folder for each controller.

In our example, you will see three sub-folders under Views, namely Account, Home and Shared which contains html files specific to that view area.

## MVC Views
App_Start Folder
This folder contains all the files which are needed during the application load.

For e.g., the RouteConfig file is used to route the incoming URL to the correct Controller and Action.

MVC App Start Folder
Content Folder
This folder contains all the static files, such as css, images, icons, etc.

The Site.css file inside this folder is the default styling that the application applies.

MVC Content Folder
Scripts Folder
This folder stores all the JS files in the project. By default, Visual Studio adds MVC, jQuery and other standard JS libraries.

MVC Scripts Folder

## MVC Framework - Architecture

MVC Flow Diagram

![MVC ](https://www.tutorialspoint.com/mvc_framework/images/mvc_flow.jpg)


Flow Steps

**Step 1** − The client browser sends request to the MVC Application.

**Step 2** − Global.ascx receives this request and performs routing based on the URL of the incoming request using the RouteTable, RouteData, UrlRoutingModule and MvcRouteHandler objects.

**Step 3** − This routing operation calls the appropriate controller and executes it using the IControllerFactory object and MvcHandler object's Execute method.

**Step 4** − The Controller processes the data using Model and invokes the appropriate method using ControllerActionInvoker object

**Step 5** − The processed Model is then passed to the View, which in turn renders the final output.
