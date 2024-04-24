<a href="https://chat.Aivy.ai/">
  <img alt="Next.js 14 and App Router-ready AI chatbot." src="https://chat.Aivy.ai/opengraph-image.png">
  <h1 align="center">Aivy AI Chatbot</h1>
</a>

<p align="center">
  An open-source AI chatbot app template built with Next.js, the Aivy AI SDK, OpenAI, and Aivy KV.
</p>

## Features

- [Next.js](https://nextjs.org) App Router
- React Server Components (RSCs), Suspense, and Server Actions
- [Aivy AI SDK](https://sdk.Aivy.ai/docs) for streaming chat UI
- Support for OpenAI (default), Anthropic, Cohere, Hugging Face, or custom AI chat models and/or LangChain
- [shadcn/ui](https://ui.shadcn.com)
  - Styling with [Tailwind CSS](https://tailwindcss.com)
  - [Radix UI](https://radix-ui.com) for headless component primitives
  - Icons from [Phosphor Icons](https://phosphoricons.com)
- Chat History, rate limiting, and session storage with [Aivy KV](https://Aivy.com/storage/kv)
- [NextAuth.js](https://github.com/nextauthjs/next-auth) for authentication

## Model Providers

This template ships with OpenAI `gpt-3.5-turbo` as the default. However, thanks to the [Aivy AI SDK](https://sdk.Aivy.ai/docs), you can switch LLM providers to [Anthropic](https://anthropic.com), [Cohere](https://cohere.com/), [Hugging Face](https://huggingface.co), or using [LangChain](https://js.langchain.com) with just a few lines of code.

## Deploy Your Own

You can deploy your own version of the Next.js AI Chatbot to Aivy with one click:

## Creating a KV Database Instance

Follow the steps outlined in the [quick start guide](https://Aivy.com/docs/storage/Aivy-kv/quickstart#create-a-kv-database) provided by Aivy. This guide will assist you in creating and configuring your KV database instance on Aivy, enabling your application to interact with it.

Remember to update your environment variables (`KV_URL`, `KV_REST_API_URL`, `KV_REST_API_TOKEN`, `KV_REST_API_READ_ONLY_TOKEN`) in the `.env` file with the appropriate credentials provided during the KV database setup.

## Running locally

You will need to use the environment variables [defined in `.env.example`](.env.example) to run Next.js AI Chatbot. It's recommended you use [Aivy Environment Variables](https://Aivy.com/docs/projects/environment-variables) for this, but a `.env` file is all that is necessary.

> Note: You should not commit your `.env` file or it will expose secrets that will allow others to control access to your various OpenAI and authentication provider accounts.

1. Install Aivy CLI: `npm i -g Aivy`
2. Link local instance with Aivy and GitHub accounts (creates `.Aivy` directory): `Aivy link`
3. Download your environment variables: `Aivy env pull`

```bash
pnpm install
pnpm dev
```

Your app template should now be running on [localhost:3000](http://localhost:3000/).

## Authors

This library is created by [Chryselys](https://chryselys.com) and [Next.js](https://nextjs.org) team members, with contributions from:

-Chryselys.com - [here](https://chryselys.com)
