
# GameSaveDoxData

**GameSaveDoxData** is a game save file management tool that allows users to scan their local directories for save files, synchronize them with their Dropbox account, and efficiently manage them through an intuitive interface.

## Main Features

1. **Directory Scanning**:  
   The application scans specific directories on the user's system to find game save files.

2. **Dropbox Synchronization**:  
   Users can log in to their Dropbox account and sync their game save files with the cloud.

3. **File Management**:  
   Users can download, delete, and update the list of game save files stored in their Dropbox account.

4. **Intuitive User Interface**:  
   The app offers an easy-to-use interface, with options to select and manage files efficiently.

## How to Use the Application

### Prerequisites
- A Dropbox account.
- A Dropbox API key (you can get it from the [Dropbox Developer Dashboard](https://www.dropbox.com/developers/apps)).

### Steps to Set Up and Use the Application

1. **Log in to Dropbox**:
   - Open the application and locate the **"Dropbox"** button in the bottom-left corner.
   - Click the **"Dropbox"** button and paste the API key into the corresponding field.
   - Click the **"Validate"** button to verify the key. If valid, the LED indicator will turn green.

2. **Obtain the Dropbox API Key (Optional)**:
   - Go to the [Dropbox Developer Dashboard](https://www.dropbox.com/developers/apps).
   - Create a new app with **"Full Dropbox"** access.
   - Copy the generated API key.

3. **Scan for Files**:
   - Enter the PC username in the corresponding field.
   - Click the **"Search"** button to scan the user's folders for game save files.

4. **Sync with Dropbox**:
   - Select the files you want to sync.
   - Click the **"Dropbox ⇵"** button to synchronize the selected files with your Dropbox account.

5. **Manage Files in Dropbox**:
   - Click the **"Dropbox ☁"** button to open the Dropbox management window.
   - From there, you can download, delete, or update the list of files in your Dropbox account.

---

### Main Buttons and Functions

- **"Dropbox" Button**:  
  - Located in the bottom-left corner, it allows you to enter your Dropbox API key.
  - Click this button, paste the API key, and validate it with the **"Validate"** button.

- **"Validate" Button**: Validates the Dropbox API key.  
- **"Login with Dropbox" Button**: Logs in to Dropbox.  
- **"Search" Button**: Scans the user's folders for save files.  
- **"Dropbox ⇵" Button**: Syncs files with Dropbox.  
- **"Dropbox ☁" Button**: Opens the Dropbox management window.  
- **"PC 🖥" Button**: Scans the PC for save files.  
- **"♡" Button**: Closes the application.  

---

## Dropbox API Integration

The application uses the Dropbox API to authenticate users and manage files. Here's the integration flow:

1. **Authentication with Dropbox**:
   - The app uses OAuth 2.0 to authenticate users.
   - The user logs in to Dropbox, and the app receives an access token.

2. **File Synchronization**:
   - The app uses the access token to make API calls to Dropbox.
   - Operations include listing, downloading, deleting, and uploading files.

3. **API Calls**:
   - `Files.ListFolderAsync`: Lists files and folders in Dropbox.
   - `Files.DownloadAsync`: Downloads files from Dropbox.
   - `Files.DeleteV2Async`: Deletes files from Dropbox.
   - `Files.UploadAsync`: Uploads files to Dropbox.

---

## Privacy Policy

The application collects and stores the Dropbox API key and the PC username to manage save files. We do not share this information with third parties. For more details, consult our [Privacy Policy](https://docs.google.com/document/d/1Nx1AiREQtFlXOAXRFG812Kg21NW0BOLdmUEjV1Jfeg4/edit?usp=sharing).

![GameSavesDoxData v1](https://github.com/user-attachments/assets/f4aba752-a4de-4933-9fa2-7c01ccafe5ab)
