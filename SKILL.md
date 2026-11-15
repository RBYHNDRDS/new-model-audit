---
name: new-model-audit
description: Audit a marketing or ecom team's AI working setup (brand files, offer docs, claims lists, customer research, briefs, prompts, skills, custom instructions, angle and test logs) for contradictions, outdated instructions, missing inputs, and rules that only exist because an older model needed them, then retest one finished job. Read-only. Every finding carries the file and the quoted line, and nothing changes without approval. Use when a new model has just been released, when the user asks to audit, clean up or sanity-check their setup, brand files, briefs or ad workflow, or when they want to know whether a new model is actually better on their own work.
---

# New Model Audit

A new model is the cheapest audit a team gets all year. Their setup has collected months of patches, old offers and rules nobody remembers writing. A fresh model reading all of it with no history is well placed to see what no longer fits.

The audit does two jobs at once. The user learns how good the model is, because it is being tested on work they know inside out. And their setup gets cleaner.

No ads, scripts or briefs get written during the audit. The only writing comes at the very end, in the retest.

## Ground rules

These hold for the whole run.

- **Read-only.** Do not edit, rename, move or delete anything in the user's setup. The audit produces a report. Changes come later, one at a time, after the user picks them.
- **Quote or it doesn't count.** Every finding names the file and quotes the exact line. A finding you cannot quote goes under "unsure", with what you would need to see to confirm it. This is what lets the user check your work in seconds, and it stops you from reporting an impression as a fact.
- **Read everything you report on.** If the setup is too big for one pass, read it in batches and keep a running inventory. Say plainly which files you skipped, skimmed or could not open. Never describe a file you did not finish.
- **Don't guess what is current.** You often cannot know whether a price, promo or product still exists. When you can't tell, put it on the "ask the team" list instead of calling it outdated.
- **Sort by damage.** Each finding goes in one of three groups: breaks the work, causes confusion, nice to fix. If everything lands in the first group, sort again.
- **Keep it local.** Do not send the user's files to any outside service. If you come across a password, key or customer record, report where it is and never repeat the value.

## Step 0. Find the setup

Work out where the setup lives. If the user pointed at a folder or attached files, use those. If not, look for the obvious places (a project folder, a skills or prompts directory, a brand or client folder) and confirm with the user before reading. Ask at most one question here.

A full setup usually has:

- brand voice and guidelines
- product and offer docs
- a list of claims they can and cannot make
- customer research and personas
- angle logs and test results
- recent briefs
- every prompt, skill and custom instruction the team uses
- a few ads that worked and a few that did not, with numbers

Missing pieces are not a reason to stop. They are findings for step 4.

Ask the user for one finished job they were happy with (a brief, a script, a set of hooks) together with the input it was made from. Step 8 needs it. If they have none, skip step 8 and say so in the report.

## Step 1. Inventory

List every file you read with one line on what it is for. Mark anything you could not open or did not finish.

Show this to the user first and let them correct it. If you have a file's purpose wrong, every later finding built on it is wrong too.

## Step 2. Contradictions

Find every place where two files, or two parts of one file, disagree.

For each one: quote both lines with their file names, say which one looks current and why, and say what would go wrong in an ad or brief if someone used the wrong one.

Where ecom teams usually have them:

- **Offer.** Price, bundle, discount, guarantee, returns or shipping differs between the offer doc and the briefs.
- **Claims.** An old script or prompt uses a claim the claims list forbids.
- **Customer.** The persona doc describes one person and the winning ads talk to another.
- **Voice.** The guidelines say one thing ("never salesy") and a prompt asks for the opposite ("urgent, hard-selling").
- **Naming.** One product under several names, or one name for several products.
- **Rules.** The same rule written in three places with three wordings that no longer agree.

## Step 3. Outdated

Find what looks out of date. Quote the line and say what made you think it is old.

Look for: products, prices, bundles and promos that may be gone. Dates and seasons that have passed. Ad formats and platform specs. People, tools and links that may no longer exist. Angles still marked as "testing" long after a decision. Instructions aimed at a problem the team no longer has.

Anything you cannot confirm goes on the "ask the team" list.

## Step 4. What's missing

Imagine you had to write a new ad for this brand tomorrow with only these files. List every question you would have to ask first.

Then list what is missing, ranked by how much it would improve the work. For each: what it is, which file it belongs in, and what a good version looks like.

The gaps that come up most:

- proof (reviews, numbers, studies) with a source for each
- real customer language from reviews, support tickets and surveys
- objections and the answer to each
- why the losing ads lost (most logs only record winners)
- which landing page each angle sends people to
- what the brand never says, and the reason
- one finished example of "good" for each type of thing the team makes

## Step 5. Briefs

Read the most recent briefs, three if there are that many. For each one, report:

1. What a freelancer who has never worked with the team would still have to ask before making the ad.
2. Whether it has one customer, one angle and one promise, or several pulling against each other.
3. Which lines are opinion with no proof behind them.
4. Whether the ad it describes matches the page it sends people to. Only judge this if the page is in the files or the user gives it to you.

Then name the fields the brief template is missing. Common ones: how aware the customer is of the problem, the proof itself instead of a pointer to a drive, the linked landing page, format and length and placement, and a past winner in the same format as reference.

## Step 6. Workflow and leftover rules

Reconstruct how an ad gets made, from idea to launch, from the process docs and the order the prompts are used in. If you cannot reconstruct it from the files, ask the user to describe it in a few lines.

Walk through it and report:

- where two steps do the same job
- where something is decided with no rule or source behind it
- where a mistake could get through with nobody checking (a claim that is never checked against the claims list, test results that never make it back into the angle log, copy that goes live with no person approving it)
- which instructions are so long or so loud (caps, repeated warnings) that they crowd out the important ones
- which instructions look like they were written to stop an older model making a mistake, and that you would follow without being told

Be careful with that last group. Your own belief that you no longer need a rule is a guess until it is tested. So these go on a list called "test removing", never "remove". The test is simple: take one rule out, run the same job, compare.

## Step 7. Proposed changes

From everything found, give the ten changes that would improve the work most, ranked. For each: the change, the file, roughly how long it takes, and what could go wrong if it is made. Then name the three to do today.

The user decides. After they pick, apply the changes one at a time and keep a short change log (date, file, what changed, why), so that if output gets worse they know what caused it.

## Step 8. Retest on real work

Take the finished job from step 0. Make it again from the same input and the same files, without looking at the earlier output first.

Then show both versions to the user as A and B, in random order, without saying which is which. Let them pick before you reveal it. Tell them the comparison is fairer still if someone who has not seen either version does the picking.

Check every fact and claim in your new version against the files, line by line, and report anything you could not back up.

If changes from step 7 have been applied, run the job once more afterwards. A cleaner setup should show up in the output. If it does not, say so.

## The report

Give the report in the conversation. Save it as a file only if the user asks.

1. **Verdict.** Three or four plain sentences: what state the setup is in, and the single most damaging problem.
2. **Inventory.** Files read, files skipped.
3. **Breaks the work.** Findings with file and quote.
4. **Causes confusion.** Same.
5. **Nice to fix.** Same, kept short.
6. **Ask the team.** What you could not confirm, as questions.
7. **Missing.** Ranked.
8. **Test removing.** The leftover rules.
9. **Top ten changes** and the three for today.
10. **Retest.** A and B, then the reveal.
11. **Unsure.** What you suspect but could not quote.

Write for someone who runs a brand, in everyday words. Lead with what matters and leave out the tour of how you got there.

## Check your own audit before you send it

- You found nothing, or "everything looks consistent". Real setups are never clean. You most likely did not read all of it. Go back to the inventory.
- A finding has no quote. Find the line or move it to "unsure".
- Dozens of findings, all urgent. Sort again. The user can act on five things, not sixty.
- You reported something as outdated when you only suspect it. Move it to "ask the team".
- You changed a file. Undo it, tell the user, and go back to read-only.
