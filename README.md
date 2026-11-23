# Independent Clinical AI Content Review

Independent educational reviews of AI-generated medical content, focusing on clinical accuracy, scientific evidence, completeness, patient safety, communication quality, and opportunities for improvement.

> **Status:** Early-stage informational website. No clinical case submission, client onboarding, clinician verification, formal certification, or patient data handling is implemented.

## Preview and GitHub Pages deployment

The site is dependency-free, using `index.html`, `assets/styles.css`, `assets/site.js`, and `assets/favicon.svg`.

To test locally: `python -m http.server 8000` and open `http://localhost:8000`.

After approving and merging the website pull request:
1. Navigate to **Settings → Pages** in this repository.
2. Select **Deploy from a branch**, then **main** and **/(root)**.
3. Save. After deployment, the expected site URL is `https://jeevantjr.github.io/clinical-ai-review/`.

Relative file links support GitHub Pages project-site hosting.

## Authentication architecture

```text
Visitor browser -- HTTPS GET --> GitHub Pages
                                     |-- index.html
                                     |-- assets/styles.css
                                     |-- assets/site.js
                                     `-- assets/favicon.svg
```

**No visitor authentication is implemented.** There are no passwords, logins, sessions, OAuth flows, authentication cookies, bearer tokens, token refresh operations, backends, or databases. The only JavaScript interaction controls the mobile navigation menu. No external scripts or analytics are included.

GitHub account login, repository authorization, and GitHub App or API credential handling occur at GitHub's platform level, not inside this website. Repository writes require appropriate GitHub permissions. **Do not commit passwords, access tokens, API keys, or private data** to this public repository or embed them in client-side HTML or JavaScript.

GitHub Pages is public static hosting and cannot securely process private medical review submissions on its own. A separate access-controlled server-side application would be needed if secure submissions become necessary.

## Editorial and privacy safeguards

- Use fictional or appropriately de-identified examples. Never submit identifiable clinical records in public GitHub discussions.
- Medical content evaluation is contextual, educational, and not a substitute for individual medical advice, clinical validation, or regulatory assessment.
- Verify citations, clinical context, evidence date, and jurisdiction before publishing substantive reviews.
- Distinguish potentially safety-critical findings from substantive factual and editorial corrections.
- Disclose relevant conflicts of interest and do not imply certifications or institutional endorsements without evidence.
- Do not accept review assignments until suitable professional contact and data-handling arrangements exist.

## Development roadmap

1. Confirm wording, scope, and professional identity disclosures.
2. Merge approved site files and enable GitHub Pages.
3. Add editorial review methodology, evidence citation rules, and transparent review examples.
4. Establish an appropriate professional contact channel and privacy notice.
5. Consider a separate authenticated backend only when real client workflows warrant it.

## License

No open-source license is granted at this stage.
