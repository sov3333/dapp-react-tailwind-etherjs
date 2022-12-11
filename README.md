# dApp Tutorial

[Build and Deploy a Modern Web 3.0 Blockchain App | Solidity, Smart Contracts, Crypto](https://youtu.be/Wn_Kb3MR_cU)

## Technologies

Requirements: `node.js`

Frameworks & Libraries:
- ViteJS: https://vitejs.dev/
- TailwindCSS with PostCSS: https://tailwindcss.com/

## Installation

### Installing Vite

Documentation: `https://vitejs.dev/guide/`

1. Install Vite in `client` folder
```
npm create vite@latest

```
- Project name: `./`
- Select a framework: `React`
- Select a variant: `JavaScript`

2. Install dependencies
```
npm install
```

3. Run server
```
npm run dev
```
Open localhost server.

### Installing TailwindCSS using PostCSS

Documentation: https://tailwindcss.com/docs/installation/using-postcss

1. Install `tailwindcss` via npm
```
npm install -D tailwindcss postcss autoprefixer
```

2. Create `tailwind.config.cjs` and `postcss.config.cjs`
```
npx tailwindcss init -p
```

3. Copy then configure template paths into `tailwind.config.cjs`
```
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{js,jsx,ts,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

4. Add Tailwind directives to `index.css`
```
@tailwind base;
@tailwind components;
@tailwind utilities;
```

5. Add `h1` to `App.jsx`
```
  <h1 class="text-3xl font-bold underline">
    Hello world!
  </h1>
```

6. `npm run dev` - if text is bold and underlined, it worked!

### Setting up other dependencies

Install both `react-icons` and `ethers`
```
npm install react-icons ethers
```

### Gradients

e.g. for `.eth-card`:
- csshero.org/mesher

### Install tailwindcss forms
```
npm install -D @tailwindcss/forms
```

### Setup Hardhat

1. Install hardhat and dependencies
```
npm install --save-dev hardhat
```

2. Init basic sample project
```
npx hardhat
```

3. Test contract
```
npx hardhat test
```