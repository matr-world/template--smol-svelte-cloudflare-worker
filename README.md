# Smol Svelte + Cloudflare Worker

A super small Svelte app with a companion Cloudflare worker as a backend when you need it. It's kinda like Sveltekit, but more modular and less guided.

## 📱 Apps

#### 📂 `./api`

The API is a Cloudflare worker. This app contains all backend logic.

#### 📂 `./ui`

The UI is a Svelte app that interacts with the API.

## 🛠️ Develop

#### ⚙️ Setup UI `.env`

Create a `.env` file in `./ui` with the following.

```bash
VITE_API_URL="http://127.0.0.1:9000"
```

#### 🏃🏽‍♂️💨 Quickstart

-   `npm i`
-   `npm run dev`

#### Commands

There are a few top level commands to make development easier. Run the following commands from the root of this repo. You can run only the UI or only the API but in most cases you'll probably want to run both at once.

| Name                   | Description              | Command                |
| ---------------------- | ------------------------ | ---------------------- |
| **Install Everything** | Install config + UI app. | `npm i`                |
| **Install UI Only**    | Install UI Only.         | `npm i --prefix ./ui`  |
| **Dev Everything**     | Run UI and API at once.  | `npm run dev`          |
| **Dev API Only**       | Run UI and API at once.  | `npx wrangler dev`     |
| **Dev UI Only**        | Run UI and API at once.  | `npm run dev --prefix` |
