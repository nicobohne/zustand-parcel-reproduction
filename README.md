# Zustand Parcel Issue Reproduction Repo

This repo is a minimal reproduction of an issue with Zustand and Parcel.

## Steps to reproduce

1. Clone this repo
2. Run `pnpm install`
3. Run `pnpm build`
4. Open `dist/index.html` in a browser (via Live Server or similar)

Note that the page will not load, and the console will show the following error:

```
app.js:3 Uncaught TypeError: (0 , i.create) is not a function
    at app.js:3:22
```

(This issue only happens in production mode. If you run `pnpm dev` and open the page in a browser, it will work fine.)