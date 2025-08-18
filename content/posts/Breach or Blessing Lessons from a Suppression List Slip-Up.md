---
date = 2025-08-18
aliases =
  - "Breach or a Blessing: Lessons from a Suppression List Slip-up"
tags =
  - blogpost
  - published
  - GDPR
  - Accountability_Principle
  - Data_Minimisation
  - Purpose_Limitation
title = 'Breach or a Blessing: Lessons from a Suppression List Slip-up'
published: true
---

Originally published [here](https://insights.priva.cat/p/breach-or-blessing-lessons-from-a?r=1x369k)

A data protection lesson on what can happen when you accidentally send emails to your suppression list

How many times have you received an 'Oops, we screwed up' email in your inbox? Y'know, after you got some random marketing message from a website you thought you'd opted out of years ago?

If you're me the answer is probably 'once a week, for the last 20 years'. It's a common enough occurrence that most of us shrug, and chalk it up to 'shit happens'. Except for that handful of folks who take great umbrage that their inbox has been besoiled by this misdirected missive.

Still, it feels *awful* if you're the poor bastard who sent the email. And it's also mildly nerve-wracking and anxiety-inducing if you're the organization ultimately responsible. I suspect this is why some companies send out an email which blames the poor intern.

A few weeks ago, one of my clients, a medium-sized charity, called me in a bit of a panic after they had unintentionally committed this venial email sin. As part of a marketing appeal, they had sent out a message both to their subscribers and accidentally included around 10,000 people who had previously unsubscribed. Whoops!

They had, in short, violated both the GDPR, and probably the ePrivacy Directive. They'd also arguably caused a technical [data breach](https://castlebridge.ie/insights/data-quality-and-data-protection-a-dpc-decision/) (at least from the DPC's perspective), though not a reportable one. But for today's post, I want to focus on one failure mode: my client's breach of the accountability principles under Article 5 of the General Data Protection Regulation. For those who don't have the GDPR on mental speed dial, Article 5 says, amongst other things that personal data must be:
* collected for specified, explicit and legitimate purposes **and not further processed** in a manner that is incompatible with those purposes;
* **accurate** and, where necessary, **kept up to date**;
* processed in a manner that **ensures appropriate security of the personal data**, including protection against **unlawful processing**, **using appropriate technical or organizational measures**.

These principles are often short-handed by data protection folks as the purpose limitation, accuracy, and security principles of accountability, and they are the foundational pillars of the GDPR (and many other data privacy/protection laws).[^1] Without the accountability principles, you might be saying you 'care about privacy' on paper, but you aren't protecting personal data. Or complying with the law.

In this case, my client had accidentally and unlawfully processed emails stored on their opt-out/unsubscribe list for a purpose that wasn't valid (i.e., they had no **lawful basis** to send out marketing emails to people who had unsubscribed).[^2] They also should have had better technical and organizational measures in place to avoid sending out these emails in the first place. But there's also an interesting accuracy issue buried in this tale as well. I'll get to that in a minute. In short, all of this can be chalked up to a case of poor data quality and data management as far as their email suppression list was concerned.

My client didn't do any of this on purpose, of course, and after we chatted for a bit, I gave them some guidance, and they addressed the problem in a timely, respectful, and apologetic way. As was the case, most recipients took the whole thing in stride and ignored the message and the apology email entirely. But a small percentage (around 0.16%) responded, with an even smaller number (~10 individuals) asking for access to their information or requesting that their data be erased. A few others responded negatively, but didn't otherwise ask for anything. This is all very much par for the course.

What made this story interesting (and therefore blog-worthy) though, was that within that 0.16% response rate, most people who received the unwanted email were surprised that they had been unsubscribed at all and asked to be resubscribed. Some of them even took the opportunity to donate to the charity!

My clients were elated to have something good come out of this slightly embarrassing error.
# Experience Really is the Best Teacher
That said, I don't think that anyone should treat this as some sort of new marketing strategy or anything. The vast majority of cases where I've witnessed this as a DPO, have usually led to a large number of angry people and demands to be removed again, with threats to complain to the regulator. My charity client's case was extraordinary, and was probably based on a combination of dumb luck & the fact that they represents a very worthy cause.

But there are a few data protection-related teachable moments in all of this that I want to share:
1. **Poor Data Quality & Data Management**: As I mentioned at the outset, my client's data quality practices fell short of the ideal in this case. Operationally, for reasons I can't really discuss, it was easy for this particular mistake to have occurred, and for it to have hit such a large number of former subscribers. Certain technical controls were quite brittle, or missing altogether, including the workflows for handling unsubscribe requests and suppression lists.

	It turns out that having good, robust data quality practices is really hard, and depending on the organization's systems, and its technical, and financial constraints, perfect data quality/management may not always be achievable. Bad, mungy, and/or inaccurate data means there's always a risk for something to go wrong, and limited budgets and resources spread organizations thin -- even if they want to do the right thing. It doesn't help that most companies see data protection as a cost-center, rather than a way to build goodwill and customer relationships.

	 That said, we're all (data) sinners here, and anyone who claims that their house is perfectly in order (or that they're 100% GDPR compliant) is probably lying, or trying to sell you something. Still, we should all strive to be better, and to meet the standards that the laws require. Fortunately, my client has been taking steps to improve their processes in response to this bit of human fallibility. As the wise data sages say, never let a good crisis / data breach go to waste.
2. **Bad Data Management Leaves Money on the Table**: When I was chatting with Daragh O'Brien, who has [ been doing the whole data quality/management thing for a long time](https://castlebridge.ie/team/daragh-o-brien/), he shared a valuable insight: my client's unsubscribe process was a blunt tool, rather than a precise, user-empowering data management process. And because of that, my client has literally been leaving money (and supporters) on the table.

	To comply with laws like the ePrivacy Directive, most emails from organizations (commercial or nonprofit) have an unsubscribe / consent management workflow that looks something like this.
	a. A person signs up to receive emails from the organization (e.g., to donate money, participate in a survey, or find out about an upcoming event).
	b. The messaging and purposes are overly broad / all-or-nothing. In addition to the stuff you want, you also get loads of emails you don't care about at all.
    c. The organization sends dozens of undifferentiated emails to the person who signed up.
    d. The person gets annoyed, and clicks the unsubscribe link, where they're presented with something like this, and maybe a survey on why (which nobody reads):

![[Modal asking Do you want to unsubscribe from this list.png]]

    e. The user unsubscribes, and promptly forgets about the 
    organization. 

But a better approach would be for the unsubscribe feature to look more like this:
![[Pasted image 20250219195234.png]]
Now, I'll leave it to the UX and marketing pros to explain why this may or may not be better from a design perspective, but it's absolutely better from an accountability/accuracy/data minimization perspective. Though I would put the unsubscribe from all at the top, and not the bottom of the message, and I'd probably leave those other boxes unchecked.

# Be Better About Your Purposes

First, this approach gives individuals more control over what they **actually want to see** without adding (much) cognitive load. For example, I might enjoy receiving emails about events, initiatives, and a general email about what the organization is doing. But as a yearly donor to a few charities, I do not need to see a donor appeal message every week. Not only is that sort of thing generally ineffective, it gets annoying, especially if everyone is doing it. Either align your processing with your stated purposes, or at least let people decide how often they want to hear from you.

Sadly, most unsubscribe options are usually binary -- if it's between 5-10 annoying emails a week or nothing -- I'm going to go with nothing every time.[^3] The organization loses engagement, and the individual forgets the organization exists -- until they receive that accidental email fired off to the suppression list.

My client was legitimately surprised (and moderately delighted) that many of their supporters were unaware that they had been unsubscribed. *But it isn't surprising at all -- it's bad data management.* If they'd had more granular subscription options, that handful of one-off donors might have been ongoing/recurrent donors -- and the relationship would have been stronger with those people.

But there's a second reason for granularity here: It provides organizations with better, less obtrusive metrics on what works (and what doesn't). Say, the marketing team is firing off weekly donor appeals / product announcements / upsells, or those pointless 'Step 1 of 49 of how to use our product' messages that nobody actually reads. A targeted unsubscribe (and/or an email frequency toggle) provides more clarity on exactly what people are sick of seeing -- and what they're comfortable with, as well as how often they want to see it. And it avoids the organization fading into the shadows, never to be considered again.

Above all, it tightly couples the data collection and processing purposes in a transparent way, and dramatically lowers the shock factor of receiving a sudden email out of the blue.

I get that I am likely scandalizing/offending marketing pros with this -- and as I mentioned above, there may be better approaches from a user experience perspective. But from a data protection angle, provided that the options are tightly coupled with the exact purposes of processing, not hidden in a dark pattern maze, and are clear and easy to distinguish, an organization will be in a better place overall.

Though I'm sure that no matter what you do, you'll always get that small percentage of people outraged that they received that accidental email after unsubscribing. But at least you'll make less of your customers (or your DPO) sad.

---

[^1]: Some pedants might also argue that this violated the data minimisation and storage limitation principles (5(1)(c) and 5(1)(e) GDPR), and to that I say, go duke it out in the comments. And for you ePrivacy Directive geeks, yes, I know that's also an issue. Don't @ me.
[^2]: To be clear, my client *did* have a lawful basis for keeping the emails -- they needed to know who to avoid emailing, after all.
[^3]: Looking at you, security compliance vendor who shall remain nameless, but should absolutely know better. My client does not do this, because they know I would be sad.