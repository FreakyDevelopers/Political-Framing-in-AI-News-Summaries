# What's This Project About?

## The Problem

So AI summaries are everywhere now. You see them in news apps, chat interfaces, all over. But here's the thing—summarizing isn't neutral. Every time you summarize, you're choosing what to include, what to drop, and what tone to use. Those choices matter.

I wanted to actually test whether different AI models make the same choices or if they diverge.

## What I Did

I picked six immigration news articles: left-leaning, center, and right-leaning sources. Then I fed them all to five different AI models—ChatGPT, Claude, Gemini, Grok, DeepSeek—with the same neutral prompt asking for 140-160 word summaries.

I manually coded all thirty summaries (6 articles × 5 models) looking at: neutrality, emotional language, political framing, accuracy, and whether anything important got left out.

## What I Found

All five models could produce readable summaries, but they didn't perform the same:

- **Claude** ranked highest overall quality-wise. Consistently solid.
- **Grok** was best at including details. Good for completeness.
- **ChatGPT** made smooth reading but cut corners on important stuff sometimes.
- **Gemini and DeepSeek** were all over the place—depended heavily on the article.

There's also a pattern with source orientation: when the original article came from a left-leaning source, the AI summaries tended to get coded as more negative. Right-leaning sources? The summaries leaned positive. Center-source articles? Cleanest results.

The big insight: these summaries *sound* neutral but they're not. They inherit framing from the source material and shape reader understanding through emphasis and omission.

## Real Talk: What This Doesn't Prove

This is exploratory. One coder, six articles, one topic. You can't generalize this to "all AI systems" or even "all news topics." 

It's more of a "here's a methodology and some interesting patterns" than a "AI is definitely biased about immigration." Future work would need more articles, multiple coders, more topics, and better statistical rigor.

But it does suggest something worth digging into further.
