# avr-asp-net-01-basic-app

#1 Exercise: AVR ASP.NET ASNA Web programming

This is the #1 exercise using ASNA Visual RPG for ASP.NET WebForms programming. 

```
.\
├── App_Code\
│   └── StateHelpers.vr
│
├── public\
│   │
│   ├── css\
│   │   └── global.css
│   └── js\
│       └── applib.js
│
├── views\
│   ├── customer-form.aspx
│   ├── customer-form.aspx.vr
│   ├── customer-number.aspx
│   └── customer-number.aspx.vr
│
├── .gitignore
├── 01-basic-app.sln
├── Global.asax
├── MasterPageNav.master
├── MasterPageNav.master.vr
├── README.md
├── Web.config
└── Web.Debug.config
```

## 1. Basic app

This is a note about this node.


### Visual Studio

- windows in Visual Studio 

  ### Solution Explorer
  The `Solution Explorer` is the "dashboard" of Visual Studio. Use to  navigate to project files.
  
  ### Properties window
  The `Properties` window shows properties for ASP.NET controls.
  
  ### Output window
  The `Output` window shows build errors.
  
  ### Source window (design/source for ASPX pages)
  The `Source` window is where you edit source code or display markup.
  
  ### DataGate Explorer
  The `DataGate Explorer` lets you view and work with DataGate data.
  
- Solution Explorer

  The Solution Explorer is the "dashboard" of Visual Studio. Use to  navigate to project files.
  
- VS settings

	- Suggested project settings

		- use output window only

		  Set VS to not show Error window and always show Output window when build starts. See the red and green check boxes.
		  
		  [Show image](https://asna-assets.nyc3.cdn.digitaloceanspaces.com/images/asp-net-training/vs-prog-sol-general-settings.png)
		  
		- set default projects location
		
		  [Show image](https://asna-assets.nyc3.cdn.digitaloceanspaces.com/images/asp-net-training/visual-studio-projects-default-location.png)
		  
	
- Set the start page

### Project folders

- root

	- Global.asax

	  This file provides global event handlers. These are events that happen at top-level of the application. For example, there is a global event (Application_Error) that you can use to provide global error handling. 
	  
	  There is also one (Application_Start) that fires when the first user  starts using the app. 
	  
	- asp-net-project-starter.sln

	  This is the project's solution file. I always tell Visual Studio to put them in the same directory as the project
	  
	  Details on projects and solutions:
	  https://learn.microsoft.com/en-us/visualstudio/ide/solutions-and-projects-in-visual-studio?view=vs-2022
	  
	- web.config

	  Project configuration information. 
	  
	- web.debug.config

	  Project configuration to use at deployment.
	  
	- .gitignore

	  A Git-related file that can be ignored/deleted if you aren't using Git.
	  
	- README.md
	- MasterPageNav.master

	  Master pages make it easy to provide consistent look and feel to your app's pages.
	
- app_code

	- StateHelpers.vr

	  This file provides a class with helper members for accessing Session and Application state variables. Using this file is optional, but it is very helpful. It's also a good little example of moving logic out of the code-behind.
	
- error-logs

  This folder isn't used in this branch. However, it needs to be for source control purposes. In a different branch, we'll see that this is the folder to which error messages are logged.
  
- public

  In many Web frameworks, the 'public' folder is where public-facing application assets (such as images, CSS, and JavaScript) are stored. With ASP.NET, you can name the assets folder anything you want. 
  
	- css

	  The various branches of this ASNA class project all use BootStrap 5 as their CSS framework. For these classroom projects, Boostrap is pulled in from a CDN (the link to the Bootstrap CSS is in the 'MasterPageNav.master' file).
	  
	  That CDN link isn't a good link to use for production work. See the Bootstrap docs for more information on BootStrap. 
	  
	  
		- global.css

		  Even when you use a custom CSS framework, your app generally needs a little custom CSS. This app's custom CSS is in 'global.css'.
		
	- js

		- applib.js

		  ASP.NET's checkbox and radio button controls don't work directly with Bootstrap CSS. 'applib.js' is a JavaScript file that fixes that issue and lets Bootstrap naturally style checkboxes and radio buttons.
	
- views

	- customer-form.aspx

	  A WebForm that lets the user enter a customer number to update.
	  
	- customer-number.aspx

	  A WebForm that lets a user update a customer.
	  
### Topics

- HTTP Request/Response

	- show post to https://httpbin.org/post

- [Paster pages](https://learn.microsoft.com/en-us/previous-versions/aspnet/wtxbf3hh(v=vs.100))

- [Postback](https://learn.microsoft.com/en-us/dotnet/api/system.web.ui.page.ispostback?view=netframework-4.8.1)

	- IsPostBack

- [State management](https://www.c-sharpcorner.com/UploadFile/b926a6/state-management-concept-in-Asp-Net/)

	- Application
	- Session
	- ViewState

- AVR

  [This page](https://asna.com/en/kb/getting-to-know-asna-visual-rpg/) provides a quick introduction to ASNA Visual RPG (AVR) syntax.
  
  [This is a list](https://asna.com/en/tag/visual-rpg/) of ASNA Visual RPG articles at ASNA.com.
  
	- Data types
	- Functions
	- CL + RPG

