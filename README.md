# 🤖 Making SAP Transactions Accessible for Autonomous Agents with OData APIs & Power Platform


## 🚀 Why SAP OData APIs Matter for Agents and Automation

SAP OData APIs are foundational for building intelligent, time-saving agents on top of SAP workflows. As organizations seek to automate complex business processes, the ability to interact with SAP in a standardized, scalable way becomes essential—not just for agents, but for any modern integration. OData provides a consistent, RESTful interface to SAP business objects—unlocking the ability to build agents that can actually be enriched with  information from SAP systems as well as help people perform transactions in them.

To operate effectively, agents need:

- **Standardized templates for communication**  
- To **decide the appropriate SAP action**  and to **generate the requests and actions needed autonomously**

 SAP OData APIs enable agents to do just that.

While these APIs are available in SAP’s official documentation, they are often difficult to navigate. This repository serves as a **one-stop shop** for:

- Sample payloads and API URLs for common business objects like Sales Orders, Purchase Requisitions, and Invoices ( See the list below):
- A practical starting point for using these APIs in **Power Automate flows**  for dynamic request generation for these APIs.
- Templates and examples to help you build **autonomous agents** that interact with SAP intelligently.

---

# 📦 What’s Inside This Repository<br>

## ✅ [SAP OData API Requests](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/SAP%20OData%20API%20Reference.md)<br>

A curated set of SAP business object APIs listed with:
- URLs for GET and POST requests
- Example payloads for each.
  

### List of SAP APIs from Buisness Accelerator Hub:

# SAP APIs from Buisness Accelerator Hub:

| **SAP Object** | **API Documentation** | **Power Automate Flow** |
|----------------|-----------------------|-------------------------|
| Sales Order | [Sales Order](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/SAP%20OData%20API%20Reference.md#create-sales-ordercreate-sales-order) |[Create Sales Order](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/PowerAutomateFlows/Createsalesorder.zip)|
| OutBound Delivery | [OutBound Delivery](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/SAP%20OData%20API%20Reference.md#deliver-the-goods-vl01n) | [Create OutBound Delivery](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/PowerAutomateFlows/CreateGoodsDelivery.zip) |
| Billing Document | [Billing Document](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/SAP%20OData%20API%20Reference.md#billing-the-sales-order-vf01) | [Create Billing Document](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/PowerAutomateFlows/BillingDocument.zip) |
| Releasing Billing to Accounting | [Release Billing Document](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/SAP%20OData%20API%20Reference.md#release-billing-document-to-fi-accounting-vf02) | [Release Billing Document](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/PowerAutomateFlows/ReleaseBIllingDocumenttoAccounting.zip)|
| Purchase Requisition | [Purchase Requistion](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/SAP%20OData%20API%20Reference.md#purchase-requisition) | [Create Purchase Requisition](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/PowerAutomateFlows/CreatePurchaseRequistion.zip)  | 
| Purchase Order | [Purchase Order](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/SAP%20OData%20API%20Reference.md#create-purchase-order) | [Create Purchase Order](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/PowerAutomateFlows/CreatePurchaseOrder.zip) | 
| Goods Receipt |  [Goods Receipt](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/SAP%20OData%20API%20Reference.md#goods-receipt)   |   [Create Goods Receipt](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/PowerAutomateFlows/CreateGoodsReceipt.zip)  |
| Supplier Invoice | [Supplier Invoice](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/SAP%20OData%20API%20Reference.md#supplier-invoice) | [Create Supplier Invoice](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/PowerAutomateFlows/CreateSupplierInvoice.zip)|
| Product Master | [Product Master](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/SAP%20OData%20API%20Reference.md#manage-product-master-data) | [Create Product](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/PowerAutomateFlows/CreateAproduct.zip)    |
| Customer Master |[ Business Partner](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/SAP%20OData%20API%20Reference.md#manage-customer-master-data) |  [Create Customer](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/PowerAutomateFlows/CreateACustomer.zip)  |
| Sales Contract | [Sales Contract](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/SAP%20OData%20API%20Reference.md#manage-sales-contracts) |    [Create Sales Contract](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/PowerAutomateFlows/CreateSalesContract.zip)    |
| Customer Return | [CustomerReturn](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/SAP%20OData%20API%20Reference.md#-manage-customer-returns) | [Create Customer Return](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/PowerAutomateFlows/CreateCustomerReturn.zip)  |
| Credit Memo Request | [Credit Memo Request](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/SAP%20OData%20API%20Reference.md#manage-credit-memo-requests)  |  [Create Credit Memo Request](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/PowerAutomateFlows/CreditMemoRequest.zip)  |
| Debit Memo Request | [CreateDebit Memo Request](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/SAP%20OData%20API%20Reference.md#manage-debit-memo-requests) | [Create Debit Memo Request](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/PowerAutomateFlows/CreateDebitmemoRequest.zip)  |
| Enterprise Project | [Enterprise Project](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/SAP%20OData%20API%20Reference.md#enterprise-projects)  |  [Create Enterprise Project](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/PowerAutomateFlows/CreateEnterpriseProject.zip)  |
| Project Billing Request | [Project Billing Request](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/SAP%20OData%20API%20Reference.md#project-billing-request) | [ Create Project Billing Request](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/PowerAutomateFlows/ProjectBillingRequest.zip)  |
 <br> <br>

## ⚙️ [Power Automate Flows](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/tree/main/PowerAutomateFlows):

These Power Automate flows provide examples of how you can dynamically create SAP objects and query SAP systems without having to fill in each field and can be easily used by Agents in Copilot Studio: <br>
#### Creating SAP Objects with Agents:

**Old Way**:  
To create a sales order from an email, you had to extract structured data, manually map it to SAP fields, and build a connector flow.

**New Way with AI**: Just say:

- “Create a sales order from this email”  
- “Turn this Teams conversation into a Purchase Requisition”

The Power Automate flow:

- Understands the API documentation using Azure Open AI
- Extracts relevant fields and creates the correct JSON payload using Azure Open AI
- Generates the correct OData URL  
- Calls your SAP system directly—no manual mapping needed

#### Quering SAP Data through natural language:

**Old Way**:  
You had to manually define filters and query parameters in a rigid format.

**New Way with AI**: Just ask:

- “Get me all POs that are open and have vendor ‘1023’”  
- “Show me the sales orders that were blocked in the last month”

Power Automate Flow:

- Parses your sentence  
- Builds the correct OData query URL using AI.
- Executes it against your SAP backend
---

This repo is a toolkit— for building intelligent agents  that:
- Understand business context and interact with SAP in real time informed with that context. 
- Dynamically generate OData queries from everyday work situations (e.g., emails, chats, meetings)  
- Are deployed directly into your workflows—like Microsoft Teams, Outlook using Copilot Studio. 

Whether you're automating purchase requisitions from a Teams conversation or querying blocked sales orders from an email, the APIs and Power Automate flows in this solution along with Copilot Studio will empower you to create SAP agents that take action with intelligence and context—right where work happens.

---



## Getting Started 🛫

## Contributing 👩🏼‍🤝‍👨🏽

This project welcomes contributions and suggestions. Use Pull Requests to propose changes to the content. Please see the [contribution guidelines](CONTRIBUTING.md) for more information.

Please use [GitHub Issues](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/issues) to report errors or request new features.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](opencode@microsoft.com) with any additional questions or comments.

## Resources
