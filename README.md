# The 76 Devs

## 📱 Apps

#### 📂 `./api`

The API is a Cloudflare worker. This app contains all backend logic.

#### 📂 `./ui`

The UI is a Svelte app that interacts with the API.

## 🛠️ Develop

There are a few top level commands to make development easier. Run the following commands from the root of this repo. You can run just the UI or just the API but in most cases you'll probably want to run both at once.

#### 🏃🏽‍♂️💨 Quickstart

-   `npm i`
-   `npm run dev`

#### Setup UI `.env`

Create a `.env` file in `./ui` with the following.

```
VITE_API_URL="http://127.0.0.1:9000"
```

#### Commands

| Name                   | Description              | Command                |
| ---------------------- | ------------------------ | ---------------------- |
| **Install Everything** | Install config + UI app. | `npm i`                |
| **Install UI Only**    | Install UI Only.         | `npm i --prefix ./ui`  |
| **Dev API + UI**       | Run UI and API at once.  | `npm run dev`          |
| **Dev API Only**       | Run UI and API at once.  | `npx wrangler dev`     |
| **Dev UI Only**        | Run UI and API at once.  | `npm run dev --prefix` |
