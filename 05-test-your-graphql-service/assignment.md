---
slug: test-your-graphql-service
id: 8otvx1ytuygh
type: challenge
title: Test your GraphQL Service
teaser: A short description of the challenge.
notes:
- type: text
  contents: Next up, we'll start-up the Konnect runtime instance and test your GraphQL
    service
tabs:
- title: Shell
  type: terminal
  hostname: container
- title: File Editor
  type: code
  hostname: container
  path: /root
- title: Konnect Cloud
  type: external
  url: https://cloud.konghq.com/login
difficulty: basic
timelimit: 600
---
🚀 Let's finish up
==============

Now that you have all the configuration files copied and configured, let's go ahead and test your graphQL service.
We recommend you use an external API design tool for testing, like Insomnia.

## Step 01
First off, let's start-up the Kong runtime instance (dataplane):

```bash
kong start -c kong.conf
```

## Step 02
You can find your hostname by running the following command:

```bash
echo $HOSTNAME.$_SANDBOX_ID.instruqt.io
```

Alternatively, you can test the service by running the following curl command:

```bash
curl --request POST \
  --url http://localhost:8000/query \
  --header 'Content-Type: application/json' \
  --header 'kong-debug: true' \
  --data '{"query":"{\n  country(code: \"AU\") {\n    name\n    native\n    capital\n    emoji\n    currency\n    languages {\n      code\n      name\n    }\n  }\n}"}'|jq
  ```

  🏁 Finish
=========

## Step 03
Press **Check** to continue to the last challenge.  Quiz Time!!