# 🤖 Making SAP Transactions Accessible Using OData APIs for Autonomous Agents and more on Power Platform. <br><br>

### Why APIs and OData for SAP?<br>

APIs provide a **consistent interface** for interacting with complex systems like SAP. With OData APIs, agents can:<br>

- Dynamically construct requests based on user intent  
- Call SAP transactions without needing custom logic  
- Improve accuracy and efficiency over time  <br>

### Importance of OData for General Application Development<br>

**OData (Open Data Protocol)** is crucial for modern application development. Key reasons include:<br>

- **Interoperability**: Seamless integration between SAP and non-SAP applications.
- **Standardization**: Simplifies development and ensures consistency.
- **Flexibility**: Suitable for various application types.<br>

By leveraging SAP OData APIs, developers can create robust, scalable applications that meet modern enterprise needs.<br><br>


## 🌐 Why APIs Matter for Autonomous Agents and Beyond:<br>

As agents become more autonomous, their ability to interact with enterprise systems through **APIs** has become not just beneficial—but essential. This repository demonstrates how to make **SAP transactions accessible to agents** using a combination of the **Power Platform**, **Copilot Studio**, **Azure AI Foundry**, and **SAP OData APIs**.<br>

In traditional automation setups, **connectors** were used to bridge systems. These connectors often relied on **predefined input fields** that required manual data entry or mappings. While effective for simple workflows, this model breaks down in the context of autonomous agents. Agents are not designed to manually fill out forms or input fields. Instead, they require:<br>

- **Standardized templates** for communication.
- The ability for **dynamic request generation** based on context and reasoning. <br><br>



## 📦 What's in This Repository<br>

This repo includes everything needed to build and deploy intelligent agents that can interact with SAP:<br>

### - OData API Templates<br>
  A curated list of common SAP business object APIs (e.g., Sales Orders, Materials, Vendors) with:
  - Minimum required fields to create each object
  - Example payloads for quick testing and integration<br>


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

 
 ### - Power Automate Flows<br>

Traditionally, working with SAP OData APIs required manual parsing of responses, mapping fields, and configuring connectors—often a tedious and technical process. But now, with **Copilot Studio**, you can use **natural language** to dynamically generate and execute OData requests. Here's how it transforms two common scenarios:<br>

> 💡 **Note:** The Power Automate flows provided here are just a starting point. You can customize and extend them to suit your specific SAP scenarios.<br>

---
**🛠️ Create Scenarios — From Conversations to Transactions**<br>

**Old Way:**  
To create a sales order from lets say an email, you had to extract structured data from emails, manually map it to SAP fields, and build a connector flow.

**New Way with AI:** 
Just say:  
> “Create a sales order from this email”
or  <br>
> “Turn this Teams conversation into a Purchase Requisition.”

Copilot Studio uses AI to:
- Understands the API documentation and extract relevant fields and creates the correct JSON Payload.
- Generates the correct OData URL.
- Call your SAP system directly—no manual mapping needed.

📷 _Before: Manual field mapping and connector setup_  
./images/create-before.png

📷 _After: Natural language to sales order via Copilot Studio_  
./images/create-after.png

---

**🔍 Query Scenarios — Natural Language Filters for Dynamic Data**

**Old Way:**  
You had to manually define filters and query parameters in a rigid format.

**New Way with AI:**  
Just ask:  
> “Get me all POs that are open and have vendor ‘1023’”  
or  
> “Show me the sales orders that were blocked in the last month.”

Copilot Studio:
- Parses your sentence.
- Builds the correct OData query URL.
- Executes it against your SAP backend.

📷 _Before: Static filter configuration in Power Automate_  
![Insert/query-before.png

📷 _After: Dynamic query generation from natural language_  
./images/query-after.png

---

#### ✨ The Impact

- **Faster workflows**: Skip the manual setup and go straight from intent to action.
-  **Smarter automation**: AI handles both the generation and execution of requests.
- **More accessible**: Business users can interact with SAP data without needing to know OData syntax.
-

  Pre-built flows for each transation mentioned below ( look at the Table of contents):
  - Accept user input
  - Use an HTTP connector to call an  Azure OpenAI API that converts natural language into structured API requests
  - Call SAP using the OData connector
  - Return the response to an agent created on Copilot Studio for further processing
 

### - Copilot Studio Agent Project**  
  A ready-to-use Copilot Studio project that demonstrates:
  - How to trigger flows using natural language or events
  - How using OData APIs make SAP transactions more easiliy accessible for Agents.
  - How to use new AI features like reasoning and memory
  - How to orchestrate actions across Microsoft 365 and SAP to save time and automate business processes
  - Instructions on how to create it.


## 🚀 Why This Matters

By combining the Power Platform, OpenAI, and SAP OData APIs, this solution enables:

- Seamless integration between communication tools (like Outlook and Teams) and ERP systems  
- Agents that can reason, decide, and act—without manual intervention  
- A scalable foundation for building intelligent business process automation





## Getting Started 🛫

## Contributing 👩🏼‍🤝‍👨🏽

This project welcomes contributions and suggestions. Use Pull Requests to propose changes to the content. Please see the [contribution guidelines](CONTRIBUTING.md) for more information.

Please use [GitHub Issues](https://github.com/Azure-Samples/sap-odata-api-guide-copilot/issues) to report errors or request new features.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](opencode@microsoft.com) with any additional questions or comments.

## Resources
