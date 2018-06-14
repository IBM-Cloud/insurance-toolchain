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

2. It is recommended to [create a new space](https://console.bluemix.net/docs/account/orgs_spaces.html#orgsspacesusers) in your organization. This helps grouping the apps and services together in the console.

3. **To Deploy, click this button:**

    [![Deploy to IBM Cloud](https://bluemix.net/deploy/button.png)](https://bluemix.net/deploy?repository=https%3A//github.com/IBM-Cloud/insurance-toolchain.git)

    Clicking it will:
    * **instantiate the toolchain** in your IBM Cloud org and space; Provide an unique name for the toolchain and Select an appropriate region and org  
    * **create 4 GitHub repositories** with the required source code for all the application components;
    * **trigger the toolchain**, thereby deploying the selected branches (default to master) for all application components.

4. Once deployed, Click on the **bot(master)** tile under Deliver >  **Deploy** stage, check LAST EXECUTION RESULT to see the webui link for the bot.

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
