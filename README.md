#MavensMate for Sublime Text

## Development Suspended

MavensMate users, 

I have temporarily suspended development & support for MavensMate to focus on spending time with my newborn daughter. If you are experiencing an issue with MavensMate, I encourage you to use the Force.com IDE, Developer Console, or one of the many other 3rd party tools for building Salesforce applications until development resumes.

Thanks very much for your support.

-Joe


MavensMate for Sublime Text is a plugin that aims to replicate the functionality of the Eclipse-based Force.com IDE. Its goal is to allow developers to work inside Sublime Text for all their Force.com-related tasks.

* Create & Edit Salesforce.com projects with specific package metadata
* Create & compile Apex Classes, Apex Trigger, Visualforce Pages, Visualforce Components
* Create & Edit Lightning Components (v7 only)
* Retrieve & compile other types of Salesforce.com metadata
* Run Apex test methods and visualize test successes/failures & coverage
* Deploy metadata to other Salesforce.com orgs
* Apex Execute Anonymous
* Create Apex Execution Overlay Actions "checkpoints" (tooling API)
* Stream Apex Logs to your local filesystem
* Apex & Visualforce Code Assist

####For detailed information and documentation, please visit [mavensmate.com][mmcom]

##Install

### Version 6 [stable]

**You must install the following before continuing:**

1. Sublime Text 3 [http://www.sublimetext.com/3](http://www.sublimetext.com/3)
2. Sublime Text Package Control [https://packagecontrol.io/installation](https://packagecontrol.io/installation)

**IMPORTANT NOTE:** If you do NOT wish to have Package Control automatically update MavensMate to the v7 betas, you MUST ensure your Package Control user settings do not have "MavensMate" listed in the "install_prereleases" setting.

####Installing the MavensMate for Sublime Text package

1. Open Sublime Text 3
2. Run `Package Control: Install Package` command
	- [Running commands from Sublime Text](http://docs.sublimetext.info/en/latest/extensibility/command_palette.html)
3. Search for `MavensMate`
4. Hit `Enter`

### Version 7 [prerelease channel]

**You must install the following before continuing:**

1. Sublime Text 3 [http://www.sublimetext.com/3](http://www.sublimetext.com/3)
2. Sublime Text Package Control [https://packagecontrol.io/installation](https://packagecontrol.io/installation)
3. MavensMate-app **(must be running in order for MavensMate for Sublime Text v7.0+ to function)** [https://github.com/joeferraro/mavensmate-app/releases](https://github.com/joeferraro/mavensmate-app/releases)

**IMPORTANT NOTE:** In order to install the v7 betas, you must add `"MavensMate"` to your Package Control `"install_prereleases"` user setting, see below:

![screen shot 2015-09-02 at 9 10 17 am](https://cloud.githubusercontent.com/assets/54157/9632003/79242b02-5152-11e5-8672-d91bb549cee6.png)
![package_control_sublime-settings_ _df15-react-communities-ios](https://cloud.githubusercontent.com/assets/54157/9632015/8cf6d800-5152-11e5-925e-627995a4aef5.png)
![screen shot 2015-10-12 at 12 53 39 pm](https://cloud.githubusercontent.com/assets/54157/10433499/557e5134-70e0-11e5-81e5-8910ad6cdd68.png)

#### Installing the MavensMate for Sublime Text package

1. Open Sublime Text 3
2. Run `Package Control: Install Package` command
	- [Running commands from Sublime Text](http://docs.sublimetext.info/en/latest/extensibility/command_palette.html)
3. Search for `MavensMate`
4. Hit `Enter`

### Setup

In order to get started using MavensMate for Sublime Text, you should be aware of a few important settings. MavensMate for Sublime Text settings follow the Sublime Text convention of providing default settings in [JSON format](https://en.wikipedia.org/wiki/JSON) that can be overwritten via a user settings file. To view MavensMate default and user settings, use the MavensMate menu in the top menu bar: `MavensMate > Settings`.

**NEW IN v7**: Most settings formerly found within Sublime Text have been moved to the "Global Settings" which can be found within mavensmate-app. To access/update those settings, use the `MavensMate` menu in Sublime Text and select `Settings > Global Settings`.

###Important Settings

####Workspaces (mm_workspace)

You must configure the `mm_workspace` setting before creating a new MavensMate project. You may set `mm_workspace` to a single path on your local filesystem or an array of paths.

#####Examples

######Array of workspaces

```
"mm_workspace" : [
	"/Users/darylshaber/Desktop/my-cool-folder",
	"/Users/darylshaber/Workspaces/my-mavensmate-workspace"
],
```

######Single workspace

```
"mm_workspace" : "/Users/darylshaber/Desktop/my-cool-folder",
```

**Windows users:** You must use escaped backslashes to set your workspaces:

```
"mm_workspace" : [
	"\\Users\\darylshaber\\Desktop\\my-cool-folder",
	"\\Users\\darylshaber\\Workspaces\\my-mavensmate-workspace"
],
```

####Salesforce API Version (mm_api_version)

Use `mm_api_version` to set your desired Salesforce.com API version. Please note, it should be set to a single decimal place:

#####Correct

```
"mm_api_version" : "33.0",
```

#####Incorrect

```
"mm_api_version" : 33,
```

##Update

Updates to the plugin are handled automatically by Package Control. Updates can be applied manually by replacing the `MavensMate` directory in your Sublime Text `Packages` directory.

##Documentation
<a href="MavensMate for Sublime Text Documentation">http://mavensmate.com/Plugins/Sublime_Text/Overview</a>

##Screenshots

###Project Wizard
<img src="http://cdn.mavensconsulting.com/mavensmate/img/new-project.png" style="box-shadow:-14px 14px 0 0 #16325c"/>
###Apex Test Runner
<img src="http://cdn.mavensconsulting.com/mavensmate/img/tests.png"/>
###Apex Execute Anonymous
<img src="http://cdn.mavensconsulting.com/mavensmate/img/execute-apex.png"/>
###Quick Panel
<img src="http://wearemavens.com/images/mm/panel.png"/>
###Apex/Visualforce Code Assist
<img src="http://cdn.mavensconsulting.com/mavensmate/img/apex2.png"/>
<img src="http://cdn.mavensconsulting.com/mavensmate/img/vf1.png"/>
<img src="http://cdn.mavensconsulting.com/mavensmate/img/vf2.png"/>

[mmcom]: http://mavensmate.com/?utm_source=github&utm_medium=st-plugin&utm_campaign=st
