# One page accessibility analysis with Fruggr A11y scanner

## Use-case

This sample illustrates the basic usage of the Fruggr A11y scanner to perform an accessibility analysis on a single page.

## Requirements

Read the [main requirements](../#requirements).

## How to use?

- [Go on Fruggr SaaS](https://www.fruggr.io/app)
- Configure the accessibility analysis for your digital service (page URL, etc.)
- Note the `FRUGGR_A11Y_PAGE_ID` from the accessibility settings
- Copy the file [`.env.sample`](.env.sample) and name it `.env`
- Configure the `FRUGGR_API_KEY` and `FRUGGR_A11Y_PAGE_ID` in the `.env` file
- Run `docker compose up` in your command line
- At the end of the analysis, [go on Fruggr SaaS](https://www.fruggr.io/app) and check the accessibility report!

## Troubleshooting / FAQ

See ["Troubleshooting / FAQ"](../#troubleshooting--faq) section.

## Getting help

See ["Getting Help"](../#getting-help) section.
