# AI News Summaries: Do Different Models Tell the Same Story?

## What This Is

This is a small research project I did on AI bias in news summaries. I took six politically charged news articles about immigration, threw them at five different AI chatbots (ChatGPT, Claude, Gemini, Grok, DeepSeek), and compared what each one came up with.

The basic question: do these AIs actually summarize the same news the same way? Or do some of them spin things differently depending on the source?

I manually coded thirty summaries (six articles × five models) looking at neutrality, emotional tone, political framing, accuracy, and whether they left out important details. The data's in `/data` and the full write-up is in `/paper`.

## What I Was Actually Trying to Answer

- Do free AI models handle politically sensitive news differently?
- Does it matter where the original article came from (left-leaning source, right-leaning source, etc.)?
- Which models were most consistent?

## How I Did It

I picked six immigration news articles—two from left-leaning sources, two from center/mainstream, two from right-leaning sources. Then I gave all five AI models the same instruction: "Summarize this neutrally in 140-160 words. Don't add stuff that's not there. Don't leave out major facts. Write like a journalist."

I got 30 summaries back and coded each one for:
- **Neutrality** — does it sound balanced?
- **Emotional language** — any loaded words?
- **Political framing** — does it lean one way or the other?
- **Accuracy** — did it get the facts right?
- **Completeness** — did it miss important details?

The Excel sheet has all the summaries, my notes, and a dashboard showing how each model did.

## The Data

Everything's in `/data/research-dataset.xlsx`. You get article metadata, the exact prompt I used, all thirty summaries, coded scores, my notes on each one, and some summary charts.

[INSERT DATASET GITHUB LINK HERE]

## What I Found

Not all these models do the same thing. Here's what stood out:

- **Claude** actually scored best overall. It consistently produced balanced, complete summaries.
- **Grok** was really good at including details. If you want completeness, Grok came through.
- **ChatGPT** made smooth, readable prose but sometimes skipped important stuff.
- **Gemini and DeepSeek** were less consistent—they varied more depending on the article.
- **Center-source articles** gave cleaner results across all models. When the source was already neutral, the AI summaries were more uniform.
- **Left-source articles** tended to get rated as more negatively framed across models.
- **Right-source articles** tended to get rated as more positively framed across models.

The pattern suggests that even when AI tries to be neutral, it still inherits and sometimes amplifies the framing of the original source. It's not that the summaries are inaccurate—they sound neutral. But they're shaping reader perception through what they emphasize, what they leave out, and the tone they adopt.

## Fair Warning: Why This Isn't the Final Word

This is small. Really small. Six articles, thirty summaries, one person coding, all on immigration. You can't take this and say "all AI is biased this way." 

Other limitations:
- Only one topic area (immigration)
- One person doing the coding (so no check for bias in my coding)
- I was testing the public versions of these models, which change over time
- No statistical testing—just patterns I noticed
- These results are a snapshot from when I did the study

Think of this as an exploratory study that raises questions, not a definitive proof of anything. It's meant to show a methodology that *could* be expanded, not to make sweeping claims.

## What's in Here

- `paper/` — the full research paper (PDF and Word doc)
- `data/` — the Excel workbook with all thirty summaries and coding scores
- `docs/` — project overview
- `Assets/` — charts and graphs from the analysis
- `LICENSE` — the usual legal stuff

## Charts and Analysis Visualizations

The following charts and analysis visualizations are available in the `/Assets/ChartsAndAnalysis` folder:

- [Overall Dashboard](./Assets/ChartsAndAnalysis/OverallDashboard.png) - Comprehensive overview of model performance
- [AI Performance by Article](./Assets/ChartsAndAnalysis/AIByArticle.png) - Model comparison across articles
- [AI Performance by Article (Alternative View)](./Assets/ChartsAndAnalysis/AIByArticle2.png) - Additional article-level analysis
- [AI Performance by Article (Extended)](./Assets/ChartsAndAnalysis/AIByArticle3.png) - Further article-level insights
- [Sources Analysis](./Assets/ChartsAndAnalysis/Sources.png) - Analysis by article source orientation

## Paper

The research paper is stored in:

```text
/paper/research-paper.pdf
```

Paper title as written in the draft:

```text
Political Framing in AI-Generated News Summaries: A Comparative Pilot Study of Five Large Language Models
```

## Citation

If citing this project, use:

```text
Sharma, A. (2026). Political Framing and Accuracy in AI-Generated News Summaries: A Small-Scale Comparative Study. Independent research project.
```

## Author

**Akshit Sharma**  
Independent Researcher  
May 2026
