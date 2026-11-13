# mongoDB-estructura
# TascaS2.03
MongoDB 

Exercises to learn NoSQL Document Database Design, Schema Validation, and Data Modeling using MongoDB Collections, Embedded Documents, References & JSON Schemas

# MongoDB NoSQL Database Design
Welcome to my MongoDB database learning repository! This space is dedicated to collecting practical exercises, document schemas, and data models regarding NoSQL Database Design that I develop as I progress through my training by ITAcademy.

## 🚀 Development Environment
- **Database Server:** MongoDB (Community Server)
- **Design & Administration Tool:** MongoDB Compass
- **Database Shell:** MongoDB Shell (`mongosh`)
- **Editor:** Visual Studio Code

## 📂 Repository Structure
The project is currently focused on the foundational NoSQL database designs corresponding to **Nivel 1**. Higher difficulty levels will be added as they are completed.

### 📌 Nivel 1
- **optica_cliente/** : Document-oriented database model for the "Cul d'Ampolla" optics store, structured from the **Customer View** and **Glasses View**
  - `cul_d_ampolla.clientes.js` / `.json` : Script and JSON schema defining the collection structure, validation rules, and sample data population.

  - `cul_d_ampolla.gafas.js` / `.json` : Script and JSON schema defining the collection structure, validation rules, and sample data population.

### ⏳ Nivel 2 & Nivel 3
- *Work in Progress* 🛠️: Advanced NoSQL schemas, complex aggregations, and multi-collection modeling exercises will be uploaded here upon completion.

## 🛠️ How to Run This Project
To set up, inspect, and test these databases, you will need a running MongoDB instance and administration tools like **MongoDB Compass**. Follow these steps to execute the code:

1. **Clone this repository:** Navigate to your local projects directory and clone the repository:
   ```bash
   git clone https://github.com/JoseBermejo-N/mongoDB-estructura.git
   cd mongoDB-estructura
   ```
2. **Open MongoDB Compass:** Connect to your local (`mongodb://localhost:27017`) or remote MongoDB server instance.
3. **Create Database & Collections:**
   - Create a new database (e.g., `optica`).
   - Create the corresponding collections (`clientes` or `gafas`).
4. **Import Data & Schemas:**
   - Select the target collection in MongoDB Compass, click **Add Data -> Import JSON or CSV file**, and select the `.json` files from their respective folders.
   - *(Optional)* Apply the JSON Schema validation rules in the **Validation** tab of each collection.

Alternatively, you can run the scripts or import files directly via the terminal:

1. **Using `mongoimport` (for `.json` data files):**
   ```bash
   mongoimport --db optica --collection clientes --file ruta/al/proyecto/cul_d_ampolla.clientes.json --jsonArray
   ```
2. **Using `mongosh` (for `.js` scripts):**
   ```bash
   mongosh
   load("C:/ruta/al/proyecto/cul_d_ampolla.clientes.js")
   ```

Jose - [@JoseBermejo-N](https://github.com/JoseBermejo-N)
