# Inventory Management System

## Overview
BiSquare, a small manufacturing organization, required a more efficient inventory system to replace their outdated spreadsheet-based approach. This **JavaFX-based Inventory Management System** provides a robust and user-friendly solution for managing parts and products.

## Features
- **User-Friendly GUI**: Built with JavaFX for a smooth and interactive interface.
- **Inventory Management**: Add, modify, delete, and search for parts and products.
- **Product-Part Association**: Assign parts to products and manage dependencies.
- **Validation & Error Handling**: Ensures data integrity with real-time validation.
- **Custom Business Logic**: Implements BiSquare’s specific requirements, such as inventory constraints and pricing rules.

## Technologies Used
- **Java 8+** (Core Programming)
- **JavaFX** (GUI Development)
- **FXML** (UI Layout Definition)
- **MVC Architecture** (Separation of Concerns)
- **NetBeans IDE** (Recommended for development)

## Application Screens

### 📌 Main Screen
- Options to **Add, Modify, Delete, and Search** for Parts & Products.
- Displays inventory lists with details.

![Main Screen](https://user-images.githubusercontent.com/10691766/29241971-0bdc88e4-7fa6-11e7-86c8-2db7917762af.jpg)

### 📌 Add Part Screen
- Choose between **In-House** and **Outsourced** parts.
- Enter **ID, Name, Inventory Level, Price, Min/Max Values, Machine ID/Company Name**.

![Add Part](https://user-images.githubusercontent.com/10691766/29241970-0bd8bec6-7fa6-11e7-9b10-189f74b6d96f.jpg)

### 📌 Modify Part Screen
- Modify an existing part with **pre-filled data**.

![Modify Part](https://user-images.githubusercontent.com/10691766/29241972-0beba4dc-7fa6-11e7-8747-e9356307d791.jpg)

### 📌 Add Product Screen
- Add new products and **associate parts** with them.
- Search and assign parts.

![Add Product](https://user-images.githubusercontent.com/10691766/29241969-0bd16c34-7fa6-11e7-99ca-ff4212e3d545.jpg)

### 📌 Modify Product Screen
- Modify existing products and update associated parts.

![Modify Product](https://user-images.githubusercontent.com/10691766/29241967-0bcc2e5e-7fa6-11e7-890b-75e15b0a49eb.jpg)

### ⚠️ Delete Confirmation
- Prevents accidental deletion of products with associated parts.

![Delete Confirmation](https://user-images.githubusercontent.com/10691766/29241968-0bcf2d52-7fa6-11e7-88c6-5a4f6dc6594b.jpg)

## System Architecture
The system follows the **Model-View-Controller (MVC)** architecture:

- **Model**: Manages business logic and data.
- **View**: Defines the UI using JavaFX and FXML.
- **Controller**: Handles user interactions and updates the model.

## Business Logic & Validations
✔ A product **must have at least one** associated part.  
✔ Products **cannot be deleted** if parts are assigned.  
✔ Inventory levels **must be within min/max constraints**.  
✔ Product price **cannot be lower** than the total cost of its parts.  
✔ **Confirmation dialogs** for all Delete & Cancel actions.  

## Setup & Installation
### Prerequisites
- **Java 8+**
- **JavaFX SDK** (If using Java 8, as newer versions include JavaFX)
- **NetBeans IDE (Recommended)**

### Steps to Run
1. Clone the repository:
   ```sh
   git clone 
2. Open the project in NetBeans.
3. Run the application.
