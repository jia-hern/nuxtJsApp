# nuxt-app

> Simple Nuxt.js app

## Basic functionalities of this app:

```bash
1.Blog page which shows all posts

2. About page that shows some generic information

3.Admin page for logging in or signing up.
After authentication:
users can create a new post,
creat a new post,
and logout.

```

## Create firebase project and replace variables (to run this locally)

```bash
# Create a firebase account, then:
1.Enable realtime database.
the url link of this realtime database would be used for
basefbUrl in the next step.

2.In realtime database tab, click on rules.
replace the default rules with:
{
  "rules": {
    ".read": "true",
    ".write": "auth !=null",
  }
}

3.Enable authentication and choose email/password. Click on the project settings icon.
Copy the Web API Key. This value would be used for basefbKey in the next step.

# Go to nuxt.config.js and replace the values for:
basefbUrl
basefbKey

```

## Build Setup

```bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn run dev

# build for production and launch server
$ yarn run build
$ yarn start

# generate static project
$ yarn run generate
```

For detailed explanation on how things work, checkout [Nuxt.js docs](https://nuxtjs.org).
