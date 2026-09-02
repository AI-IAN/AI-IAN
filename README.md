# Hi, I'm Ian

I design, operate, and debug agent systems on my own hardware. I build with AI and
I'm not shy about it: the architecture, the instrumentation, and the debugging when
things break at 2am are mine. Most of what's here exists because something failed
and I instrumented my way to the cause.

The recurring lesson, and the thing I'm actually good at, is that the instrument is
usually the bug. A monitor that reports success it hasn't earned is worse than no
monitor, and finding those takes checking the report against the source rather than
reading the code and nodding.

## What I run

A two-machine fleet (Mac plus an RTX 5090 Windows box) on self-hosted vLLM: 29
services and 22 scheduled agents, with 61 agents tracked for liveness by real
output rather than by exit code. 1.33B prompt tokens and 862 GPU-hours have gone
through an inference proxy I wrote to capture every call, and 29,523 runs have been
classified by an eval layer I built after my first evals measured the wrong unit
and called a 59%-duplicate pipeline healthy.

## What to look at

- **[shh-paste](https://github.com/AI-IAN/shh-paste)**: local voice transcription
  for macOS. On-device Whisper large-v3-turbo, no cloud, no subscription, my daily
  driver for five months. Available now.
- **[FabricSemanticToolkit](https://github.com/AI-IAN/FabricSemanticToolkit)**: a
  Python CLI that audits DAX measures and semantic models. From consulting work,
  sanitized. Available now.
- **Price observatory**: 374,749 observations and growing, collected daily from four
  public ticketing sites. One adapter per site, a normalized schema that reconciles
  products named and structured differently on every one, and a validation oracle
  that quarantines a run unless coverage, level, and row count all pass. Writeup
  coming.
- **Agent-fleet observability**: the capture proxy, liveness-by-real-output fleet
  monitoring, and incident-driven alerting, extracted from the system above. Coming.

## Background

Nine years as a data and analytics consultant: solo, end-to-end delivery, from
stakeholder conversation to shipped system. Currently architecting a marketing
revenue platform on Microsoft Fabric for a NYC REIT.

