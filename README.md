# nextjs-preactjs-boilerplate
NextJS, PreactJS and TailwindCSS boilerplate

## Techonologies
### NextJS

### PreactJS
[Differences to react](https://preactjs.com/guide/v10/differences-to-react)

#### Bundle size
There is a huge difference between ReactJS and Preact bundle size. ReactJS is about 38,5kB GZIP and PreactJS is only 8,9kB GZIP.

- [react](https://bundlephobia.com/result?p=react@16.13.1): 2.6kB
- [react-dom](https://bundlephobia.com/result?p=react-dom@16.13.1): 35.9kB
- [preact](https://bundlephobia.com/result?p=preact@10.4.4): 3.9kB
- [preact/compat](https://bundlephobia.com/result?p=preact-compat@3.19.0): 5kB

## TailwindCSS
[Utility first](https://tailwindcss.com/docs/utility-first/)
                                   
# How to build 
Clone the example repo from [developit](https://github.com/developit/nextjs-preact-demo)

```shell script
git clone https://github.com/developit/nextjs-preact-demo.git
cd nextjs-preact-demo
npm install
```

The example takes advantage of npm/yarn aliases, which essentially allow installing preact/compat at node_modules/react.

Here's how this example repo was set up:

Set up a basic Next.js app using create-next-app
Install preact, uninstall react and react-dom.
Install preact-compat/react and preact-compat/react-dom for aliasing.
Use an npm alias to replace react-ssr-prepass with preact-ssr-prepass (also works with Yarn).

## TypeScript
https://nextjs.org/docs/basic-features/typescript

Create an empty tsconfig.json file in the root of your project:
```shell script
touch tsconfig.json
```

Then, install the required packages to finish the set up:
```shell script
npm install --save-dev typescript @types/react @types/node
```

Rename .js files to .tsx.

Run start the local server:
```shell script
npm run dev
```

It will automatically fill the tsconfig.json. Make sure you set strict to true.