---
slug: create-a-service-and-route-using-deck
id: oqnfzr97cmvd
type: challenge
title: Create a Service & Route using decK
teaser: Now that we have credentials figured out, let's try exposing a Service & Route
  using Konnect Cloud
notes:
- type: text
  contents: Services and Routes are the core building blocks of Kong.  Let's see if
    we can figure out how to configure them using our declarive language of choice,
    decK!
tabs:
- title: Shell
  type: terminal
  hostname: container
- title: Konnect Cloud
  type: external
  url: https://cloud.konghq.com/login
difficulty: basic
timelimit: 600
---

🚀 Let's continue
==============

## Step 01
Use the terminal to add a Service and Route declaratively, using decK:

```
deck sync --konnect-runtime-group-name default --konnect-token-file pat --state kong-new.yaml
```

## Step 02
Via the Konnect Cloud browser, verify that both the Service and Route have been created successfully.

🏁 Finish
=========

## Step 03
Press **Check** to continue to the next challenge.