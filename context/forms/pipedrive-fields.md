# Pipedrive Form Integration

## Required Forms

- Partner form
- Investor form
- Press / media form
- Support form
- General contact form
- Demo / sales form

## Integration Rule

All public forms must submit through one central form handler. Do not create separate Pipedrive API logic for each form.

## Recommended Fields

| Field | Required | Notes |
| --- | --- | --- |
| name | Yes | Full name of the contact. |
| email | Yes | Primary email address. |
| company | No | Company or organization. |
| role | No | Job title or function. |
| country | No | Country for regional context. |
| interest_type | Yes | One of `demo`, `sales`, `partner`, `investor`, `press`, `support`, `general`. |
| message | No | Free-text message. |
| preferred_language | Yes | `en` or `es`. |
| source_page | Yes | Full route where the form was submitted. |
| utm_source | No | Campaign tracking. |
| utm_medium | No | Campaign tracking. |
| utm_campaign | No | Campaign tracking. |

## Suggested Pipedrive Mapping

Create or update a person record using `name` and `email`.

Create an organization when `company` is provided.

Create a lead or deal with:

- Title: `[interest_type] - [company or name]`
- Source page: `source_page`
- Preferred language: `preferred_language`
- Message: `message`
- UTM fields when present

## Form Behavior

- Validate required fields before submission.
- Include the current route as `source_page`.
- Preserve UTM parameters from the visitor session.
- Show a localized success message.
- Show a localized error message if submission fails.
- Avoid exposing Pipedrive API keys in browser code.
