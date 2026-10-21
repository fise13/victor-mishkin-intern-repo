# Data Privacy Reflection

## Research & Learn

**Key takeaways from the [Focus Bear privacy policy](https://www.focusbear.io/privacy-policy)**
- **Data collected:** email and optional phone number, habits users create, optional survey answers (including occupation and whether they have ADHD), device type and OS, anonymized crash logs, subscription history (card details are handled by Stripe), and anonymous website analytics.
- **Sensitive data:** habits can reveal health or religious information, so even a simple habit name can be sensitive.
- **How it's used:** running accounts and support, personalizing the app, marketing emails (opt-out), daily motivational messages and website-blocking decisions using OpenAI, and a streak leaderboard under pseudonyms.
- **Sharing:** with service providers such as AWS, Stripe, Auth0, OpenAI and Brevo, and with legal authorities when required.
- **Security:** habit data is double-encrypted; survey data is anonymized or aggregated. Data may be handled outside the EU, including in Australia.
- **User rights:** access, correct, delete, export, object to processing, and withdraw consent. Requests go to privacy@focusbear.io and are answered within 30 days.
- **Age:** the service is for users aged 16 and over.

**What data is confidential at Focus Bear?**
User data (email, phone, habits, survey answers, health-related hints, purchase history), plus internal company information: access keys and credentials, internal documents, and anything not public.

**Best practices for handling confidential data**
- Collect and look at only what the task needs.
- Don't put real user data into test files, screenshots, chats or AI tools.
- Keep secrets (API keys, tokens) out of code and the repository; use environment variables.
- Share data only with people who need it, through approved channels.
- Delete data when it's no longer needed.

**What to do after a suspected breach or accidental disclosure**
Stop and don't try to hide or quietly fix it. Tell the team right away (supervisor or the team channel), say what happened, what data was involved and when, and follow their instructions. Change affected passwords or keys immediately. Reporting quickly matters more than the mistake itself.

## Reflection

**Steps I can take to handle data securely in daily tasks**
I rotate my API keys every 6 months. In daily work I'll also keep keys in environment variables and never commit them, and use fake data when testing.

**How should I store, share and dispose of sensitive information?**
- **Store:** in a password manager or environment files that are not in git.
- **Share:** only once and only to the person who needs it, never in a public channel. If a secret has been shared by mistake, I treat it as exposed and replace it.
- **Dispose:** delete files and old keys when they're no longer needed, and revoke keys that are no longer in use.

**Common mistakes that lead to privacy issues, and how to avoid them**
- Committing a key or `.env` file to GitHub: add it to `.gitignore` and check before every commit.
- Pasting real user data into an AI tool or a public chat: use fake or anonymized data.
- Sending sensitive info to the wrong person or channel: double-check the recipient first.
- Keeping old keys and files forever: rotate and delete regularly.

## Task

**A habit I will adopt at Focus Bear**
Before every commit I check what's in it (`git status` and `git diff`) to make sure there are no keys, passwords or real user data. If a key ever gets committed by mistake, I treat it as leaked: I replace it immediately and tell the team.

**Key learning**
Even a habit name in Focus Bear can be sensitive data (health, religion), so user data needs more care than just emails and passwords.
