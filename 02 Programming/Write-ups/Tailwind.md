Status: #Doing 
Tags: #css #Internet #webdesign
Links: [[Environment - Programming]] [[React]]
MOC: [[Programming MOC]]
___
# Writeup - Tailwind
Tailwind is a css framework that uses a class syntax that is very similar to pure css but it guides you into using good habits like `rem` for font size. This way you are almost forced into using best practices and it even automates tasks for you like minimizing your css.

Tailwind is **not** a css framework to fully give styling like a navbar, you will have to create that yourself, **however** it does provide a more usable and quickly customizable way of editing it.

## Tailwind installation in React app
```js
// Create the project
npx create-react-app my-project
cd my-project
// Install Tailwind CSS
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
//Configure template paths in tailwind.config.js
module.exports = {  content: [    "./src/**/*.{js,jsx,ts,tsx}",  ],  theme: {    extend: {},  },  plugins: [],}
//Add tailwind directives to your css 
@tailwind base;
@tailwind components;
@tailwind utilities;
//Start build
npm run start
//Start using tailwind in project
export default function App() {  return (    <h1 className="text-3xl font-bold underline">      Hello world!    </h1>  )}
```


___
1. [Tailwind documentation](https://tailwindcss.com/docs/guides/create-react-app)