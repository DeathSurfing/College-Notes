____
## Objective:

To learn how to install **MySQL Server** and **MySQL Workbench** on different operating systems (Windows, macOS, and Linux), enabling database management and query execution.

This lab provides step-by-step instructions to install **MySQL Server** and **MySQL Workbench** on **Windows**, **macOS**, and **Linux**.

---

## 1. Installation on Windows

### Step 1: Download MySQL Installer
- Visit https://dev.mysql.com/downloads/installer/
- Download **MySQL Installer for Windows**.
``
### Step 2: Run Installer
- Run the downloaded installer (`mysql-installer-community-*.exe`).
- Choose the setup type:
  - **Developer Default** (Recommended)
  - **Server only**
  - **Client only**
- Click **Next**.

### Step 3: Configure MySQL Server
- Set the root password.
- Optionally, create a user account.
- Configure MySQL as a Windows service.

### Step 4: Install MySQL Workbench
- During installation, ensure **MySQL Workbench** is selected.
- Complete installation.

### Step 5: Verify Installation
- Open MySQL Workbench.
- Connect to `localhost` using root credentials.
- Run a test query:
  ```sql
  SELECT VERSION();
  ```

---

##  2. Installation on macOS

### Step 1: Download MySQL DMG
- Visit https://dev.mysql.com/downloads/mysql/
- Download the macOS DMG archive.

### Step 2: Install MySQL Server
- Open the DMG file.
- Run the MySQL installer package.
- Follow the installation wizard.
- Set a root password.

### Step 3: Install MySQL Workbench
- Visit https://dev.mysql.com/downloads/workbench/
- Download and install **MySQL Workbench for macOS**.

### Step 4: Start MySQL Server
- Use System Preferences → MySQL → Start MySQL Server.
- Alternatively, use terminal:
  ```bash
  sudo /usr/local/mysql/support-files/mysql.server start
  ```

### Step 5: Verify Installation
- Open MySQL Workbench.
- Connect to `localhost` with root credentials.
- Run a test query:
  ```sql
  SELECT VERSION();
  ```

---

##  3. Installation on Linux (Ubuntu)

### Step 1: Update Package Repository
```bash
sudo apt update
```

### Step 2: Install MySQL Server
```bash
sudo apt install mysql-server
```

### Step 3: Secure MySQL Installation
```bash
sudo mysql_secure_installation
```
- Set root password, remove anonymous users, disallow remote root login, and remove test database.

### Step 4: Install MySQL Workbench
```bash
sudo apt install mysql-workbench
```

### Step 5: Start MySQL Service
```bash
sudo systemctl start mysql
sudo systemctl enable mysql
```

### Step 6: Verify Installation
- Open MySQL Workbench.
- Connect to `localhost` with root credentials.
- Run a test query:
  ```sql
  SELECT VERSION();
  ```


