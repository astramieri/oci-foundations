# Cost Management

OCI provides different tools to manage costs.

The first tool are **OCI Budgets**. You can use budgets to track costs in your tenancy. After creating a budget for a compartment, you can set up alerts that will notify you if a budget is forecast to be exceeded or if spending surpasses a certain amount. 

The second tool is **Cost Analysis**. You could analyze your cost after you have spent it, but it's a nice way to look at your past cost and then make changes for the future. If there are elements you want to change, this is a great way to do that.

There are also **Usage reports**. Today, currently the Usage Reports get downloaded in form of these CSV files, and these are generated daily. And they show usage data for each resource in your tenancy. The CSV files are stored in an object storage bucket that is accessible using a cross-tenancy policy, so you could look across not just your tenancy, you could look across multiple tenancies if there are multiple tenancies being used.

There are also **Service Limits**, the tool to set your limits, quota, and usage. So as with any Cloud, OCI limits how many resources you can run in a traditional tenancy to prevent things like fraud and misuse. If you are using compartments, you have ability to set up **Compartment Quotas**.  

## Notes

In Oracle Cloud Infrastructure, you can set up email alerts to receive notifications when budget thresholds are reached. These alerts help customers stay informed about their spending and take appropriate actions to manage their costs.

Service limits are the upper bounds placed by Oracle on the number of resources you can create in a region or tenancy, while compartment quotas are the upper bounds defined by the users for resource usage within specific compartments. The distinction is that service limits are set by Oracle and apply to a tenancy in a region, while compartment quotas are set by the users and apply to specific compartments.

