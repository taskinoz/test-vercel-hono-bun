# Test Vercel Hono Bun
Deploy a test hono server on vercel


## Setup
```
bun i
bun run start
```

## Notes
- `vercel.json` is the configuration file for vercel
    - `rewrites` is used to rewrite the url to the serverless function
        - `source` is the request path
        - `destination` is the serverless function (setting it to `src` will download the serverless function from the `src` directory)
- `api/index.js` is the serverless function
- `package.json` has the vercel dev dependency and the start script