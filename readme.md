# svelte withe environment variables

The sveltejs/template starter project doesn’t allow the use of environment variables out-of-the-box.

Env can be used by using this module with svelte.

<br/><br/>

## how to use

<br/>

### installation

```bash
npm install @goesvt/svelte-use-env
```

<br/>

### useage

Just following below code.

in `rollup.config.js` file

```jsx
...

import insertEnv from "@goesvt/svelte-use-env";

const production = !process.env.ROLLUP_WATCH;

...

export default {
    ...,
    plugins : [
        ...,
        insertEnv(),     // insert here !!
    ],
    ...
}
```
