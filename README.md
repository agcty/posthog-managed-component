# PostHog Managed Component

> A managed component for Postman analytics

Common use is currently for [Cloudflare Zaraz](https://www.cloudflare.com/application-services/products/zaraz/) (it's OSS so hopefully more use cases will come).

## TODO:

- [ ] pull users PotsHog API key from environment
- [ ] send page views to PostHog
- [ ] send events to PostHog
- [ ] send user data to PostHog
- [ ] send custom data to PostHog
- [ ] add MC to <https://managedcomponents.dev/components/>
- [ ] add MC to <https://github.com/PostHog/integrations-repository/blob/main/integrations.json>
- [ ] mention MC on [PostHog Docs](https://posthog.com/docs/advanced/proxy/cloudflare)
- [ ] mention MC on [Discord](https://discord.com/channels/595317990191398933/917505178016579605/1225745641351675925)

## Documentation

[Managed Components docs](https://managedcomponents.dev/)

Find out more about Managed Components [here](https://blog.cloudflare.com/zaraz-open-source-managed-components-and-webcm/) for inspiration and motivation details.

[![Released under the Apache license.](https://img.shields.io/badge/license-apache-blue.svg)](./LICENSE)
[![PRs welcome!](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](./CONTRIBUTING.md)
[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)

## 🚀 Quickstart local dev environment

1. Make sure you're running bun (any version) or NodeJS version >=18.
2. Install dependencies with `bun i` or `npm i`
3. Run unit test watcher with `bun run test:dev` or `npm run test:dev`

## ⚙️ Tool Settings

> Settings are used to configure the tool in a Component Manager config file

### Example Setting `boolean`

`exampleSetting` can be the pixelID or any other essential/optional setting like the option to anonymize IPs, send ecommerce events etc.

## 🧱 Fields Description

> Fields are properties that can/must be sent with certain events

### Human Readable Field Name `type` _required_

`field_id` give it a short description and send to a more detailed reference [Find more about how to create your own Managed Component](https://managedcomponents.dev/).

## Deployment

```bash
npx managed-component-to-cloudflare-worker ./index.js my-new-counter-mc
```

## 📝 License

Licensed under the [Apache License](./LICENSE).
