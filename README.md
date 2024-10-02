
![Project Horizon](./thumb.png)

# Set up a personal website

## Step 1: Install Node JS

### Windows

1. Visit the [Node.js Website](https://nodejs.org/)
2. Download the Windows Installer (.msi) for the LTS version.
3. Run the installer and follow the installation wizard.
4. Verify the installation by opening Command Prompt and typing:

   ```bash
   node --version
   npm --version
   ```

### macOS

#### Using the Official Installer

1. Visit the [Node.js Website](https://nodejs.org/)
2. Download the macOS Installer (.pkg) for the LTS version.
3. Run the installer and follow the installation wizard.

Verify the installation by opening Terminal and typing:

```bash
node --version
npm --version
```

#### Using Homebrew

1. Install Homebrew if not already installed:

   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

2. Install Node.js:

   ```bash
   brew install node
   ```

## Linux (Ubuntu/Debian)

1. Update your package index:

   ```bash
   sudo apt update
   ```

2. Install Node.js from the repositories:

   ```bash
   sudo apt install nodejs npm
   ```

For the latest version, you can use the NodeSource repository:

```bash
curl -fsSL https://deb.nodesource.com/setup_lts.x | sudo -E bash -
sudo apt-get install -y nodejs
```

Verify the installation:

```bash
node --version
npm --version
```

## Step 2: Set up Firebase

1. Go to the [Firebase Console](https://console.firebase.google.com/)
2. Click "Add project" and follow the prompts to create a new project
3. Once your project is created, click on "Hosting" in the left sidebar

## Step 3: Install Firebase CLI

Open your terminal and run:

```bash
npm install -g firebase-tools
```

## Step 4: Initialize the project

1. Navigate to your project directory in the terminal
2. Log in to Firebase:

   ```bash
   firebase login
   ```

3. Initialize your project:

   ```bash
   firebase init
   ```

4. Select "Hosting" when prompted for features
5. Choose your Firebase project
6. Set your public directory, 404 page, ect

## Step 5: Deploy a website

1. Download the template from github or create your own website
2. Make sure that your `index.html` is in your `public` folder
3. Deploy your site:

   ```bash
   firebase deploy
   ```

## Step 6: Access your website and apply finishing touches

1. After deployment, Firebase will provide you with a hosting URL. You can also set up a custom domain in the Firebase Console
2. If you want the contact form to work, go to  [Formspark](https://dashboard.formspark.io/sign-in) and create an account
3. Crate a new form then follow the "How-To" instructions
