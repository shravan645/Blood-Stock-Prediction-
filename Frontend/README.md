# Blood Stock Prediction Dashboard

## Run locally

```sh
npm install
```

Copy `.env.example` to `.env` if the API is not running at `http://localhost:8000`, then start the development server:

```sh
npm run dev
```

`VITE_API_BASE_URL` must be the backend origin only. The API paths already start with `/api`.

## Deploy to Vercel

Import the GitHub repository `shravan645/Blood-Stock-Prediction-` into Vercel and set **Frontend** as the Root Directory. Vercel detects Vite automatically; use `npm run build` as the build command and `dist` as the output directory.

The included `vercel.json` proxies `/api/*` requests to the deployed Render backend. No frontend environment variable is required for the production deployment. Local development continues to use `http://localhost:8000` by default.
