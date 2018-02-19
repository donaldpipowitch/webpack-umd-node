Just a small test case, because it looks like I cannot create an UMD build with webpack, which can be required by Node.

Just run `yarn && yarn build && yarn test`.

I get this error:

```
ReferenceError: window is not defined
    at Object.<anonymous> (/mnt/c/Users/foo/webpack-umd-node/dist/main.js:1:272)
```

It looks like the UMD build expects `window` to be defined. AFAIK this shouldn't be the case. 