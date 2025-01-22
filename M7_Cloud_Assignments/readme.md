# Azure Cloud Exercises

## Exercise 1: Create and Configure VMs
### Ubuntu VM
- **Task:** Create an Ubuntu Server 20.04 LTS virtual machine on Azure.
- **Steps:**
  1. Configure SSH for secure access.
  2. Allow inbound port 22 for SSH connections.
  3. Install Apache (`sudo apt update && sudo apt install apache2`).
  4. Verify by accessing the default Apache page in your browser using the VM's public IP.

### Windows VM
- **Task:** Create a Windows Server 2022 virtual machine on Azure.
- **Steps:**
  1. Configure a username and password for access.
  2. Allow inbound port 3389 for Remote Desktop Protocol (RDP).
  3. Install IIS:
     - Open **Server Manager** > **Add roles and features** > Install **Web Server (IIS)**.
  4. Verify by accessing the default IIS page in your browser using the VM's public IP.

---

## Exercise 2: Deploy Static Web App
### Task:
- Deploy a static website using Azure App Service.
### Steps:
1. Create an App Service with the following configuration:
   - **Runtime:** Python 3.10
   - **OS:** Linux
2. Upload a static website (e.g., `index.html`) via Azure portal or FTP.
3. Verify the deployment by accessing the public URL of the App Service.
4. Modify `index.html` to include a welcome message and confirm the changes are reflected.

---

## Exercise 3: Deploy Flask App
### Task:
- Deploy a Flask application to Azure App Service.
### Steps:
1. Create a simple Flask application and push the code to GitHub.
2. Deploy the Flask app to Azure App Service:
   - **Runtime:** Python 3.10
   - **Deployment Source:** GitHub repository.
3. Verify the app by accessing its public URL.

---

## Exercise 4: Set Up Azure SQL Database
### Task:
- Create an SQL database on Azure and interact with it.
### Steps:
1. Create a database named `StudentDB` on Azure SQL.
2. Use Azure Data Studio or SQL Server Management Studio (SSMS) to:
   - Connect to `StudentDB`.
   - Create a table `Students` with columns for student details.
   - Insert and query sample data to verify the setup.

---

## Exercise 5: Integrate Flask with Azure SQL
### Task:
- Modify the Flask app to perform CRUD operations with Azure SQL.
### Steps:
1. Install `pyodbc` in your Flask app environment to connect to the Azure SQL database.
2. Update the Flask application to perform the following:
   - Create, Read, Update, and Delete (CRUD) operations on the `Students` table in `StudentDB`.
3. Deploy the updated app to Azure App Service.
4. Verify the functionality by testing the app's endpoints with CRUD operations.

---

