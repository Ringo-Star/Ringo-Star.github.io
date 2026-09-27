---
layout: post
title: "Research note: [the question you want to understand]"
date: 2026-09-27 12:00:00 +1000
description: "[One sentence explaining the question, your perspective, and what readers will learn.]"
tags: [diffusion, generative-modeling]
categories: [research]
author: Yasong Dai
published: false
related_posts: false
giscus_comments: false
toc:
  sidebar: left
---

{% comment %}
AUTHOR SETUP — this block is not displayed on the website.

An original research-writing scaffold inspired by the organization of Lilian
Weng's Lil'Log: motivation, foundations, technical detail, comparisons, and
references. It does not reproduce her prose or change your site's theme.
Reference: https://lilianweng.github.io/posts/2021-07-11-diffusion-models/

1. Copy to _posts/YYYY-MM-DD-your-topic.md in your repository.
2. Replace the title, date, description, tags, and bracketed placeholders.
3. Keep published: false while drafting. Set published: true when ready.
4. Your repository already enables MathJax globally. Use $$ for inline and
   display mathematics, as in its existing math example post.
5. Preview locally with: bundle exec jekyll serve --unpublished
   This also shows other unpublished posts locally. Do not deploy that flag.
6. Enable Blog by changing nav: false to nav: true in _pages/blog.md.
   Keep its existing layout and pagination settings.
7. Replace the existing values in _config.yml (do not append duplicate keys):
   blog_name: "Research Notes"
   blog_description: "Notes on diffusion models, learning, and inference."
   display_tags: [diffusion, generative-modeling]
   display_categories: [research]
8. Before exposing Blog, review the bundled demo posts in _posts/ and set
   published: false in their front matter if you do not want them public.
   Inspect external_sources in _config.yml too: remove template feeds you
   do not want imported. Display tags/categories are links, not filters.
9. Optional: enable latest_posts in _pages/about.md to show posts on Home.

No repository files have been changed by downloading this template. The
front matter follows the repository's existing post and sidebar-TOC examples;
a full Jekyll build and browser preview have not been performed.
{% endcomment %}

> **In one paragraph:** [State the problem, central idea, and main takeaway.
> Say whether this is a literature review, an explanation, or a preliminary
> research idea. Avoid presenting an untested idea as a result.]

**Prerequisites:** [For example: basic probability, neural networks, and ODEs.]

## Why this question interests me

[Start with a concrete difficulty or observation. What works already, what
remains difficult, and why does that gap matter? Connect this to your research
focus in two or three paragraphs.]

*Optional opening to adapt:* My research focuses on diffusion generative
modeling, particularly how training and inference dynamics affect what these
models can do. In this note, I want to examine one specific question:
**[insert the question]**. I will first introduce the necessary background,
then compare existing approaches, and finally describe what I would like to
test next.

## Background and notation

[Introduce only the concepts needed for this post. Explain each idea in words
before introducing its mathematical form. Link to the original papers.]

| Symbol | Meaning |
| --- | --- |
| $$x$$ | [Define the data or state variable.] |
| $$z$$ | [Define the latent variable, if needed.] |
| $$c$$ | [Define the conditioning information.] |
| $$\theta$$ | [Define the model parameters.] |

### A minimal mathematical setup

[Replace this generic equation with the central equation of your topic.]

$$
\hat{x} = G_\theta(z, c).
$$

[Explain the input, output, and role of each term. State the assumptions:
for example, whether this map is deterministic and whether any randomness
is included in its inputs. Do not leave these choices implicit.]

## The core idea

### Intuition first

[Explain the mechanism using one concrete example. Describe what changes at
each step and what information is preserved or lost.]

### Then the technical details

[Develop the argument step by step. For each equation, explain what it says,
why it follows, and where the approximation or assumption enters. Cite a
source when the derivation comes from prior work.]

### A figure that explains the mechanism

[Add a diagram or visual comparison here. It should answer a specific question,
such as where conditioning enters or how two methods differ.]

{% comment %}
After creating the actual image, uncomment and edit this figure block.
Use your own diagram or attribute an appropriately reusable source.

<figure>
  <img src="{{ '/assets/img/posts/your-topic/overview.png' | relative_url }}"
       alt="Describe the mechanism and the relationships shown in the figure."
       loading="lazy" style="max-width: 100%; height: auto;">
  <figcaption>Figure 1. Explain the key observation. Source: [attribution].</figcaption>
</figure>
{% endcomment %}

## How existing approaches differ

[Organize the literature around ideas and trade-offs, rather than listing
papers chronologically. Use comparable settings when discussing performance.]

| Approach | Main mechanism | Strength | Limitation | Source |
| --- | --- | --- | --- | --- |
| [Baseline] | [What it does] | [When it helps] | [Where it struggles] | [Paper link] |
| [Alternative] | [What changes] | [Benefit] | [Trade-off] | [Paper link] |

[Explain the most meaningful difference in prose. Separate a reported result
from your interpretation of why it happens.]

## My current perspective

[State what you find convincing, what you disagree with, and what remains
unclear. Connect the discussion to your work without implying that a new
idea has already been validated.]

**Working hypothesis:** [A precise, testable statement.]

**Why it might hold:** [The mechanism or evidence motivating it.]

**What would change my mind:** [An observation that would contradict it.]

## A small experiment to test the idea

[Describe the simplest experiment that distinguishes your explanation from
an alternative. Delete this section for a purely explanatory post.]

| Design choice | Specification |
| --- | --- |
| Question | [What exactly is being tested?] |
| Baseline | [Which implementation and configuration?] |
| Intervention | [What single factor changes?] |
| Held fixed | [Data, seeds, compute, and other relevant controls.] |
| Evaluation | [Metrics and qualitative examples, with reasons.] |
| Failure criterion | [What would count against the hypothesis?] |

[If you report results, include the actual setup, uncertainty where relevant,
and failure cases. If the experiment is planned, explicitly say so.]

## Open questions

1. [Which assumption is most questionable?]
2. [What might change with scale, data, or a different model?]
3. [Which question would be most useful to investigate next?]

## Takeaways

- [The central concept readers should remember.]
- [The practical implication or most important trade-off.]
- [The unresolved question motivating your next step.]

## References

[Replace these entries with verified citations and direct links. Cite sources
near the claims they support as well as listing them here.]

1. [Authors. *Paper title*. Venue or arXiv, year. URL.]
2. [Authors. *Paper title*. Venue or arXiv, year. URL.]

## Updates

- [YYYY-MM-DD: First published.]
- [YYYY-MM-DD: Describe any substantive correction or addition.]

