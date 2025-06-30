# 💻 Laptop Request Management System | ServiceNow

This project is a ServiceNow-based **Laptop Request Management System** that allows employees or users to request new laptops via a predefined service catalog form. The request form collects essential details such as laptop model, justification, and optional accessories.

---

## 📌 Project Overview

The Laptop Request System simplifies the hardware request process by enabling users to submit detailed laptop requisitions from a catalog interface. It ensures transparency, traceability, and standardized approval workflows.

---

## 🧰 Tech Stack

- **Platform**: ServiceNow (Classic UI)
- **Module**: Service Catalog → Hardware → Laptop Request
- **Features**: Catalog item form with validation, workflow routing, and accessory tracking

---

## 🚀 Features

- ✅ **Model Input**: User specifies laptop brand/model (e.g., "HP")
- ✅ **Justification**: Free-text reasoning field (e.g., “Good product HP”)
- ✅ **Optional Accessories**: Checkbox-enabled accessory section
- ✅ **Accessories Details**: Captures OS or add-on specs (e.g., "Windows 11")
- ✅ **Order Flow**: Submit via "Order Now" or save to cart
- ✅ **Delivery Estimate**: Displays expected delivery (e.g., 2 days)

---

## 📷 UI Snapshot

Form fields captured from the ServiceNow catalog item:

| Field               | Example Value     |
|--------------------|-------------------|
| **Laptop Model**    | HP                |
| **Justification**   | Good product hp   |
| **Accessories**     | Windows 11        |
| **Delivery Time**   | 2 Days            |

---

## 🛠️ Setup & Customization (Admin Guide)

### 1. Create the Catalog Item

- Navigate to **Service Catalog > Maintain Items**
- Click **New**
- Fill in the name: `Laptop Request`
- Assign category: `Hardware`

### 2. Configure Variables

| Name                | Type         | Notes                         |
|---------------------|--------------|-------------------------------|
| `Laptop Model`      | Single Line  | Input model name              |
| `Justification`     | Multi-line   | Reason for request            |
| `Additional Accessories` | Checkbox | Toggle accessories            |
| `Accessories Details` | Multi-line | Describe OS or add-ons        |

### 3. Add Workflow (Optional)

Attach an approval or fulfillment workflow to route the request through:

- Manager approval
- IT support fulfillment
- Delivery updates

---

## 🔐 Permissions

Ensure users have access to:

- **Catalog item visibility**
- **Submit request permission**
- **View order history**

---

## 💡 Future Enhancements

- 🔁 Auto-approval for predefined models
- 📦 Integration with asset management
- 📊 Dashboard for laptop request analytics
- 🔔 Email/SMS notifications

---

## 📂 Folder Structure (If Exported to Update Set)

