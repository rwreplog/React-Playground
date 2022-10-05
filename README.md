# React-Playground

Playground for learning React/Native

## How to Run

---

Install all of the packages by running `npm install`

Start the application by running `expo start --tunnel`

## Setting up Linting

---

Install eslint `npm install eslint --save-dev`

Then create your .eslintrc.json by running `npx eslint --init`

You will then be prompted with the following questions:

- How would you like to use ESLint? `To check syntax and find problems`

- What type of modules does your project use? `JavaScript modules (import/export)`

- Which framework does your project use? `React`

- Does your project use TypeScript `No`

- Where does your code run? `Press A to select both browser and node`

- What format do you want your config to be in? `JSON`

- Would you like ot install them now with npm? `No`

In your .eslintrc file add the following line to "rules":

<code>"react/react-in-jsx-scope": "off"</code>

Next, install eslint prettier plugin:

<code>npm install eslint-config-prettier eslint-plugin-prettier prettier --save-dev</code>

After installing, make the following changes to `.eslintrc`

<code>
"extends": [
        "eslint:recommended",
        "plugin:react/recommended"
    ],
</code>

Create a `.prettierrc` file in the root directory and add the following code:

<code>
{
  "semi": true,
  "tabWidth": 2,
  "printWidth": 100,
  "singleQuote": true,
  "trailingComma": "none",
  "jsxBracketSameLine": true
}
</code>
