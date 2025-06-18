
# fenrir-security
# fenrir-security
# vscode-app
# fenrir-security
# Customized VS Code with Built-In Wingman AI

This repository includes a customized build of Visual Studio Code with Wingman AI integrated directly as a native component. It launches automatically on first run, is not listed among user-installable extensions, and cannot be removed via the standard Extensions panel.

---



 Wingman AI is embedded within the application and starts without user intervention.
 It is hidden from the Marketplace and the Extensions sidebar.
Full VS Code functionality remains unaffected.
Upgrade process is documented for future maintenance.
 A demo recording highlights the build behavior and integration.

---

# How to Build (macOS ARM64)

### Step 1: Set Up Environment

Ensure the following tools are installed:

- Node.js v16
- Yarn (`npm install -g yarn`)
- Gulp CLI (`npm install -g gulp`)
- Python 3
- Git, CMake, and Ninja (via Homebrew)

### Step 2: Clone the VS Code Source

--in terminal how i made it 
git clone https://github.com/microsoft/vscode.git
cd vscode
yarn install or else npm install

cd extensions
git clone https://github.com/RussellCanfield/wingman-ai
cd wingman-ai
yarn install


made file in -build->builtinExtensions.json
Hide the Extension from the UI  -> src/vs/workbench/contrib/extensions/browser/extensionsViewlet.ts 


for building the app in mac use the command 
NODE_OPTIONS="--max-old-space-size=8192" npx gulp vscode-darwin-arm64  (if u have 8gb ram laptop) if 16gb then use "npx gulp vscode-darwin-arm64"


```
Developed by: Rajesh Chauhan
GitHub: rajeshchauhan1426
Submission for: Fenrir Security – Technical Assessment

yaml
Copy
Edit

```
ASK FOR PERMISSION FOR THE USE OF THE SOURCE CODE # fenrir-security
# vscode-app
