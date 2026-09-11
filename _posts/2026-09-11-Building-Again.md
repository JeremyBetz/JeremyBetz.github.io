---
layout: post
title: Building Again
---

I built this site while attending Metis in 2017. The archive abruptly stops a few weeks later.

Nine years later, I’m writing here again.

Data science never entirely disappeared from my life during that time. I did analytical work, helped develop quantitative tools, occasionally worked on projects, and kept thinking about many of the same kinds of problems that interested me when I first learned data science. But for a long time, I wasn’t doing the kind of sustained technical work I had imagined when I created this site.

Over the past year, that has changed.

I started an M.S. in Data Science at the University of Colorado Boulder, but some of the most useful learning has happened outside coursework. I’ve started building things again.

One thing I’ve learned about myself is that I’m much better at learning technical material when there’s a question on the other side of it.

It’s hard for me to get excited about learning a tool simply because it’s a tool I’m supposed to know. Give me a problem I care about, though, and figuring out the tool becomes part of figuring out the problem.

Soccer has been particularly useful for that.

I’ve coached for more than a decade, so there are plenty of things I think I understand intuitively about the game. Tracking data creates an opportunity to ask whether some of those intuitions can actually be measured.

That led to [Moving the Defense](https://github.com/JeremyBetz/moving-the-defense).

The project started with a fairly intuitive question about off-ball movement: when an attacker moves without the ball, what happens to the defenders around them?

That question turned out to be much harder than it sounded.

A defender can move because the entire defensive unit moves. They can move differently from the rest of the unit. Nearby defenders may behave differently from more distant defenders. Relationships that look obvious in one passage of play may disappear across thousands of observations.

And even if attacker movement precedes defensive movement, that doesn’t mean the attacker caused it.

The project gradually became as much about how to ask the question as answering it.

I’ve worked with tracking data from multiple providers, developed ways of separating localized defensive movement from collective translation, tested results on held-out data, replicated findings in other tracking environments, run sensitivity analyses, and spent a lot of time trying to work out exactly what the evidence does and doesn’t permit me to say.

Some ideas worked.

Quite a few didn’t.

That has probably been the most valuable part.

Earlier in my data science education, I tended to think of a failed model or unsupported hypothesis as something standing between me and the result I was trying to find. I’m much more interested now in designing analyses where failure tells me something.

If a result disappears on held-out data, I want to know that.

If a plausible football interpretation doesn’t survive a direct test, I want to keep the negative result.

If changing a reasonable methodological choice changes the conclusion, that’s part of the result too.

Coming back to data science older, I’m less interested in getting a model to produce an impressive answer and more interested in figuring out whether the answer survives an attempt to prove myself wrong.

That research has also generated new questions.

I’m now beginning [Disrupting the Network](https://github.com/JeremyBetz/defensive-network-disruption), a project for PySport’s Analytics Cup 2.0 using SkillCorner tracking data.

This time I’m looking at the other side of the game.

One way of thinking about possession is as a network of potential connections between attacking players. Defenders are simultaneously trying to disrupt those connections while maintaining useful relationships with one another.

That raises a question I’m interested in exploring: what makes an attacking connection viable, and how does defensive positioning weaken it?

There are obvious football concepts nearby — passing lanes, cover shadows, pressure, support, compactness — but putting familiar football terminology on a geometric relationship doesn’t mean you’ve measured the underlying concept.

Right now, the project mostly consists of questions, research scaffolding, and things I explicitly haven’t established yet.

That’s intentional.

Not everything I’m working on needs to turn into a research project.

I’ve also started doing the monthly Kaggle Playground competitions again. I’m deliberately treating those differently. They’re an excuse to practice more conventional tabular machine learning, experiment with models and features, and keep those skills active without spending months trying to extract a research question from every dataset.

That’s useful in its own way.

Moving the Defense has become a large, methodologically careful project, and I expect the Analytics Cup work to require substantial investment as well. Having something where I can build a baseline, try a few ideas, submit a model, and move on gives me a different kind of repetition.

Sometimes a project can just be fun.

Put together, this has started to resemble an informal curriculum.

Graduate coursework gives me formal structure.

The soccer research forces me to think about measurement, statistics, validation, spatial data, research design, and scientific claims.

Kaggle gives me repetitions with predictive modeling and keeps me working with more conventional machine-learning problems.

And each project exposes something I don’t know yet.

I think that’s the part I’ve missed most.

There is an enormous amount of data science I don’t know. There always will be. But that feels considerably less intimidating when learning starts with *I want to understand this* rather than *I should probably learn this technology because it appears in job descriptions*.

So I’m building again.

I don’t know exactly where all of these projects will end up. Some ideas will probably fail. Some projects will change direction. Hopefully a few will turn into something useful.

For now, that’s enough reason to keep going.
