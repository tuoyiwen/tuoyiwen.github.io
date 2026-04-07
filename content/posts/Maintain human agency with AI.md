---
title: How can we develop agency when working with AI? Four takeaways
date: 2026-04-07
draft: false
tags:
  - AI
  - Human Agency
  - Bandura
  - Human-AI Interaction
---

How can people effectively interact with AI? As tools like Claude, GPT, and Gemini become part of daily work, this question gets more urgent by the month.

Simon Willison, Django co-creator and one of the most prolific AI engineers alive, was asked exactly this on Lenny's Podcast. His answer wasn't "learn to code" or "master prompt engineering." It was simpler:

> "Invest in your own agency."

But what is agency, exactly? What are its properties? And how can we develop it when working with AI? Simon didn't dig into these questions. Drawing from Bandura's (2006) Psychology of Human Agency, I answer these questions, walk through an example to demonstrate the ideas, and provide a Claude skill you can copy for practicing agency. The goal is to advance your understanding of what agency actually means when collaborating with AI, and give you concrete tools for developing it.

---

## What Is Agency?

Albert Bandura, one of the most cited psychologists in history, spent decades studying why some people shape their circumstances while others are shaped by them. His answer: **agency, the capacity to intentionally influence one's own functioning and life circumstances.**

The core premise is that people are not passive products of their environment; instead, they are self-organizing, proactive, self-regulating, and self-reflecting. Bandura identified four properties that make someone an agent rather than a spectator. Each one maps onto how we interact with AI, and each one can be deliberately developed.

---

## The Four Properties of Agency and How to Develop Them

### 1. Intentionality

Agents form intentions that include action plans and strategies for realizing them. This is more than "having a goal." It means constructing a mental blueprint for how to get there and committing to execute it.

**How to develop it**: Before each work session, ask yourself: *What is the most important problem I should work on today, and why?* Then use AI to help solve it. This reverses the default pattern, where AI's capabilities drive your agenda. You become the director, not the responder.

> **Takeaway 1**: *What is the most important problem I should solve, and why?*

### 2. Forethought

People set goals, anticipate likely outcomes, and use those anticipated futures to guide present behavior. Bandura called this "anticipatory self-guidance": you bring a visualized future into the present as a motivator.

With AI, forethought means forming a hypothesis *before* you prompt. What do you expect the answer to look like? What would a good solution include? 

**How to develop it**: Before asking AI anything non-trivial, think what you expect the answer to look like. This takes 30 seconds. It transforms you from a passive consumer into an active evaluator. When the AI response arrives, you have something to compare it *against*, not just something to accept.

> **Takeaway 2**: *What would a good response include? 

### 3. Self-Reactiveness

Agents don't just plan. They construct appropriate courses of action, motivate themselves to follow through, and regulate their execution against internal standards. This is self-regulation: the internal feedback loop that keeps you on course even when no one is watching.

Here's the AI trap. When AI output *looks* polished, the self-regulatory alarm doesn't fire. The output seems fine, so you accept it. But "looks fine" and "meets my actual standard" are different things. Self-reactiveness means checking the output against what *you* know to be true, not just whether it reads well.

**How to develop it**: Don't accept AI output just because it's fluent. Compare it against what *you* know. If you can't tell the difference between "reads well" and "actually good," that's a signal. Your standards need recalibrating. Go back to the source material. Rebuild your own judgment.

> **Takeaway 3**: *Does this meet my actual quality bar, or does it just read well?*

### 4. Self-Reflectiveness

Agents examine their own functioning. They reflect on whether their thinking is sound, whether their strategies are working, whether they are developing or stagnating. Bandura called this "the most distinctly human core property of agency."

In the AI context, self-reflectiveness is the meta-question: *Am I getting better at this, or is AI getting better at doing it for me?* If you can't answer that, you've already started slipping.

**How to develop it**: Once a month, try doing a meaningful task without AI. Not as a stunt. As a diagnostic. Can you still structure an argument from scratch? Can you still spot the flaw in a dataset without AI pointing it out? If the answer is "not as well as before," you're in an erosion spiral. Catch it early.

> **Takeaway 4**: *Can I still do this without AI? Am I building skill, or building dependence?*

---

## Putting It All Together: Building an Argument

As a PhD student, one of the most important things I do is build theoretical arguments. It's also one of the first things people outsource to AI.

**Without agency**: You open Claude. You type "build a theoretical argument for why AI feedback enhances employee creativity." The output is structured, logical, and cites real papers. You clean up the wording, paste it into your draft, and move on. It reads like a real argument. But you didn't choose *why* this argument matters. You didn't anticipate what the counterargument would be. You didn't check whether the logic actually holds against what you know from the literature. And next time you need to build an argument, you'll do the exact same thing: open AI and ask.

**With agency**:

*Intentionality*: Before opening any tool, you decide what problem you're actually solving. "My paper's weakness is that the mechanism is underspecified. I need to build the argument for *why* AI feedback triggers creative engagement, not just *that* it does." You've chosen the problem.

*Forethought*: You sketch your own logic first. "I think the mechanism runs through self-efficacy: AI feedback that highlights what the employee did well increases their belief that they can be creative, which drives more experimentation." It might be wrong. That's fine. Now you have something to test AI's output against.

*Self-reactiveness*: You prompt AI to generate alternative mechanisms. It suggests three: self-efficacy, cognitive offloading, and psychological safety. The self-efficacy path aligns with your intuition but AI frames it differently than you expected. The cognitive offloading argument sounds elegant but doesn't match the empirical evidence you've read. You keep what holds up. You discard what doesn't. You're evaluating, not accepting.

*Self-reflectiveness*: After the session, you ask: "Do I understand this mechanism better than I did an hour ago? Could I explain it to my advisor without notes?" If yes, you've built skill. If the answer is "I'd need to re-read the AI output to explain it," you've built dependence.

The draft might look similar either way. The difference is what happened inside you. One version made you a better researcher. The other just made your document longer.

---

## Bonus: A Claude Skill for Practicing Agency

I built a Claude skill that turns these four takeaways into a reusable checklist. You can copy the prompt below into your own Claude project instructions, and then type `/agency-check` before or after any AI-assisted work session.

```
# Agency Check — Develop Human Agency with AI

Based on Bandura's (2006) Psychology of Human Agency.
Use before, during, or after an AI-assisted work session.

## Pre-Flight: Before You Start

Walk through these four questions before working with AI.

1. INTENTIONALITY
   Ask: "What is the most important problem I want to solve right now, and why?"
   If the answer is vague, push further: "What would a good outcome look like?"
   Do not proceed until you have a clear direction.

2. FORETHOUGHT
   Ask: "What do I expect a good answer to look like? What would surprise me?"
   If unsure, flip it: "What would a bad answer look like?"
   Write down your expectation. This is your benchmark.

3. SELF-REACTIVENESS (Set Standards)
   Ask: "What is my quality bar for this task? How will I know if the output
   is actually good versus just reads well?"
   Name specific criteria: accuracy, depth, fit with what I already know.

4. CONFIRM
   Summarize: "My goal is [X]. I expect [Y]. My quality bar is [Z]."
   Now proceed.

## Post-Session: After You Finish

1. SELF-REACTIVENESS CHECK
   "Did the output meet the quality bar I set?
    Or did I lower it because the output sounded good?"

2. SELF-REFLECTIVENESS CHECK
   "Did I learn something I could apply without AI next time?"
   "Could I do a better version of this, with or without AI?"
   "If the answer is 'I would just prompt AI again the same way,'
    what does that tell me?"

## Remember
Agency is not a trait. It is a practice.
It strengthens with use. It atrophies with disuse.
```

Feel free to adapt it. The point isn't to follow it rigidly — it's to build the habit of directing AI rather than being directed by it.

---

## The Bottom Line

AI is getting better at execution every month. That's not going to stop. The question is what happens to the human on the other side of the screen.

If you let AI handle the doing *and* the deciding, you gradually become a reviewer of its work rather than a director of your own. The output may stay high, but the agency quietly drains.

But if you invest in the four capacities Bandura identified, something different happens. You use AI *more* effectively because you bring clearer intentions, sharper hypotheses, higher standards, and honest self-awareness to the interaction. The tool gets better. And so do you.

---
Source:
- *Bandura, Albert. 'Toward a Psychology of Human Agency'. _Perspectives on Psychological Science_ 1, no. 2 (2006): 164–80. [https://doi.org/10.1111/j.1745-6916.2006.00011.x](https://doi.org/10.1111/j.1745-6916.2006.00011.x).
- *Simon Willison's appearance on [Lenny's Podcast](https://lennysnewsletter.com/p/an-ai-state-of-the-union) (April 2026).*
