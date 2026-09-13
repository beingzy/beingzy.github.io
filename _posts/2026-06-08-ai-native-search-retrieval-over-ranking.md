---
layout: post
title: "AI-Native Search: Retrieval Over Ranking"
date: 2026-06-08
categories: ai
description: "A short note from a conversation with Ray on why search engines built for agents should optimize for evidence coverage, not first-page ranking."
---

Yesterday I chatted with my friend Ray. We share a similar path: PhD years in the US, startup scars from crypto, and now a lot of time thinking about the AI layer.

The question was simple: if AI agents become real users of the internet, what should a search engine optimize for?

Classic search was built for humans. Human attention is narrow. In one search round, most people can only inspect a small number of results, often single digits. That makes ranking central. The product is not just retrieval; it is the ordering of a tiny list.

AI changes the constraint. A model context window is not infinite, but compared with human attention it is practically vast. An agent can read, compress, compare, and revisit far more material than a person would tolerate.

So the core job shifts.

For human search, the question is:

> What are the best ten links to show first?

For AI-native search, the question is:

> Can we reduce millions of possible items into a high-recall set of thousands, where nearly every plausible answer or decisive source is still inside?

Ranking still matters, but its purpose changes. It should not only predict what a person would click. It should estimate marginal reasoning value: novelty, source quality, contradiction, coverage, freshness, and whether a document helps verify or falsify an answer.

The better mental model is evidence acquisition. An AI-native search engine is not mainly a page-ranking machine. It is a retrieval system that feeds a reasoning loop.

That suggests a different product metric: not first-result satisfaction, but whether the agent can assemble a complete enough evidence set to answer correctly, cite properly, and notice when the answer is uncertain.

Google ranks the web for human attention. AI-native search retrieves the substrate for machine reasoning.
