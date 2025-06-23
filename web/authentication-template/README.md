# Authentication Script Template

## Use-case

This sample provides a template for creating external authentication scripts with Fruggr scanner. The template includes common authentication patterns like:

- Navigating to a login page
- Filling in credentials
- Submitting the form
- Waiting for authentication to complete
- Verifying successful login

## Requirements

Read the [main requirements](../fruggr-scanner/#requirements).

## How to use?

1. [Go on Fruggr SaaS](https://www.fruggr.io/app)
2. Create a new Fruggr digital service of type "web"
3. Copy the file [`.env.sample`](.env.sample) and name it `.env`
4. Configure the `FRUGGR_API_KEY` in the `.env` file
5. Modify the [`script.json`](work/script.json) template with your authentication details:
   - Update the login URL
   - Set the username/email selector
   - Set the password selector
   - Update the submit button selector
   - Configure success verification
6. Run `docker compose up` to test your script

## Script Template Structure

The template provides a basic navigation flow with cookie handling:

1. Navigate to Fruggr homepage
2. Handle language selector interaction
3. Accept cookies by clicking the accept button

Customize the selectors and steps according to your application's needs. The current script shows how to:

- Navigate to a specific URL (optional if the login page is the same as the project origin URL)
- Interact with page elements using selectors
- Handle common website requirements like cookie acceptance

To add authentication:

- Add steps for login form interaction
- Configure username/password fields
- Set up success verification

## Testing Tips

- Start with the debug screenshots mode to verify each step
- Use browser developer tools to identify correct selectors
- Add appropriate waits between actions if needed
- Verify success conditions carefully

## Troubleshooting / FAQ

See ["Troubleshooting / FAQ"](../fruggr-scanner/#troubleshooting--faq) section.

## Getting help

See ["Getting Help"](../fruggr-scanner/#getting-help) section.
