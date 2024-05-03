first we run npx-create-next-app@13.4.9 or @latest

then we install npm i eslint-config-standard  this will install stadard ESLint configurration in your project
then add it to your .eslintrc.json 
which is this 
{
  "extends": "next/core-web-vitals"
}

we modify it to this
{
  "extends": ["next/core-web-vitals","standard"]
}


now  since we are using tailwind css we add classes and all the classes we add randomly so to properly structure the classes one after the othr logically such as {"flex flex-col justify-between m-1 p-1 "} we make use of another speacial plugin which is "eslint-plugin-tailwindcss " this will arrange the classes logically 

to do this we do npm i  eslint-plugin-tailwindcss and addd that in the eslintrc.json


{
  "extends": ["next/core-web-vitals","standard","plugin:tailwindcss/recommended"]
}

we also install eslint-config-prettier to avoid conflicts between prettier and ESLint 

npm i eslint-config-prettier

now we also add "prettier" in the config file 

{
  "extends": ["next/core-web-vitals","standard","plugin:tailwindcss/recommended","prettier"]
}
