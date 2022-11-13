---
slug: deploy-a-runtime-instance
id: wjmbyvkzxwtw
type: challenge
title: Deploy a Runtime Instance
teaser: Learn how to deploy a runtime instance (proxy) to a Linux VM
notes:
- type: text
  contents: This challenge walks you through deploying a runtime instance to a Linux
    VMs
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
🚀 Let's continue
==============

## Step 01
Using the Konnect Cloud browser, navigate to Runtime Manager > default > Runtime Instances.

## Step 02
Click the **Create runtime instance** button.

## Step 03
On the **Create a new runtime instance** page, click **Linux**.

## Step 04
Copy and paste the Cluster Certificate, Cluster Key and Configuration Parameters to the corresponding files (cluster.crt, cluster.key and kong.conf).  You can find these files in the Text Editor tab.

## Step 05
Update the contents of the `kong.conf` file to include the correct path to your `cluster_cert` and `cluster_key`.

## Step 06
**Save** all files.

🏁 Finish
=========

## Step 07
Press **Check** to continue to the next challenge.
