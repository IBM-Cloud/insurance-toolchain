# Cloud Insurance Co. - Toolchain

This toolchain deploys the [Cloud Insurance Co.](https://github.com/IBM-Cloud/cloudco-insurance) project.

Get started with this project, which is an online insurance application that consists of microservices:

* [insurance-bot][bot_github_url] - UI that provides a chat bot interface for users to query their health benefits and file claims.
* [insurance-bot-dashboard][dashboard_github_url] - A user interface showing an history of the bot chats for further analysis.

## Create the toolchain

1. Ensure you have 2GB of free memory and space for the [Continuous Delivery](https://console.bluemix.net/catalog/services/continuous-delivery) and 4 additional services in your organization:
* [IBM Cloudant](https://console.bluemix.net/catalog/services/cloudant)
* [Watson Assistant](https://console.bluemix.net/catalog/services/watson-assistant-formerly-conversation)
* [App ID](https://console.bluemix.net/catalog/services/app-id)
* [Tone Analyzer](https://console.bluemix.net/catalog/services/tone-analyzer)

2. It is recommended to [create a new space](https://console.bluemix.net/docs/account/orgs_spaces.html#orgsspacesusers) in your organization. This helps grouping the apps and services together in the console.

3. **To Deploy, click this button:**

    [![Deploy to IBM Cloud](https://bluemix.net/deploy/button.png)](https://bluemix.net/deploy?repository=https%3A//github.com/IBM-Cloud/insurance-toolchain.git)

    Clicking it will:
    * **Instantiate the toolchain** in your IBM Cloud org and space. Provide an unique name for the toolchain and select an appropriate region and org.  
    * **Create 2 GitHub repositories** with the required source code for all the application components. You may be asked to provide permissions to create repos on your GitHub account.
    * **Trigger the toolchain**, thereby deploying the selected branches (default to master) for all application components.

4. Once deployed, click on the **bot(master)** tile under Deliver >  **Deploy** stage, check LAST EXECUTION RESULT to see the webui link for the bot.
5. You can check and modify your toolchain anytime under [DevOps](https://console.bluemix.net/devops) on IBM Cloud. Choose an appropriate region and Org.

The toolchain is preconfigured for:

- issue tracking
- source control
- continuous delivery and integration (CI/CD)
- unit and code coverage testing
- blue-green deployment

## Cleanup
If you want to remove the resources associated to the Cloud Insurance Co. project, follow these steps to clean up toolchain, services and GitHub repositories.   
1. Go to the [IBM Cloud dashboard for toolchains](https://console.bluemix.net/devops/toolchains), select the **region** and **organization** in which you deployed the toolchain. Locate the toolchain and in its action menu click on **Delete**. The toolchain and its components are going to be removed.
2. Next, delete the deployed apps and their services. In the [IBM Cloud dashboard](https://console.bluemix.net/dashboard/apps) locate the two deployed Cloud Foundry apps. You can select the organization, space and location (region). In addition, you can utilize the search filter.
  * Click on the action menu for the UI (bot) app and select **Delete App**. In the dialog window, mark both the shown services and route for deletion. Thereafter, click on **Delete**.
  * Repeat the same for the dashboard app.
  * Last, locate the related Cloudant service under **Cloud Foundry Services**. In the action menu, click on **Delete Service** and complete the dialog.
3. To remove the GitHub repositories for the bot and bot dashboard, you need to log in to your [GitHub account](https://github.com).
  * Go to your profile, e.g., by selecting it in the top right menu. Then, go to the repositories overview. The URI has this form: `https://github.com/username?tab=repositories`
  * Locate the bot and later the dashboard repository. For each, click on **Settings**. At the bottom, in the so-called **Danger Zone**, is an option to delete the repository. After clicking on **Delete this repository** you are asked to confirm by typing or copying in the reopsitory name. Then complete the dialog.

Once done, all resources that were created during the toolchain-based deployment are cleaned up. The only exception is the Continuous Delivery service. It is a shared service. If it is not used by any other project, you can find and delete it in the IBM Cloud dashboard. See step two.

## Learn more

* IBM Cloud DevOps Services: https://console.bluemix.net/devops
* Documentation on [IBM Cloud Toolchains][toolchains_overview_url]
* [IBM Cloud Garage Method][garage_method_url]

<!--Links-->
[bot_github_url]: https://github.com/IBM-Cloud/insurance-bot
[dashboard_github_url]: https://github.com/IBM-Cloud/insurance-bot-dashboard
[toolchains_overview_url]: https://console.bluemix.net/docs/services/ContinuousDelivery/toolchains_working.html
[toolchains_interconnect_video_url]: https://vimeo.com/156126035/8b04b8878a
[garage_method_url]: https://www.ibm.com/cloud/garage/toolchains
