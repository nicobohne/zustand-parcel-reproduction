# Zustand Parcel Issue Reproduction Repo

This repo is a minimal reproduction of an issue with Zustand and Parcel.

## Steps to reproduce

1. Clone this repo
2. Run `pnpm install`
3. Run `pnpm build`
4. Open `dist/index.html` in a browser (via Live Server or similar)

Note that the page will not load, and the console will show the following error:

```
index.js:41 Uncaught TypeError: Cannot convert undefined or null to object
    at Function.assign (<anonymous>)
    at index.js:41:42
```

(This issue only happens in production mode. If you run `pnpm dev` and open the page in a browser, it will work fine.)