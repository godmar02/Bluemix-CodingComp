![alt tag](http://www.dbtekpro.com/wp-content/uploads/2015/07/bluemix-logo.png)

# Getting ready to use Bluemix in the Coding Competition

Below we have collated a list of material that we hope participants will find useful to get up and running quickly.

## Sign up for Bluemix

Make sure to [sign up here for Bluemix][bluemix_signup_url]

## Learn the Basics

### Welcome to Bluemix

Please start by watching these **introductory videos:**

<a href="https://www.youtube.com/watch?v=Hcu664HbfS4"><img src="http://img.youtube.com/vi/Hcu664HbfS4/0.jpg" width="600">

<a href="http://www.youtube.com/watch?v=GsGnyZedlFk"><img src="http://img.youtube.com/vi/GsGnyZedlFk/0.jpg" width="600">

### Learn how to deploy an app based on Cloud Foundry

[Cloud Foundry][cloud_foundry] is the open-source platform-as-a-Service (PaaS) that Bluemix is built upon. This platform allows you to concentrate on your code without worrying about the underlying infrastructure (like setting up virtual machines (VMs) or containers). That allows you to get your apps up and running quickly... which makes it an ideal environment for a coding competition.

Here's a link to get you started: [Creating Cloud Foundry apps][cf_basics]

If you prefer a more structured course, here is a link to a 4-hour online class to get you started with Bluemix: [Bluemix Essentials][bluemix-essentials]

For additional start-up guides please see the following [here][additional_guide1] and  [here][additional_guide2].

## More in depth material

Covered the basics and want to move on? Level up with this in-depth material.

#### Collaborative coding and CI/CD pipeline

If you're working with others as part of a team, you'll probably want to use a collaborative coding tool like github and maybe also automate and orchestrate testing, notifications and deployments. The toolchain feature is meant to do exactly that. [Click here to find out how to use it.][opentoolchain_docs]

#### Internet of Things (IoT)

If you want to work to an IoT theme, you'll want to learn [Node-RED][nodered_url]. It's an open-source "visual tool for wiring the Internet of Things" and a great way to quickly become productive in a very short period of time. It also requires very little coding knowledge.

Node-RED can be deployed on Bluemix [with a single click.][iotp_boilerplate]. Here is a great example of how to build a real-time chat app with Node-RED in [5 minutes!][example_node_red_chat]

Next, [learn more about our IoT platform service][IoTP_url]. Once you understand how it works, go to [this link here to find step-by-step instructions to connect your physical devices][recipes_url] (like a [Rasperry Pi][raspberry_url], an [Arduino][arduino_url] or [TI Sensor Tag][sensortag_url]).

#### Using Watson cognitive services

Most coding competition participants want to take our IBM Watson services for a spin. Here are two detailed tutorials on how to integrate a cognitive service into your app:

* [Developing a Watson application in Node.js][watson_nodejs]
* [Developing a Watson application in Java][watson_java]

#### Online Courses

Here is the link to all the Bluemix online classes from IBM: [developerWorks Courses][developer_courses]

To really dive deep, you might want to take "Cloud Application Developer Certification Preparation", which should take you two or three days: [Cloud Application Developer Certification Preparation][certification_url]


## Step-by-step tutorials

And if you're looking for more, [here is a link to over 400 detailed step-by-step coding tutorials][bluemix_tutorials-url] for Bluemix.

## Inspiring examples

Looking for some inspiring examples? [Here is a gallery of 20 well documented apps built on Bluemix.][watson_starter-kits] All of them with a cognitive capability and based on the Watson technology. Each has a link to the running app and also links to the source on github.

And [here are almost 500 apps built on Bluemix from hackathons around the world][devpost_url], many linking to the source code.

## Support Documentation

Make sure to [search the Bluemix docs][bluemixdocs_url] first.

Still stuck? Head on over to stackoverflow.com and make sure to tag your question with "bluemix". [Here is a direct link.][stackoverflow_url]

## Further Reading

[Here is][jazz_editor] a very quick start-up to getting a node.js app up and running but more importantly it shows you how you can integrate with GIT and use Bluemix’s WEB IDE code editor to autodeploy your application

There are plenty of freely available Bluemix resources stored in [github][git_hub].


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

[example_node_red_chat]: http://www.ibm.com/developerworks/cloud/library/cl-rtchat-app
[jazz_editor]: https://hub.jazz.net/tutorials/jazzeditor
[additional_guide1]: http://www.ibm.com/cloud-computing/bluemix/getting-started/
[additional_guide2]: http://www.ibm.com/developerworks/learn/cloud/bluemix/quick-start/index.html
[git_hub]: https://github.com/ibm-bluemix?cm_mc_uid=55107028533214736821719&cm_mc_sid_50200000=1473779643
[Web_IDE]: https://new-console.ng.bluemix.net/docs/toolchains/web_ide.html

