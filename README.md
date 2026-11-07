
<div align="center">

# 📊 Rekon Analytics – Education Planning Analysis System

Bridging Education Insights and School Planning Through Intelligent Analysis.

A web-based application designed to analyze the alignment of School Annual Work Plans (RKT) and School Activity and Budget Plans (RKAS) with Education Report (Rapor Pendidikan) data. Powered by structured data matching, rule-based validation, and Google Gemini AI to provide meaningful insights and actionable recommendations for better school planning.

![Laravel](https://img.shields.io/badge/Laravel-11-FF2D20?logo=laravel&logoColor=white)
![React](https://img.shields.io/badge/React-18-61DAFB?logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-3-06B6D4?logo=tailwindcss&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-6-646CFF?logo=vite&logoColor=white)
![Gemini](https://img.shields.io/badge/AI-Gemini-8E75B2?logo=googlegemini&logoColor=white)

</div>

## Acknowledgements

 - [Laravel 11 Documentation](https://laravel.com/docs/11.x)
 - [Learn React JS](https://react.dev/learn)
 - [Template Component Documentation](https://ui.shadcn.com/)
 - [Tailwind CSS Documentation](https://tailwindcss.com/)


## Important Notes

We’re using Laravel for the backend and ReactJS for the frontend! 🚀
• We’ve wrapped it all up with Shadcn for templates and Tailwind CSS for styling! 🌟
• Tailwind makes styling a breeze—no separate CSS files needed! 🙌
This combination is sure to make development smooth and fun! Let’s rock this project! 💪


## ✨ Core Features

**Rekon Analytics** provides several integrated features to support the evaluation and improvement of **school planning documents**.

### 📥 Education Report Excel Import

| Feature | Description |
|---|---|
| 📂 **Excel Workbook Upload** | Import school planning data from an Excel workbook |
| 🔎 **Automated Data Extraction** | Extract relevant information from multiple workbook sheets |
| 🧱 **Structured Data Mapping** | Transform spreadsheet data into structured application records |
| 🏫 **School Information Extraction** | Identify school names and reporting years from the uploaded workbook |
| ⚙️ **Data Processing** | Prepare educational priorities, root problems, RKT activities, and RKAS information for analysis |

### 🎯 RKT Alignment Analysis

| Feature | Description |
|---|---|
| 🧭 **Priority Identification Matching** | Compare RKT identification indicators against Education Report priorities |
| 🌱 **Root Problem Matching** | Evaluate the relationship between planned activities and identified educational problems |
| 🛠️ **Improvement Activity Evaluation** | Assess whether proposed improvement activities directly address identified root problems |
| 📝 **Implementation Evaluation** | Analyze whether implementation descriptions are specific and meaningful follow-up activities |
| 🧮 **Alignment Scoring** | Calculate an overall score from multiple assessment components |
| 🧩 **Independent Program Identification** | Distinguish activities that are not based on Education Report priorities |

### 🤖 AI-Powered Evaluation with Google Gemini

| Feature | Description |
|---|---|
| 🧠 **AI-Based Activity Assessment** | Evaluate the quality and relevance of improvement activities |
| 🔬 **Implementation Quality Assessment** | Check whether implementation activities are specific, operational, and derived from improvement activities |
| 💡 **Automated Recommendations** | Generate practical suggestions for improving activities |
| 🗺️ **Contextual Evaluation** | Consider identified root problems and reference activities during assessment |

**Consistent scoring rubric** – results are classified into three levels:

| Level | Score Range |
|---|:---:|
| 🟢 **Good** (*Baik*) | 0.80 – 1.00 |
| 🟡 **Fair** (*Cukup*) | 0.50 – 0.79 |
| 🔴 **Poor** (*Kurang*) | 0.00 – 0.49 |

### ✍️ RKT Recommendation Generation

| Feature | Description |
|---|---|
| 🚩 **Missing Priority Identification** | Identify educational priorities not yet addressed in the RKT |
| 📌 **Improvement Suggestions** | Generate recommended improvement activities from Education Report data |
| 🔧 **Implementation Recommendations** | Generate more specific implementation descriptions |
| 👀 **Recommendation Review** | Let users review suggested improvements |
| ✅ **Recommendation Acceptance** | Apply accepted suggestions to the matching RKT records |

### 💰 RKAS and ARKAS Analysis

| Feature | Description |
|---|---|
| 🔗 **RKT-to-RKAS Alignment** | Check whether budget activities support the matching RKT improvement activities |
| 📚 **ARKAS Activity Validation** | Compare budget activity names against official reference datasets |
| 🛒 **Goods and Services Validation** | Check budget descriptions against reference goods and services |
| 📏 **Unit Validation** | Verify that selected units match reference data |
| 🏷️ **Unit Price Validation** | Flag prices that exceed reference maximum prices |
| ➗ **Budget Calculation Validation** | Check that total price equals quantity × unit price |
| ⚠️ **Budget Consistency Monitoring** | Highlight potential inconsistencies through visual warnings |

### 🧾 AI-Powered RKAS Recommendations

| Feature | Description |
|---|---|
| 📋 **Automated Budget Recommendations** | Generate draft RKAS details based on RKT activities |
| 🔍 **Activity Reference Matching** | Suggest relevant ARKAS activities using reference datasets |
| 📦 **Goods and Services Recommendations** | Recommend relevant items, units, and reference prices |
| 📅 **Budget Scheduling** | Suggest implementation months |
| 💵 **Quantity and Cost Estimation** | Generate suggested quantities, unit prices, and total costs |
| 🔒 **Reference-Based Generation** | Restrict recommendations to available reference candidates instead of inventing activity or product names |

### 🗄️ Report Management

| Feature | Description |
|---|---|
| 🕘 **Analysis History** | View previously processed school reports |
| 📄 **Report Details** | Explore detailed RKT and RKAS analysis results |
| 🔎 **Search and Filtering** | Find reports by school name and reporting year |
| 🗑️ **Report Deletion** | Remove existing analysis records |
| 🔐 **User Authentication** | Secure access through authenticated sessions |
| 👤 **Profile Management** | Update user profile information |


# Installation Guide

This guide provides step-by-step instructions to install **PHP 8.2**, **Node.js 20** using **NVM** (Node Version Manager), and **MySQL** for both **Linux** and **Windows** users.

---

## **1. Install PHP 8.2**

### **For Linux Users**

#### **Step 1.1: Update the System**
Run the following command to update the package manager and system packages:
```bash
sudo apt update && sudo apt upgrade -y
```

#### **Step 1.2: Add PHP Repository**
Add the PHP PPA (Personal Package Archive) to your system:
```bash
sudo add-apt-repository ppa:ondrej/php
sudo apt update
```

#### **Step 1.3: Install PHP 8.2**
Install PHP 8.2 along with common extensions:
```bash
sudo apt install php8.2 php8.2-cli php8.2-fpm php8.2-mysql php8.2-xml php8.2-curl php8.2-mbstring php8.2-zip php8.2-intl -y
```

#### **Step 1.4: Verify Installation**
Check the installed PHP version:
```bash
php -v
```

### **For Windows Users**

#### **Step 1.1: Download PHP**
Visit the official PHP download page: https://windows.php.net/download/
Download the Thread Safe zip file for PHP 8.2.

#### **Step 1.2: Extract PHP**
Extract the downloaded ZIP file to a directory, e.g., C:\php.

#### **Step 1.3: Configure PHP**
Add the PHP directory to your system's PATH environment variable:

Open Control Panel → System → Advanced system settings → Environment Variables.
In the System variables section, find and edit the Path variable.
Add the full path to your PHP folder, e.g., C:\php.
Rename php.ini-development to php.ini in the extracted folder.

#### **Step 1.4: Verify Installation**
Open a command prompt and run:
```bash
php -v
```


## **2. Install Node.js 20 Using NVM**
### **For Linux Users**
#### **Step 2.1: Install NVM**
Download and install the latest version of NVM ([you can read for more detail from here](https://github.com/nvm-sh/nvm?tab=readme-ov-file#installing-and-updating)):

```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.5/install.sh | bash
```

#### **Step 2.2: Activate NVM
Reload your shell to activate NVM:
```bash
export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
```
Alternatively, close and reopen your terminal.

#### **Step 2.3: Install Node.js 20**
Install Node.js 20 using NVM:

```bash
nvm install 20
```
#### **Step 2.4: Use Node.js 20**

Set Node.js 20 as the default version:
```bash
nvm use 20
nvm alias default 20
```
#### **Step 2.5: Verify Installation**
Check the installed Node.js and npm versions:
```bash
node -v
npm -v
```

### **For Windows Users**
#### **Step 2.1: Install NVM for Windows**
Download NVM for Windows from the official repository: https://github.com/coreybutler/nvm-windows/releases.
Install NVM using the downloaded installer.
#### **Step 2.2: Configure NVM**
During installation:

Select a directory for NVM (e.g., C:\nvm).
Select a directory for global Node.js installations (e.g., C:\Program Files\nodejs).
#### **Step 2.3: Install Node.js 20**
Open a command prompt and run:

```bash
nvm install 20
nvm use 20
```

#### **Step 2.4: Verify Installation**
Check the installed Node.js and npm versions:

```bash
node -v
npm -v
```

## **3. Install MySQL**

### **For Windows Users**

#### **Step 3.1: Download MySQL Installer**
Visit the official MySQL download page: https://dev.mysql.com/downloads/installer/
Download the **mysql-installer-web-community** or **mysql-installer-community** version.

#### **Step 3.2: Install MySQL Server**
1. Run the downloaded installer.
2. Choose **Custom** or **Developer Default** setup type.
3. Ensure **MySQL Server** is selected.
4. Click **Next** and follow the installation wizard.

#### **Step 3.3: Configure MySQL**
1. Set the **Root Password** (remember this for your `.env` file).
2. Create a new user if needed.
3. Keep the default port **3306**.
4. Complete the configuration and finish the installation.

#### **Step 3.4: Verify Installation**
Open the **MySQL Command Line Client** or use a terminal:
```bash
mysql -u root -p
```
Enter the password you set during installation.

## *Summary*
- PHP 8.2, Node.js 20, and MySQL are installed successfully on your system.
- Linux users installed Node.js 20 using NVM for Linux.
- Windows users installed Node.js 20 using NVM for Windows and MySQL using the installer.

For additional support, refer to:

- [PHP Documentation](https://www.php.net/manual/en/install.php)
- [NVM for Linux](https://github.com/nvm-sh/nvm)
- [NVM for Windows](https://github.com/coreybutler/nvm-windows)
- [MySQL Documentation](https://dev.mysql.com/doc/)
## Run Locally

### Install dependencies

*Install Node Dependencies*
```bash
  npm install
```

*Install PHP Dependencies*
```bash
  composer install
```

### Create environment

- rename file .env.example into .env
- generate APP_KEY:
```bash
php artisan key:generate
```
- adjust the database section:
```
DB_CONNECTION=sqlite
# DB_HOST=127.0.0.1
# DB_PORT=3306
# DB_DATABASE=laravel
# DB_USERNAME=root
# DB_PASSWORD=
```
into:
```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=database_name (rekon)
DB_USERNAME=mysql_username (root)
DB_PASSWORD=mysql_password (root_pass)
```
- add Gemini API configuration:
```
VITE_GEMINI_API_KEY=GEMINI_API_KEY
VITE_AI_MODEL=gemini-2.5-flash-lite
```


### Migrate database
Open terminal / bash then type command:
```bash
php artisan migrate
```

### Generate your first admin account
Open terminal / bash then type command:
```bash
php artisan db:seed --class=AdminSeeder
```
it will creating user: superadmin@rekon.com / qwerty123

### Start Run Locally
Open terminal / bash then type command:
```bash
php artisan serve
```

Open another terminal / bash then type command:
```bash
npm run dev
```

### Build locally
Open terminal / bash then type command:
```bash
npm run build
```
then start it using:
```bash
php artisan serve
```
