# 🌐 SocialWeb-Simulator - Connect with friends through simple tools

[![Download SocialWeb-Simulator](https://img.shields.io/badge/Download-SocialWeb--Simulator-blue) ](https://github.com/Faiktalhasezer1122/SocialWeb-Simulator/releases)

## 📌 Project Overview
SocialWeb-Simulator acts as a demonstration of modern web communication. This application provides a space to register accounts and exchange messages with other users. It runs on your local machine and uses common database tools to save your information. You can test different ways to store data by changing simple text settings in the configuration file.

## ⚙️ System Requirements
Ensure your computer meets these requirements before you begin:

*   **Operating System:** Windows 10 or Windows 11.
*   **Processor:** Any modern dual-core processor.
*   **Memory:** 4 GB of RAM or more.
*   **Storage:** 500 MB of free space.
*   **Software:** You must have the .NET Desktop Runtime installed. If your computer lacks this, the installer will prompt you to download it from the official Microsoft website.

## 📥 Getting Started
Follow these steps to set up the software on your machine:

1.  Visit the [releases page](https://github.com/Faiktalhasezer1122/SocialWeb-Simulator/releases) to download the application.
2.  Locate the latest version link on the page.
3.  Download the compressed folder to your computer.
4.  Right-click the folder and select "Extract All" to see the application files.
5.  Open the folder containing the extracted files.
6.  Look for the file named `SocialWeb-Simulator.exe`.
7.  Double-click this file to launch the application.

## 🛠️ Configuration Settings
The software allows you to choose how it saves your data. You can modify these choices in the `appsettings.json` file found within the application folder. Open this file with a basic text editor like Notepad.

*   **Database Types:** You can switch between Dapper, Entity Framework Core, or in-memory storage.
*   **Repository Selection:** Change the value associated with the repository setting to match your preferred storage method. 
*   **Saving Changes:** Save the file after you make your changes and restart the application for the updates to take effect.

## 🔐 Registration and Authentication
Once the application starts, it presents a login screen. You can create a new account by clicking the registration link. Provide a username and a password to secure your account. 

Authentication happens locally. The system verifies your credentials against the database you selected in the configuration file. Once you log in, you gain access to the main dashboard where you can begin messaging other users registered in your local instance.

## 📂 Understanding Data Persistence
The software functions as a layer between your input and your database. When you send a message, the system routes your data through the active repository implementation. 

*   **Dapper:** Uses simple queries to map your data directly to the database.
*   **Entity Framework Core:** Uses a higher-level structure to manage complex relationships between users and their messages.
*   **In-Memory:** Stores all information in your computer's temporary memory. This data clears when you close the application. Use this for testing purposes only.

## 🔧 Troubleshooting Tips
If the application fails to start, verify the following:

*   **Runtime Errors:** Confirm that the .NET Runtime is current. If unsure, visit the Microsoft website and download the latest version.
*   **Permissions:** Ensure your user account has permission to write to the folder where you extracted the application.
*   **SQL Server:** If you select SQL Server as your database, ensure the server instance is running and reachable on your network.
*   **Port Conflicts:** The application uses default web ports. If another service restricts these ports, the application may fail to open the web interface. Close other web-based software to free up the network ports.

## 📜 Project Background
This project serves as a practical exercise in software architecture. It demonstrates how to decouple application logic from data storage. By using interfaces, the code remains flexible. You can swap storage methods without changing the features that users see. This design pattern ensures that the software stays clean and manageable.

The project incorporates standard web technologies to provide a smooth user experience. The interface loads quickly in your browser, allowing you to manage your profile and conversations without delay.

## ℹ️ Support and Updates
The repository tracks all changes and improvements in the release notes. Check the main page periodically to see if a newer version of the software is available. If you encounter issues while using the application, review the documentation sections provided above. The setup remains consistent across all versions to ensure a stable experience as the project evolves. 

Keep your configuration files backed up if you decide to upgrade to a newer version of the application. This prevents the loss of your account registration details or message history during the update process.