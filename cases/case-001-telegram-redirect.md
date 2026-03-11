# Case 001 — Telegram Redirect Funnel Observation

## Context
While participating in a public Telegram мараthon channel, I noticed that most external links were distributed through shortened redirect services.
Instead of linking directly to platforms such as YouTube or Instagram, the channel used intermediate redirect URLs.

## Observation

Several elements raised suspicion:

- links were distributed via redirect shorteners
- the final destination changed dynamically
- a login page resembling Instagram appeared during one of the redirects
- the overall structure resembled a marketing funnel designed to capture user interaction

## Potential Risk

Such redirect chains can potentially be used for:

- phishing login pages
- user tracking and profiling
- collection of personal data
- credential harvesting

Even when the initial content appears legitimate, redirect chains make it difficult to verify the true destination.

## Response

The interaction with the funnel was stopped before entering any credentials or personal information.

No authentication data or financial information was provided.

## Security Insight

Redirect chains are a common technique used in both marketing funnels and phishing campaigns.

Users should always verify the final domain before entering credentials, especially when links originate from social media or messaging platforms.
