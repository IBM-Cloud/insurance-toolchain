# Cloud Insurance Co. - Toolchain

This toolchain deploys the [Cloud Insurance Co.](https://github.com/IBM-Cloud/cloudco-insurance) project.

Get started with this project, which is an online insurance application that consists of microservices:

* [insurance-catalog][catalog_github_url] - An API to retrieve and update a catalog of insurance policies
* [insurance-orders][orders_github_url] - An API to retrieve and update a list of insurance policy orders made by customers
* [insurance-bot][bot_github_url] - UI that provides a chat bot interface for users to query their health benefits and file claims.
* [insurance-bot-dashboard][dashboard_github_url] - A user interface showing an history of the bot chats for further analysis.
* [insurance-bot-ios][ios_github_url] - An iOS application for the chat bot.
* [insurance-bot-android][android_github_url] - An Android application for the chat bot.

## Create the toolchain

1. Ensure you have 2GB of free memory and space for 5 additional services in your organization.

1. It is recommended to create a new space in your organization. This helps grouping the apps and services together in the console.

1. **To get started, click this button:**

  [![Deploy To IBM Cloud](./.bluemix/create_toolchain_button.png)](https://new-console.ng.bluemix.net/devops/setup/deploy/?repository=https%3A//github.com/IBM-Cloud/insurance-toolchain.git)

  Clicking it will:
  * **create 4 GitHub repositories** with the required source code for all the application components;
  * **instantiate the toolchain** in your IBM Cloud org and space;
  * **trigger the toolchain**, thereby deploying the selected branches (default to master) for all application components.


The toolchain is preconfigured for:

- issue tracking
- source control
- continuous delivery and integration (CI/CD)
- unit and code coverage testing
- blue-green deployment

---

### Learn more

* IBM Cloud DevOps Services: https://new-console.ng.bluemix.net/devops
* Documentation on [IBM Cloud Toolchains][toolchains_overview_url]
* InterConnect 2016 [video recording][toolchains_interconnect_video_url]
* [IBM Cloud Garage Method][garage_method_url]

<!--Links-->
[bot_github_url]: https://github.com/IBM-Cloud/insurance-bot
[orders_github_url]: https://github.com/IBM-Cloud/insurance-orders
[catalog_github_url]: https://github.com/IBM-Cloud/insurance-catalog
[dashboard_github_url]: https://github.com/IBM-Cloud/insurance-bot-dashboard
[ios_github_url]: https://github.com/IBM-Cloud/insurance-bot-ios
[android_github_url]: https://github.com/IBM-Cloud/insurance-bot-android
[toolchains_overview_url]: https://new-console.ng.bluemix.net/docs/toolchains/toolchains_overview.html
[toolchains_interconnect_video_url]: https://vimeo.com/156126035/8b04b8878a
[garage_method_url]: https://www.ibm.com/devops/method
