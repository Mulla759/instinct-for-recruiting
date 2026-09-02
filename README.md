# 🎯 Instinct for Recruiting

![Use cases](https://img.shields.io/badge/use%20cases-16-brightgreen) ![Status](https://img.shields.io/badge/status-field--tested-blue) ![Setup](https://img.shields.io/badge/setup-clone%20%26%20prompt-orange)

**One personal agent running the whole job hunt** - sourcing, applications, outreach, referrals, interviews, and the logistics around them. Everything in this repo is a use case that has actually run on a real search.

---

## 🧠 How it works

**Instinct** is a personal AI agent. You text it like a person; it works like a teammate who never sleeps. Two pieces make that possible:

- 🔌 **Connectors** link your accounts - Gmail, Calendar, Sheets, Docs, and more - with your permission. The agent reads what it needs and works where you already live: drafts in your Gmail, rows in your Sheets, events on your calendar.
- 🔐 **The vault** holds your credentials securely. When a site needs a login, the agent signs in for you without a password ever passing through a chat.

**The split:** the agent does the ninety percent - sourcing, research, form filling, drafting, tracking, follow-ups. You do the last two minutes where a portal walls automation (captchas, logins, no-AI rules) and the one tap where your name goes on a send.

---

## 🗂️ Use cases

### 🔍 Sourcing & watches

| # | Use case | What it does |
|---|----------|--------------|
| 1 | [Daily internship drop watch](use-cases/01-daily-internship-drop-watch.md) | Verified-open postings every day, kills included |
| 11 | [Standing company watches](use-cases/11-standing-company-watches.md) | A dedicated eye on target employers' career pages |
| 13 | [Role sweeps](use-cases/13-role-sweeps.md) | Wide passes for roles beyond what the tracker caught |

### 📊 Tracking & sheets

| # | Use case | What it does |
|---|----------|--------------|
| 2 | [Application pipeline tracker](use-cases/02-application-tracker.md) | One live sheet for every role, stage, and deadline |
| 16 | [Opportunity tracker sheet](use-cases/16-opportunity-tracker.md) | The intake queue: roles worth pursuing, ranked by fit and deadline |

### ✍️ Applications & resumes

| # | Use case | What it does |
|---|----------|--------------|
| 3 | [Application autofill](use-cases/03-application-autofill.md) | Portals filled with standing answers and the right resume |
| 6 | [Resume ops](use-cases/06-resume-ops.md) | JD-versus-resume fit scores and gap lists per role |
| 7 | [LinkedIn SEO/AEO audit](use-cases/07-linkedin-seo-aeo-audit.md) | Headline and profile benchmarked against profiles that rank |
| 14 | [Application answer drafting](use-cases/14-application-answer-drafting.md) | Portal essays and short answers written from real material |

### ✉️ Outreach & email

| # | Use case | What it does |
|---|----------|--------------|
| 4 | [Cold recruiter outreach](use-cases/04-cold-recruiter-outreach.md) | Drafts staged and ready, sent one at a time on approval |
| 5 | [Recruiter email discovery](use-cases/05-recruiter-email-discovery.md) | Addresses found and verified by a private email-enrichment pipeline - confirmed patterns only, never guessed |
| 12 | [InMail copy doc](use-cases/12-inmail-copy-doc.md) | Ranked, copy-paste-ready LinkedIn blocks |
| 15 | [Rejection recovery](use-cases/15-rejection-recovery.md) | Rejections logged and triaged, follow-ups drafted for the doors worth keeping open |

### 📅 Interviews & logistics

| # | Use case | What it does |
|---|----------|--------------|
| 8 | [Interview logistics](use-cases/08-interview-logistics.md) | Assessments, recorded interviews, and deadlines tracked |
| 9 | [Conference trip prep](use-cases/09-conference-trip-prep.md) | Flights priced and ranked, outreach prepped before wheels up |
| 10 | [Referral tracking](use-cases/10-referral-tracking.md) | Referrals verified as actually attached, not assumed |

---

## 🚀 Set this up for yourself

You don't need to rebuild anything from scratch. The use-case files are written as specs - the prompts, rules, and workflows for each one - so an AI coding tool can implement them against your own accounts.

1. **Clone the repo:**
   ```bash
   git clone https://github.com/Mulla759/instinct-for-recruiting.git
   ```
2. **Open the folder in your AI coding tool** - Claude Code, Cursor, or whatever you already use.
3. **Point it at a use case:** "Read `use-cases/01-daily-internship-drop-watch.md` and set this up for me."
4. **Bring your own accounts.** The workflows assume access to your email, calendar, and spreadsheets (directly or through an agent's connectors), plus your resume and a target company list.

No coding tool? The prompts below work as-is in any agent that can reach your inbox, calendar, and sheets.

---

## 💬 Prompts to try

<details>
<summary><b>Sourcing & tracking</b></summary>

- "Watch for new internship postings at these companies and ping me only when something real opens."
- "Log this application in my tracker: [link]. Stage: applied."
- "Sweep startup boards for roles my tracker missed."
- "Add this role to my opportunity tracker and score the fit: [link]."

</details>

<details>
<summary><b>Applications & resumes</b></summary>

- "Fill this application portal and stop before submit: [link]."
- "Score my resume against this job description and list the gaps: [link]."
- "Rewrite my LinkedIn headline so recruiters actually find me."
- "Write the 'why this company' answer for this application from my resume: [link]."

</details>

<details>
<summary><b>Outreach & interviews</b></summary>

- "Draft a cold email to the recruiter on this posting. Don't send it."
- "Find a verified email for this recruiter, or tell me it's LinkedIn-only: [LinkedIn URL]."
- "A rejection came in from [company]. Log it, and draft a follow-up if it's worth saving."
- "I have a HireVue due Friday - put it on my calendar and remind me the day before."

</details>

---

## 🛡️ Ground rules the agent works under

- 🚫 **Nothing sends without approval.** Drafts sit in Gmail until you say go, one at a time.
- ✅ **No invented numbers.** Resumes and outreach reframe what is true; they never fabricate.
- ⛔ **Employer rules are hard stops.** If a posting bans AI assistance, the agent preps instead of writes.
- 🤫 **Quiet days stay quiet.** A watch with nothing real to report says so and stops.
# Instinct for Recruiting

One personal agent running the whole job hunt: sourcing, applications, outreach, referrals, interviews, and the logistics around them. Everything in this repo is a use case that has actually run.

## What is Instinct

Instinct is a personal AI agent. You text it like a person; it works like a teammate who never sleeps.

Two pieces make that possible:

- **Connectors** link your accounts - Gmail, Calendar, Sheets, Docs, and more - with your permission. The agent reads what it needs and works where you already live: drafts in your Gmail, rows in your Sheets, events on your calendar.
- **The vault** holds your credentials securely. When a site needs a login, the agent signs in for you without a password ever passing through a chat.

## The split

The agent does the ninety percent: sourcing, research, form filling, drafting, tracking, follow-ups. You do the last two minutes where a portal walls automation (captchas, logins, no-AI rules) and the one tap where your name goes on a send.

## Use cases

| # | Use case | What it is |
|---|----------|------------|
| 1 | [Daily internship drop watch](use-cases/01-daily-internship-drop-watch.md) | Verified-open postings every day, kills included |
| 2 | [Application pipeline tracker](use-cases/02-application-tracker.md) | One live sheet for every role, stage, and deadline |
| 3 | [Application autofill](use-cases/03-application-autofill.md) | Portals filled with standing answers and the right resume |
| 4 | [Cold recruiter outreach](use-cases/04-cold-recruiter-outreach.md) | Drafts staged and ready, sent one at a time on approval |
| 5 | [Recruiter email discovery](use-cases/05-recruiter-email-discovery.md) | Addresses derived from confirmed patterns only, never guessed |
| 6 | [Resume ops](use-cases/06-resume-ops.md) | JD-versus-resume fit scores and gap lists per role |
| 7 | [LinkedIn SEO/AEO audit](use-cases/07-linkedin-seo-aeo-audit.md) | Headline and profile benchmarked against profiles that rank |
| 8 | [Interview logistics](use-cases/08-interview-logistics.md) | Assessments, recorded interviews, and deadlines tracked |
| 9 | [Conference trip prep](use-cases/09-conference-trip-prep.md) | Flights priced and ranked, outreach prepped before wheels up |
| 10 | [Referral tracking](use-cases/10-referral-tracking.md) | Referrals verified as actually attached, not assumed |
| 11 | [Standing company watches](use-cases/11-standing-company-watches.md) | A dedicated eye on target employers' career pages |
| 12 | [InMail copy doc](use-cases/12-inmail-copy-doc.md) | Ranked, copy-paste-ready LinkedIn blocks |
| 13 | [Role sweeps](use-cases/13-role-sweeps.md) | Wide passes for roles beyond what the tracker caught |
| 14 | [Application answer drafting](use-cases/14-application-answer-drafting.md) | Portal essays and short answers written from real material |

## Prompts to try

- "Watch for new internship postings at these companies and ping me only when something real opens."
- "Log this application in my tracker: [link]. Stage: applied."
- "Fill this application portal and stop before submit: [link]."
- "Draft a cold email to the recruiter on this posting. Don't send it."
- "Find a verified email for this recruiter, or tell me it's LinkedIn-only: [LinkedIn URL]."
- "Score my resume against this job description and list the gaps: [link]."
- "Rewrite my LinkedIn headline so recruiters actually find me."
- "I have a HireVue due Friday - put it on my calendar and remind me the day before."
- "Sweep startup boards for roles my tracker missed."
- "Write the 'why this company' answer for this application from my resume: [link]."

## Ground rules the agent works under

- Nothing sends without approval. Drafts sit in Gmail until you say go, one at a time.
- No invented numbers. Resumes and outreach reframe what is true; they never fabricate.
- Employer rules are hard stops. If a posting bans AI assistance, the agent preps instead of writes.
- Quiet days stay quiet. A watch with nothing real to report says so and stops.
