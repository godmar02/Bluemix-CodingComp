# Getting ready for a Bluemix Coding Competition

Here is a list of material that we found particularly useful to get participants up and running quickly.

## Sign up for Bluemix

Make sure to [sign up here for Bluemix][bluemix_signup_url]

## Learn the Basics

### Get an overview

Start with these **introductory videos:**

<a href="https://www.youtube.com/watch?v=Hcu664HbfS4"><img src="http://img.youtube.com/vi/Hcu664HbfS4/0.jpg" width="600">

<a href="http://www.youtube.com/watch?v=GsGnyZedlFk"><img src="http://img.youtube.com/vi/GsGnyZedlFk/0.jpg" width="600">

### Learn how to deploy an app based on Cloud Foundry

[Cloud Foundry][cloud_foundry] is an open-source platform-as-a-Service (PaaS) that allows you to concentrate on your code without worrying about the underlying infrastructure (like VMs or containers). That allows you to get your apps up and running quickly ... an ideal environment for a coding competition.

Here's a a link to get you started: [Creating Cloud Foundry apps][cf_basics]

If you prefer a more structured course, here is a link to a 4-hour online class to get you started with Bluemix: [Bluemix Essentials][bluemix-essentials]

## Drill down

Covered the basics and want to move on? Level up with this in-depth material.

#### Collaborative coding and CI/CD pipeline

If you're working with others as part of a team, you'll probably want to use a collaborative coding tool like github and maybe also automate and orchestrate testing, notifications and deployments. The toolchain feature is meant to do exactly that. [Click here to find out how to use it.][opentoolchain_docs]

#### Internet of Things (IoT)

If you want to work to an IoT theme, you'll want to learn [Node-RED][nodered_url]. It's an open-source "visual tool for wiring the Internet of Things" and a great way to quickly become productive in a very short period of time. It also requires very little coding knowledge.

Node-RED can be deployed on Bluemix [with a single click.][iotp_boilerplate]

Next, [learn more about our IoT platform service][IoTP_url]. Once you understand how it works, go to [this link here to find step-by-step instructions to connect your physical devices][recipes_url] (like a [Rasperry Pi][raspberry_url], an [Arduino][arduino_url] or [TI Sensor Tag][sensortag_url]).

#### Using Watson cognitive services

Most coding competition participants want to take our IBM Watson services for a spin. Here are two detailed tutorials on how to integrate a cognitive service into your app:

* [Developing a Watson application in Node.js][watson_nodejs]
* [Developing a Watson application in Java][watson_java]

#### Online Courses

Here is the link to all the Bluemix online classes from IBM: [developerWorks Courses][developer_courses]

To really dive deep, you might want to take "Cloud Application Developer Certification Preparation", which should take you two or three days: [Cloud Application Developer Certification Preparation][certification_url]

#### Webinars

We have an assortment of webinars available in various languages. [Have a look here.][webinars-url]

## Over 400 step-by-step tutorials

And if you're looking for more, [here is a link to over 400 detailed step-by-step coding tutorials][bluemix_tutorials-url] for Bluemix.

## Stuck? Need help?

Make sure to [search the Bluemix docs][bluemixdocs_url] first.

Still stuck? Head on over to stackoverflow.com and make sure to tag your question with "bluemix". [Here is a direct link.][stackoverflow_url]

## Inspiring examples

Looking for some inspiring examples? [Here is a gallery of 20 well documented apps built on Bluemix.][watson_starter-kits] All of them with a cognitive capability and based on the Watson technology. Each has a link to the running app and also links to the source on github.

And [here are almost 500 apps built on Bluemix from hackathons around the world][devpost_url], many linking to the source code.


## Further Reading
https://hub.jazz.net/tutorials/jazzeditor/#git_integration_and_autodeployment - This is a very quick start-up to getting a node.js app up and running and how you can then connect it to git such that you can , as well as integrating with GIT and coding using the web editor and git to autodeploy
https://console.eu-gb.bluemix.net/?/&direct=classic/#/resources/orgGuid=4c26d2f3-eca6-402f-b8fa-8fee5785263a&spaceGuid=6837eb01-3d09-4326-b836-831a2342f8c9&appGuid=a0057d01-556b-4cff-a5a0-b74623e3c2a3&detailType=gettingstarted&paneId=4
http://www.ibm.com/cloud-computing/bluemix/getting-started/
https://github.com/ibm-bluemix?cm_mc_uid=55107028533214736821719&cm_mc_sid_50200000=1473779643
https://console.ng.bluemix.net/docs
http://www.ibm.com/developerworks/learn/cloud/bluemix/quick-start/index.html 	
https://developer.ibm.com/courses/all-courses/bluemix-essentials/ 	
https://hub.jazz.net/tutorials/jazzeditor/ 	
https://opensource.com/life/16/5/getting-started-node-red 
http://www.ibm.com/developerworks/cloud/library/cl-rtchat-app/ - get sample code
https://new-console.ng.bluemix.net/docs/starters/IoT/iot500.html - boilerplates 	

## License

See [License](License) for license information.

<!--Links-->
[bluemix_signup_url]: https://console.ng.bluemix.net/registration
[cloud_foundry]: https://www.cloudfoundry.org/
[cf_basics]: https://new-console.ng.bluemix.net/docs/cfapps/index.html
[bluemix-essentials]: https://developer.ibm.com/courses/all-courses/bluemix-essentials
[opentoolchain_docs]:https://new-console.ng.bluemix.net/docs/toolchains/toolchains_overview.html
[developer_courses]: https://developer.ibm.com/courses/#courses

[watson_starter-kits]:https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/starter-kits.html

[nodered_url]: http://nodered.org/
[iotp_boilerplate]: https://new-console.ng.bluemix.net/docs/starters/IoT/iot500.html#iot500
[IoTP_url]: https://new-console.ng.bluemix.net/docs/services/IoT/index.html
[recipes_url]: https://developer.ibm.com/recipes/
[raspberry_url]: https://developer.ibm.com/recipes/?post_type=tutorials&s=raspberry
[arduino_url]: https://developer.ibm.com/recipes/?post_type=tutorials&s=arduino
[sensortag_url]: https://github.com/uwefassnacht/ti-sensor-tag-demo

[watson_nodejs]: http://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/doc/getting_started/gs-full-nodejs.shtml
[watson_java]: http://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/doc/getting_started/gs-full-java.shtml

[bluemix_tutorials-url]: https://ibm.biz/bluemixtutorialsfordevs
[webinars-url]: https://webinars.mybluemix.net

[devpost_url]: http://devpost.com/software/built-with/bluemix

[bluemixdocs_url]: https://console.ng.bluemix.net/docs
[stackoverflow_url]: https://stackoverflow.com/questions/tagged/bluemix

[certification_url]: https://developer.ibm.com/courses/all-courses/cloud-app-developer-cert-prep/
