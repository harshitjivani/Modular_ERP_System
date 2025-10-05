# 🧩 Modular ERP System (Axelor Framework)

## 📘 Overview
The **Modular ERP System** is an enterprise-grade application developed using the **Axelor Open Platform**.  
It streamlines and automates key business operations through **modular architecture** and **domain-driven design**.  
The project integrates essential modules such as:
- **Contact Management**
- **Sales Management**
- **Invoice Management**
- **Account & Move Management**

Each module operates independently but integrates seamlessly with others through Axelor’s robust service and ORM layer.

---

## 🎯 Objectives
- Develop a **modular and scalable ERP** using the **Axelor Framework**.  
- Automate business processes such as **Sales, Accounting, and Invoicing**.  
- Implement **Role-Based Access Control (RBAC)** for secure user management.  
- Provide **CSV import functionality** for batch data integration.  
- Enable **custom business logic** using Java and Axelor Action scripts.  

---

## ⚙️ Technology Stack

| Category | Tools / Technologies |
|-----------|----------------------|
| **Framework** | Axelor Open Platform |
| **Backend** | Java 17, Hibernate ORM, JPA |
| **Database** | PostgreSQL 15 |
| **Build Tool** | Gradle |
| **IDE** | Eclipse / IntelliJ IDEA |
| **Testing Tools** | Postman, JUnit |
| **Version Control** | Git & GitHub |
| **API Framework** | RESTEasy |
| **Dependency Injection** | Google Guice, Spring Core |

---

## 🧠 Modules Implemented

### 1. Contact Module
- Manage customer contact details and addresses.  
- Auto-generate full names and validate data integrity.  
- Linked with Account and Invoice modules.  

### 2. Sales Module
- Create and manage **Sales Orders** and **Order Lines**.  
- Integrate with products, prices, and tax calculation.  
- Enable sales-to-invoice conversion.  

### 3. Invoice Module
- Handle **Invoice Creation, Merging, and Cancellation**.  
- Generate totals dynamically and track statuses.  
- Implemented **invoice merge feature** via service & controller integration.  

### 4. Account & Move Module
- Manage **financial transactions**, debit/credit entries.  
- Auto-generate **Move Lines** linked to invoices.  
- Maintain **financial consistency** and audit tracking.  

---

## 🧩 Additional Features
- **Dashboard & Reporting:** Visual KPIs using charts for sales and revenue.  
- **Role-Based Access Control:** Secure module-level permissions.  
- **CSV Import:** Simplifies bulk data onboarding.  
- **Low-Code Integration:** Combine XML configuration with Java logic.  

---

## 🧪 Testing
- **Unit Testing:** Module-level entity and service validation.  
- **Integration Testing:** Cross-module data flow (Contact → Sales → Invoice → Account).  
- **Functional Testing:** Validation of forms, actions, and expressions.  
- **JUnit & Postman:** For controller and REST API testing.  

---

## 🚀 Setup & Run Instructions

### 1️⃣ Clone the Repository & Build the Project

```bash
# Clone the repository
https://github.com/harshitjivani/Modular_ERP_System.git
cd Modular_ERP_System/module

# Build the project using Gradle Wrapper (no manual Gradle installation required)
./gradlew clean build
```

🧠 **Note:**
- The `clean` command deletes previously compiled files.  
- The `build` command compiles the code, runs tests, and generates necessary artifacts.  
- On **Windows**, use `gradlew.bat` instead of `./gradlew`.  
- After a successful build, you should see:  
  ```
  BUILD SUCCESSFUL
  ```

---

### 2️⃣ Run the Application

To start the application locally, use:

```bash
./gradlew run
```

⚙️ This command launches the embedded **Tomcat server** and deploys the **Axelor ERP** application.  

Once the server starts, you’ll see:
```
Tomcat started on port(s): 8080 (http)
```

---

### 3️⃣ Access the Application

Open your browser and go to:

```bash
http://localhost:8080/axelor-erp
```

🧭 **Default Credentials:**
- **Username:** `admin`  
- **Password:** `admin`

---

### 4️⃣ Database Configuration

Update your PostgreSQL credentials in:

```
src/main/resources/application.properties
```

**Example configuration:**
```properties
db.default.driver=org.postgresql.Driver
db.default.url=jdbc:postgresql://localhost:5432/axelor_erp
db.default.user=postgres
db.default.password=yourpassword
```

---

### 5️⃣ Import Sample Data (Optional)

To load demo data or CSV imports:

1. Go to **Axelor → Data Import Tool** in the web UI.  
2. Choose your CSV file from the `/import/` folder.  
3. Map the fields and click **Import**.

---

### 6️⃣ Stop the Application

To stop the running server, press:
```bash
CTRL + C
```

Or stop it explicitly via Gradle:
```bash
./gradlew --stop
```

---

### 📈 Future Enhancements

- Integration of **Inventory** & **HR** modules.  
- Addition of **real-time analytics dashboards**.  
- Implementation of **BIRT-based PDF reports**.  
- **REST API** enhancements for external integration.

---

### 👨‍💻 Developer

**Harshit Jivani**  
_Bachelor of Technology in Information Technology_  
**Organization:** Axelor Technologies India Pvt. Ltd.


