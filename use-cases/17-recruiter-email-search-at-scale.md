# Recruiter email search at scale

## What it does
The batch version of recruiter email discovery: Instinct, [treg](https://treg.to), and your own CLI coding agent (Claude Code, Cursor, whatever you run) split the work so a full contact batch gets enriched in one run. Same never-guess rule as the one-off version, at roughly 10x the speed.

## How it runs
- **Instinct stages the batch.** From your tracker or a target list, the agent pushes the contacts to enrich - names, companies, LinkedIn URLs - into a git repo, with the context each row needs.
- **Your CLI agent runs the enrichment locally.** You `git pull`, point your coding agent at the batch, and let it work through [treg](https://treg.to): one key over thousands of lookup and verification endpoints across providers like Hunter, Apollo, and Lusha, with per-provider pricing and measured success rates shown so the agent picks on evidence instead of a guess. Setup is one prompt to your agent: `set up treg - https://treg.to/llms.txt`.
- **Verified results write back.** Confirmed addresses land back in the tracker sheet. Anything unverified stays labeled unverified - confirmed patterns only, never guessed.

## What you get back
A contact sheet that grows by the batch instead of by the email, every address labeled verified or not, at per-lookup prices instead of per-seat subscriptions.
