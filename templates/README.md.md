step 1: install shopify CLI
  npm install -g @shopify/cli@latest

step 2: install theme access: https://apps.shopify.com/theme-access

step 3: get password by theme access

step 4: in visual code - create file shopify.theme.toml
  [environments.env1]
  theme = "141541998741"
  store = "6ac8b9-9e.myshopify.com"
  password  = "shptka_32cb9998bc8bbe9ecbe10c28e854ad2d"
  ignore = "sections/header.liquid"

  environments.env2]
  theme = "theme_id"
  store = "store_url"
  password  = "theme-access-password"
  ignore = "any file path"

Step 5: run shopify theme pull

push code run: 
  shopify theme dev --environment env1
  note: env1 define in shopify.theme.toml