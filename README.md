# 🤖 Making SAP Transactions Accessible for Autonomous Agents with OData APIs & Power Platform


## 🚀 Why SAP OData APIs Matter for Agents and Automation

SAP OData APIs are foundational for building intelligent, time-saving agents on top of SAP workflows. As organizations seek to automate complex business processes, the ability to interact with SAP in a standardized, scalable way becomes essential—not just for agents, but for any modern integration. Without a standardized approach like OData, automation efforts become fragmented and hard to scale. OData provides a consistent, RESTful interface to SAP business objects—unlocking the ability to build agents that can actually be enriched with  information from SAP systems as well as help people perform transactions in them,

To operate effectively, agents need:

- **Standardized templates for communication**  
- To **decide the appropriate SAP action**  and to **generate the requests and actions needed autonomously**

 SAP OData APIs enable users to create agents that can do just that.

While these APIs are available in SAP’s official documentation, they are often difficult to navigate. This repository serves as a **one-stop shop** for:

- Sample payloads and API URLs for common business objects like Sales Orders, Purchase Requisitions, and Invoices ( See the list below):
- A practical starting point for using these APIs in **Power Automate flows**  for dynamic request generation for these APIs.
- Templates and examples to help you build **autonomous agents** that interact with SAP intelligently.

---

## 📦 What’s Inside This Repository

### ✅ SAP OData API Requests

A curated set of SAP business object APIslisted with:
- URLs for GET and POST requests
- Example payloads for each.
  

    # List of SAP APIs from Buisness Accelerator Hub:

| **SAP Object** | **API Documentation** | **Power Automate Flow** |
|----------------|-----------------------|-------------------------|
| Sales Order | [Sales Order](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/Createsalesorder.zip) |[Create Sales Order](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/Createsalesorder.zip)|
| OutBound Delivery | [OutBound Delivery](https://github.com/noopurav/ordertocashsteps/tree/main?tab=readme-ov-file#deliver-the-goods-vl01n) | [Create OutBound Delivery](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/CreateOutboundDelivery.zip) |
| Billing Document | [Billing Document](https://github.com/noopurav/ordertocashsteps/tree/main?tab=readme-ov-file#billing-the-sales-order-vf01) | [Create Billing Document](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/Createsalesorder.zip) |
| Releasing Billing to Accounting | [Release Billing Document](https://github.com/noopurav/ordertocashsteps/tree/main#release-billing-document-to-fi-accounting-vf02) | Create Billing Document|
| Purchase Requisition | [Purchase Requistion](https://github.com/noopurav/ordertocashsteps/tree/main?tab=readme-ov-file#purchase-requisition) | [Create Purchase Requisition](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/CreatePurchaseRequistion.zip)  | 
| Purchase Order | [Purchase Order](https://github.com/noopurav/ordertocashsteps/tree/main?tab=readme-ov-file#create-purchase-order) | [Create Purchase Order](https://github.com/noopurav/ordertocashsteps/blob/main/CreatePurchaseOrder.zip)] | 
| Goods Receipt |  [Goods Receipt](https://github.com/noopurav/ordertocashsteps/tree/main?tab=readme-ov-file#goods-receipt )   |   Create Goods Receipt  |
| Supplier Invoice | [Supplier Invoice]( https://github.com/noopurav/ordertocashsteps/tree/main?tab=readme-ov-file#supplier-invoice) | [Create Supplier Invoice](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/CreateSupplierInvoice.zip)|
| Product Master | [Product Master](https://github.com/noopurav/ordertocashsteps/tree/main?tab=readme-ov-file#manage-product-master-data) | [Create Product](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/CreateAproduct.zip)    |
| Customer Master |[ Business Partner](https://github.com/noopurav/ordertocashsteps/tree/main?tab=readme-ov-file#manage-customer-master-dat) |  [Create Customer](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/CreateACustomer.zip)  |
| Sales Contract | [Sales Contract](https://github.com/noopurav/ordertocashsteps/tree/main?tab=readme-ov-file#manage-sales-contracts) |    [Create Sales Contract](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/CreateSalesContract.zip)    |
| Customer Return | [CustomerReturn](https://github.com/noopurav/ordertocashsteps/tree/main?tab=readme-ov-file#-manage-customer-returns) | [Create Customer Return](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/CreateCustomerReturn.zip)  |
| Credit Memo Request | [Credit Memo Request](https://github.com/noopurav/ordertocashsteps/tree/main?tab=readme-ov-file#manage-credit-memo-requests)  |  [Create Credit Memo Request](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/CreditMemoRequest.zip)  |
| Debit Memo Request | [CreateDebit Memo Request](https://github.com/noopurav/ordertocashsteps/tree/main?tab=readme-ov-file#manage-debit-memo-requests) | [Create Debit Memo Request](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/blob/main/CreateDebitmemoRequest.zip)  |


### ⚙️ Power Automate + Copilot Studio in Action

#### Create Scenarios — From Conversations to Transactions

**Old Way**:  
To create a sales order from an email, you had to extract structured data, manually map it to SAP fields, and build a connector flow.

**New Way with AI**: Just say:

- “Create a sales order from this email”  
- “Turn this Teams conversation into a Purchase Requisition”

Copilot Studio:

- Understands the API documentation  
- Extracts relevant fields and creates the correct JSON payload  
- Generates the correct OData URL  
- Calls your SAP system directly—no manual mapping needed

#### Query Scenarios — Natural Language Filters for Dynamic Data

**Old Way**:  
You had to manually define filters and query parameters in a rigid format.

**New Way with AI**: Just ask:

- “Get me all POs that are open and have vendor ‘1023’”  
- “Show me the sales orders that were blocked in the last month”

Copilot Studio:

- Parses your sentence  
- Builds the correct OData query URL  
- Executes it against your SAP backend

---

### 🤖 Copilot Studio Agent Project

A ready-to-use agent that:

- Triggers flows via natural language or events  
- Uses memory and reasoning to handle SAP transactions  
- Orchestrates actions across SAP and Microsoft 365  
- Accepts user input, uses an HTTP connector to call Azure OpenAI, and returns structured responses

---

## ✨ The Impact

- **Faster Workflows**: From intent to action—no manual setup  
- **Smarter Automation**: AI handles request generation and execution  
- **More Accessible**: Business users can interact with SAP using plain language  

---

## 🛠️ Build Your Own Agent

This repo is more than a toolkit—it’s a **starting point** for building intelligent agents that:

- Understand business context  
- Interact with SAP in real time  
- Dynamically generate OData queries from everyday work situations (e.g., emails, chats, meetings)  
- Use Copilot Studio to deploy these capabilities directly into your workflows—like Microsoft Teams, Outlook, or Power Apps  

Whether you're automating purchase requisitions from a Teams conversation or querying blocked sales orders from an email, this solution empowers agents to act with intelligence and context—right where work happens.

---



## Getting Started 🛫

## Contributing 👩🏼‍🤝‍👨🏽

This project welcomes contributions and suggestions. Use Pull Requests to propose changes to the content. Please see the [contribution guidelines](CONTRIBUTING.md) for more information.

Please use [GitHub Issues](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/issues) to report errors or request new features.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](opencode@microsoft.com) with any additional questions or comments.

## Resources
