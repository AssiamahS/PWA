# Text Editor Application
## Author: Sylvester Assiamah - Module 19

## Description

This Text Editor application allows users to create and manage notes or code snippets, with or without an internet connection. The app is designed as a progressive web application (PWA) that functions offline and meets the criteria for PWA. Data persistence techniques, including IndexedDB, ensure reliable storage and retrieval of content, even when offline. The codebase has been meticulously developed and optimized to provide seamless functionality and a smooth user experience.

## Visuals

![Text Editor Landing Page](assets/images/TextEditorLandingPage.png)

![Text Editor Functionality](assets/images/TextEditorFunctionality.png)

## Deployment

Access the deployed application via this link: [Text Editor Application](hhttps://github.com/AssiamahS/PWA.git)

## Usage

1. Start the application:
    ```bash
    npm start
    ```

2. Open your browser and navigate to:
    ```
    http://localhost:3000
    ```

3. You will be presented with the text editor interface. Enter content and click off the window to save it automatically to IndexedDB. Reopen the editor to retrieve saved content.

## Features

- Single-page application with client-server folder structure.
- Next-gen JavaScript used with webpack bundling.
- IndexedDB for immediate database storage.
- Service worker for offline functionality.
- Install button for desktop icon download.
- Static assets pre-cached with workbox.
- Proper build scripts for webpack application.

## Deployment

This application can be easily deployed using Render.

1. Create a `render.yaml` file in the root directory with the following content:

    ```yaml
    services:
      - type: web
        name: text-editor
        env: node
        region: oregon
        buildCommand: npm install
        startCommand: node server.js
    ```

2. Push all changes to your GitHub repository.

3. Go to [Render](https://render.com/) and create a new account if you don't have one.

4. Click on "New +" and choose "Web Service".

5. Connect your GitHub account and select the repository you created.

6. Render will automatically detect the `render.yaml` file and configure the deployment settings.

7. Click "Create Web Service" to deploy your application.

## Credits

- ASKBCS - Assisted in setting up the deployment configurations.

## License

Please refer to the LICENSE file in the repository.
