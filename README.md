# CloudCo Toolchain


Get started with this sample, which is an online insurance application that consists of three microservices:  
- [Policy Catalog][github_catalog_url] - An API for retrieving and updating a catalog of insurance policies  
- [Orders][github_orders_url] - An API for retrieving and updating a list of insurance policy orders made by customers  
- [Store Front][github_store_url] - UI that leverages both of the above APIs to allow users to intelligently query the policies and narrow down to their best possible options

## Create the toolchain

**To get started, click this button:**  
[![Deploy To Bluemix](./.bluemix/create_toolchain_button.png)](https://new-console.ng.bluemix.net/devops/setup/deploy/?repository=https%3A//github.com//IBM-Bluemix/insurance-toolchain.git&branch=new-toolchain)

The toolchain is preconfigured for:

- issue tracking
- source control
- continuous delivery and integration (CI/CD)
- unit and code coverage testing
- blue-green deployment

![Toolchain template steps](./.bluemix/toolchain.png)

---
###Learn more

* Bluemix DevOps Services: https://new-console.ng.bluemix.net/devops
* Documentation on [Bluemix Toolchains][toolchains_overview_url]
* InterConnect 2016 [video recording][toolchains_interconnect_video_url]
* [IBM Bluemix Garage Method][garage_method_url]

<!--Links-->
[github_store_url]: https://github.com/IBM-Bluemix/insurance-store-front
[github_catalog_url]: https://github.com/IBM-Bluemix/insurance-catalog
[github_orders_url]: https://github.com/IBM-Bluemix/insurance-orders
[toolchains_overview_url]: https://new-console.ng.bluemix.net/docs/toolchains/toolchains_overview.html
[toolchains_interconnect_video_url]: https://vimeo.com/156126035/8b04b8878a
[garage_method_url]: https://www.ibm.com/devops/method
