See [vite-plugin-ssr.com/vercel](https://vite-plugin-ssr.com/vercel).

How to deploy:
 1. Fork this repository.
 1. Log in to your [Vercel](https://vercel.com/) account (or create one).
 1. Add your fork on Vercel's dashbaord with following settings:
    - `FRAMEWORK PRESET` should be `Vite`. (Vercel should automatically detect Vite; just make sure it's already set.)
    - Modify `Build and Output Settings` > `OUTPUT DIRECTORY` from `dist` to `dist/client`.

That's it, your fork is now deployed on Vercel (it should look like [vite-plugin-ssr-demo.vercel.app](https://vite-plugin-ssr-demo.vercel.app)). It's continuously deployed: if you commit and push a change to your fork, then Vercel automatically re-deploys your app.

Integration points:
 - API Route: [api/ssr.js](api/ssr.js).
 - Routing URLs to our API Route: [vercel.json#rewrites](vercel.json).
 - Build: the [package.json](package.json)'s scripts `package.json#scripts['vercel-build']` and `package.json#scripts.build`.
 - Development: the [package.json](package.json)'s script `package.json#scripts.dev`; we use Vite's development server for improved DX.

``` 
/star-wars/2
```

"daisyui": "^2.6.0",

https://directus-serverless-vercel.vercel.app/proxy/v1/status
https://directus-serverless-vercel.vercel.app/proxy/sys/serverless/info