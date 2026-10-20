## Lightweight Chrome extension for secure API token management. Centralizes token handling for developers.

## 🎥 Demo Video
Watch a quick demo.
🚀 Features
- Manage multiple roles 🧑‍💻 Create roles (e.g., admin, user). Stores unique credentials and last API response.
- Save credentials securely 🔒 Store username/password per role. Remembers them to avoid retyping.
- Receive tokens instantly ⚡ Send API request and retrieve token in one click.
- Copy tokens easily 📋 Copy last token via “Copy” button. Disabled if no valid token.
- View last API response 📄 Click “Last Response” to view previous response for selected role.
- Edit or delete roles ✏️❌ Modify credentials or delete roles with confirmation.
- Smart UI & UX 🎨
  - Responsive layout, neat design.
  - Colored messages: success ✅, errors ❌.
  - Context-aware button visibility.
  - Retains last token after closing popup.

## 🛠️ How It Works
1. Set API URL Click Change to edit. Press Apply to save.
2. Add Roles Click + to create new role.
3. Add Credentials Select role, click Edit Credentials, enter username/password, save.
4. Get Token Click Receive Token to query API.
  - On success, token is saved and displayed.
  - “Copy” button activates to copy access token.
5. View Last Response Click Last Response to see selected role’s last response.
6. Delete Role Select role, click Delete. Confirmation alert prevents accidental deletion.

## 💾 Storage
Uses Chrome local storage to save:
- API URL
- Roles list
- Credentials (username + password) per role
- Last access token per role
- Last API response per role
All data remains local. Nothing is sent elsewhere.

## 🎨 UI Details
- Messages:
  - ✅ Green = Success
  - ❌ Red = Error
  - ⚪ Gray = Info
- Buttons:
  - Copy token spans full width at bottom.
  - Action buttons (Receive Token, Last Response, Delete, Edit Credentials) appear only when a role is selected.
  - Disabled buttons turn gray.
- Selected roles are highlighted.

## 🔧 Installation
1. Open Chrome, go to chrome://extensions/
2. Enable Developer mode
3. Click Load unpacked, select TokenBox folder
4. Pin extension for quick access

## 🧑‍💻 Usage Tips
- Save credentials before requesting tokens.
- Use separate roles for dev, staging, prod.
- Use Last Response for debugging.

## 📌 Notes
- Only sends requests to configured API URL.
- Data stays on device, never shared.
- Works offline for viewing saved roles, responses, credentials.
