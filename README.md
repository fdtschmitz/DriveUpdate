# DriveUpdate
Simple usage of the PyDrive2 library. Iterate through a Google Drive root folder and return a list of folders and files.

# Context
The implementation idea arose from the need to create an index and update it for a public repository of books.

# Before Getting Started
To make the code work, it's necessary to generate authentication keys in the Google Cloud Console at https://console.cloud.google.com/.

Create a new project and search for APIs and Services. Before generating the key, you'll need to configure the OAuth consent screen; Select the user type. Since we're using the free version, we only have access to the External option. Click on Create.

On the next screen, provide the name of your app, your support email, and the developer contact. Click Save and Continue. You can leave the Scope field empty for now.

In the Test users screen, you need to add the users who will use this code. Even if it's just you, you need to enter your email. Click "Add User" to enter the email. Save and finish the configuration.

Back to the dashboard, go to Credentials and click Create Credentials. Select OAuth client ID. For this example, select Desktop app. Give a name to the key and click Create. On the screen that appears, you'll be able to download the JSON file that we will use in the code. It needs to be in the same project folder.

Prerequisites
This code uses the PyDrive2 library. Visit the project page to see how to install it: https://github.com/iterative/PyDrive2/

We will also use the openpyxl library. Documentation can be found here: https://openpyxl.readthedocs.io/

