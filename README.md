![alt tag](http://www.dbtekpro.com/wp-content/uploads/2015/07/bluemix-logo.png)

# Getting ready to use Bluemix in the Coding Competition

Below we have collated a list of material that we hope participants will find useful to get up and running quickly.

## Sign up for Bluemix and migrating to the Coding Competition organisation

Make sure to [sign up here for the Bluemix 30 day free trial][bluemix_signup_url]. Once you have done this we will request team names and email addresses, we will then upgrade these accounts to fully managed and supported ones. Please note that this will need to be a new account if you have previously signed up.

Once we have let you know that we have added you to our Organisation you will be able to see "Coding Competition 2016" listed as an Organisation when you click on the top right hand icon in Bluemix (or in the new version of Bluemix this is to the left of this icon). Within that organisation we will have created a 'Space' named after your team, where you will work going forward. You may need to also change the 'Account' to GBS c/o GCPD.

In order to keep coding you will need to re-provision any services or applications that you set up in your 'Trial Space' and then push your code into this new 'Space'. Referencing the section below (Learn how to deploy an app based on Cloud Foundry) see the following steps for migrating your code into this 'Space':
- If you have been working on code using the Cloud Foundary CLI you will find that when you login using "cf login -a https://api.eu-gb.bluemix.net -u your_login_email_address" it will now ask you to select an organisation and a space to work in before you then can then push your code to Bluemix usinf "cf push". In order to skip this step at subsequent logins you can amend your login command to be "cf login -a https://api.eu-gb.bluemix.net -u your_login_email_address -o CodingCompetition2016 -s "your_team_space" "
- If you have been connecting you Bluemix app to a GIT repository then simply re-connect your app in the new 'Space' to the same repository you have been working off (using the GIT URL as you were using before), as per the instructions below.
- If you have been using NodeRed then please following the very simple instructions on this site [here][migrating_node_red] to export your settings and then import them into a new NodeRed space (note it is good practice to backup your code regardless of migration).

## Learn the Basics

### Welcome to Bluemix

Please start by watching these **introductory videos:**

<a href="https://www.youtube.com/watch?v=Hcu664HbfS4"><img src="http://img.youtube.com/vi/Hcu664HbfS4/0.jpg" width="600">

<a href="http://www.youtube.com/watch?v=GsGnyZedlFk"><img src="http://img.youtube.com/vi/GsGnyZedlFk/0.jpg" width="600">

### Learn how to deploy an app based on Cloud Foundry

[Cloud Foundry][cloud_foundry] is the open-source platform-as-a-Service (PaaS) that Bluemix is built upon. This platform allows you to concentrate on your code without worrying about the underlying infrastructure (like setting up virtual machines (VMs) or containers). That allows you to get your apps up and running quickly... which makes it an ideal environment for a coding competition. You can start adding cloud foundry apps directly from your Dashboard within bluemix and it allows you to select numerous templates depending upon what language you want to code in etc.

For a structured course on getting started here is a link to a 4-hour online class: [Bluemix Essentials][bluemix-essentials]. For additional start-up guides please see the following [here][additional_guide1] and [here][additional_guide2].

Once you have created a new app in Bluemix there are a number of ways you can work on it. 

For Beginners we would suggest that you choose to download code locally and then use the Cloud Foundry CLI in order to deploy changes to your applications on Bluemix. To do this:
- Click on your App in the Dashboard
- Then click on Start Coding on the left hand pane
- Find and click on DOWNLOAD STARTER CODE to save it on your machine.
- Make changes to the code however you want
- Ensure you have the Cloud Foundry CLI installed on your machine (download it from [here][CLI_Download]). This enables your computer to push changes to your code that you have made on your computer to Bluemix via the command line. 
- Navigate to your code directory using the Command Line in Windows or Terminal in a Mac (cd code_directory)
- Run the following command: cf login -a https://api.eu-gb.bluemix.net -u your_login_email_address
- Enter your Bluemix password
- Run the following command: cf push
- This will push a new version of your code up to Bluemix and restart your application for you! Check your app URL to see those changes.

A slightly more advance method involves connecting Bluemix to a GIT repository. The advantage of this method is that you then have your code in a repository that you can collaborate on and deliver changes rapidly without having to install the Code Foundry CLI or set up a GIT repository within GitHub as below in the collaborative coding section. To do this:
- Click on your app in the Dashboard
- Then click on Overview in the left hand pane
- Click on ADD GIT in top right hand corner of the page
- On the resulting popup ensure 'Populate the repo with the starter app package and enable the Build & Deploy pipeline' is ticked (this will allow for any changes to the GIT Repo to be picked up automatically).
- Bluemix will now create a GIT Repository containing the Starter Code as mentioned above. The resulting location will be a URL on the App Overview Page where ADD GIT was.
- Copy the GIT URL and clone it to your local machine using 'git clone' - you will need GIT installed on your machine if you're using Windows (see below for usage of GIT)
- Make changes to the code however you want
- GIT add, commit and push - the source code repo has a continuous delivery pipeline that will automatically pick up committed changes and build those into your app. Check your app URL to see those changes.

For further details on these methods, and more, visit the 'Start Coding' page which you can access in the left hand pane once you have clicked on your app within the Dashboard. 

## More in depth material

#### Collaborative coding and source control

If you're working with others as part of a team, you'll probably want to use a collaborative coding tool like GIT to keep track of your code and work together. In order to do this you will need to install GIT on your computer, which you can [download here][git]. This allows multiple users to 'clone' online Repositories (effectively just a code store) to their computers and work on seperately before pushing updates back into the central Repository.

If you are using the advanced method of code deployment above then you will already have a GIT Repository stored on the web, which users can collaborate on, click on the Repository URL and you can add members. If you have opted to use Cloud Foundry CLI to deploy your code then you can create a standalone Repository on GitHub. You can signup for a free a GitHub account [here][GitHub] and get started creating Repositories (you can push your starter code up into a new Repository).  

For a quick tutorial on GIT a great place to start is [here][learn_git].

#### Code Editing Tools

If you are working on your code locally i.e. on your laptop or computer, then we would suggest using one of the following tools that are designed for coding:
- [Sublime][sublime]
- [Notepad++][notepad]
- [Atom][atom]

#### Internet of Things (IoT)

If you want to work to an IoT theme, you'll want to learn [Node-RED][nodered_url]. It's an open-source "visual tool for wiring the Internet of Things" and a great way to quickly become productive in a very short period of time. It also requires very little coding knowledge. For example here is how to build a real-time chat app with Node-RED in [5 minutes!][example_node_red_chat]

Node-RED can be deployed on Bluemix and connected to an IoT device [with just a few clicks.][iot_connection]. To learn more about our IoT platform service [visit here][IoTP_url]. Once you understand a bit more about how it works, go to [this link here to find step-by-step instructions to connect your physical devices][recipes_url], like a guide to build an IOT Bluemix app in node.js with sensors on a [Raspberry Pi][iot_pibluemix] (and many more for the [Raspberry Pi][raspberry_url], [Arduino][arduino_url] or [TI Sensor Tag][sensortag_url]).

#### Data Visualisation

There are a number of data visualisation tools within Bluemix. Additionally, [this website][sitepoint] lists the 12 Best JavaScript libraries for Data Visualisation. 

There are a number of freely available datasets that you may wish to use for data visualisation:
- [Analytics Exchange][analytics_exchange]
- [UK Government Open Data][data_gov]
- [Namara open data sets][namara]

#### Using Watson cognitive services

Most coding competition participants want to take our IBM Watson services for a spin. Here are two detailed tutorials on how to integrate a cognitive service into your app:

* [Developing a Watson application in Node.js][watson_nodejs]
* [Developing a Watson application in Java][watson_java]

#### Online Courses

Here is the link to all the Bluemix online classes from IBM: [developerWorks Courses][developer_courses]

To really dive deep, you might want to take "Cloud Application Developer Certification Preparation", which should take you two or three days: [Cloud Application Developer Certification Preparation][certification_url]

For additional learning on the basic of Node.js (javascript) visit [Nodeschool][nodeschool] and for numerous other coding tutorials and lessons [Codecademy][codecademy].

## Step-by-step tutorials

And if you're looking for more, [here is a link to over 400 detailed step-by-step coding tutorials][bluemix_tutorials-url] for Bluemix.

## Inspiring examples

Looking for some inspiring examples? [Here is a gallery of 20 well documented apps built on Bluemix.][watson_starter-kits] All of them with a cognitive capability and based on the Watson technology. Each has a link to the running app and also links to the source on GitHub.

And [here are almost 500 apps built on Bluemix from hackathons around the world][devpost_url], many linking to the source code.

## Support Documentation

Make sure to [search the Bluemix docs][bluemixdocs_url] first.

Still stuck? Head on over to stackoverflow.com and make sure to tag your question with "bluemix". [Here is a direct link.][stackoverflow_url]

## Further Reading

There are plenty of freely available Bluemix resources stored in [GitHub][git_hub].


<!--Links-->

[bluemix_signup_url]: https://console.ng.bluemix.net/registration

[cloud_foundry]: https://www.cloudfoundry.org/
[cf_basics]: https://new-console.ng.bluemix.net/docs/cfapps/index.html
[bluemix-essentials]: https://developer.ibm.com/courses/all-courses/bluemix-essentials
[additional_guide1]: http://www.ibm.com/cloud-computing/bluemix/getting-started/
[additional_guide2]: http://www.ibm.com/developerworks/learn/cloud/bluemix/quick-start/index.html
[CLI_Download]: https://GitHub.com/cloudfoundry/cli
[migrating_node_red]: https://randomnerdtutorials.com/exporting-and-backing-up-your-node-red-nodes

[developer_courses]: https://developer.ibm.com/courses/#courses
[watson_starter-kits]: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/starter-kits.html


[GitHub]: https://GitHub.com
[git_hub]: https://GitHub.com/ibm-bluemix?cm_mc_uid=55107028533214736821719&cm_mc_sid_50200000=1473779643
[git]: https://git-scm.com/downloads 
[learn_git]: https://try.GitHub.io/levels/1/challenges/1 

[atom]: https://atom.io/
[sublime]: https://www.sublimetext.com/
[notepad]: https://notepad-plus-plus.org/

[nodeschool]: http://nodeschool.io/
[codecademy]: https://www.codecademy.com/ 

[nodered_url]: http://nodered.org/
[example_node_red_chat]: http://www.ibm.com/developerworks/cloud/library/cl-rtchat-app
[iot_connection]: https://developer.ibm.com/recipes/tutorials/creating-a-nodered-application-on-bluemix/
[iotp_boilerplate]: https://new-console.ng.bluemix.net/docs/starters/IoT/iot500.html#iot500
[IoTP_url]: https://new-console.ng.bluemix.net/docs/services/IoT/index.html
[recipes_url]: https://developer.ibm.com/recipes/
[iot_pibluemix]: https://developer.ibm.com/recipes/tutorials/build-an-iot-bluemix-app-in-node-js-with-sensors-on-raspberry-pi/
[raspberry_url]: https://developer.ibm.com/recipes/?post_type=tutorials&s=raspberry
[arduino_url]: https://developer.ibm.com/recipes/?post_type=tutorials&s=arduino
[sensortag_url]: https://GitHub.com/uwefassnacht/ti-sensor-tag-demo

[sitepoint]: https://www.sitepoint.com/twelve-javascript-libraries-data-visualization/ 
[analytics_exchange]: https://console.ng.bluemix.net/data/exchange/ 
[data_gov]: https://data.gov.uk/ 
[namara]: https://namara.io/#/ 

[watson_nodejs]: http://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/doc/getting_started/gs-full-nodejs.shtml
[watson_java]: http://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/doc/getting_started/gs-full-java.shtml
[bluemix_tutorials-url]: https://ibm.biz/bluemixtutorialsfordevs
[webinars-url]: https://webinars.mybluemix.net
[devpost_url]: http://devpost.com/software/built-with/bluemix
[bluemixdocs_url]: https://console.ng.bluemix.net/docs
[stackoverflow_url]: https://stackoverflow.com/questions/tagged/bluemix
[certification_url]: https://developer.ibm.com/courses/all-courses/cloud-app-developer-cert-prep/
[jazz_editor]: https://hub.jazz.net/tutorials/jazzeditor
[Web_IDE]: https://new-console.ng.bluemix.net/docs/toolchains/web_ide.html

