Ionic Cordova installation:
---------------------------
---------------------------
	. First we need to install npm Node.js package manager https://nodejs.org/en/ : Check this link for the download.
	. Then in cmd Command Line give npm install -g ionic cordova   ----> 'g' means globally.
	. Then to create a project give this, ionic start MyFirstApp(ProjectName) ----> you can specify like this to create a project -- OR -- you can
		also specify how the project should look like default. Like Should it be blank or tab or sidememu or tutorial ? For this it should be like this
		ionic start MyFirstApp blank
	. 





Page Lifecycle:
---------------
----------------

	. ionViewCanEnter       Navigation Guard => Should the page be loaded?
	. ionViewDidLoad		Page has loaded; Not fired when cached => Setup Code for Page
	. ionViewWillEnter		Page is about to enter and become active Page
	. ionViewDidEnter		Page has fully entered and now is active Page; Also fired when cached
	. ionViewCanLeave		Navigation Guard => May the Page be left?
	. ionViewWillLeave		Page is about to leave and become inactive
	. ionViewDidLeave		Page finished leaving and is no inactive
	. ionViewWillUnload		Page is about to be destroyed(not cached anymore)
	

Navigation between pages:
-------------------------
-------------------------

	There are two ways navigating between pages.
		1. By using navCtrl to push to the respective page.
		2. By adding class name of the other page in a variable and in html just add [navPush] = 'usrPage' (<----- variable name defined in the class ---- ) in the button instead of click attribute.