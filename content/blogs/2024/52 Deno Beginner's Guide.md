---
title: "Deno Made Easy: A Beginner's Guide to Web Development"
author: "Maheen Waris"
url: "/blogs/deno-beginners-guide/"
date: "2024-10-12"
tags: ["Programming", "Deno Land"]
draft: "false"
toc: "true"
---

Deno is a modern runtime for JavaScript and TypeScript that makes web development easier and more secure. If you’re new to Deno, this guide will walk you through the basics step by step.

## 1. Installing Deno
Before you can start using Deno, you need to install it. Here’s how:
- **For macOS**:
  Open your terminal and run:
  ```bash
  brew install deno
  ```
- **For Windows**:
  Open PowerShell and run:
  ```bash
  iwr https://deno.land/x/install/install.ps1 -useb | iex
  ```
- **For Linux**:
  In your terminal, type:
  ```bash
  curl -fsSL https://deno.land/x/install/install.sh | sh
  ```

## 2. Verify Installation
Once installed, make sure it’s working by typing:
```bash
deno --version
```
You should see the version number of Deno displayed.

## 3. Running Your First Script
Let’s create a simple script. Open your favorite text editor and make a file called `hello.ts` with the following code:
```typescript
console.log("Hello, Deno!");
```
Now, run the script in your terminal with:
```bash
deno run hello.ts
```
You should see “Hello, Deno!” printed in your terminal!

## 4. Importing Modules

Deno makes it easy to use third-party libraries. You can import them directly from URLs. For example, let’s create a simple server:

```typescript
import { serve } from "https://deno.land/std/http/server.ts";

const server = serve({ port: 8000 });
console.log("Server running on http://localhost:8000");

for await (const request of server) {
  request.respond({ body: "Hello from Deno!\n" });
}
```

Run it with:
```bash
deno run --allow-net server.ts
```

The `--allow-net` flag gives your script permission to use the network.

## 5. Understanding Permissions

Deno is designed with security in mind. By default, your scripts don’t have access to files, the network, or the environment. You must give explicit permissions using flags like `--allow-read`, `--allow-write`, or `--allow-net` when running your scripts.

## 6. Built-in Tools

Deno comes with useful tools to help you write better code:

- **Formatting**: To format your code neatly, run:
  ```bash
  deno fmt
  ```
- **Linting**: To check your code for common errors, use:
  ```bash
  deno lint
  ```
- **Testing**: If you want to run tests, just type:
  ```bash
  deno test
  ```

## 7. Deploying with Deno Deploy
If you want to deploy your Deno application, check out **Deno Deploy**. It’s a serverless platform that lets you run your Deno code in the cloud. Sign up for an account on the [Deno Deploy website](https://deno.com/deploy), and follow the instructions to get started.

## Conclusion
Deno is a powerful tool that makes developing applications simpler and safer. With its straightforward installation, easy module importing, and built-in tools, it’s a great choice for both beginners and experienced developers. Explore more about Deno in the [official documentation](https://deno.land/manual) as you continue your journey!
That's it <3



<script src="https://utteranc.es/client.js"
        repo="maheenwaris/Website"
        issue-term="pathname"
        theme="github-dark"
        crossorigin="anonymous"
        async>
</script>
---