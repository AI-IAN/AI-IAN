# Ian Jacobs

Nine years taking enterprise data platforms from requirements to production, working
directly with the people who own the data. Now doing the same with agent systems, where
the hard part is not building them but making their output trustworthy: run-level scoring,
deterministic checks, and a human gate before anything writes.

## Systems I designed and operate

**Life OS**: the operations system I run my work on, in daily use. Scheduled agents produce
briefings, research, monitoring and drafts. Most of the engineering is the part that keeps
them honest, and I built it because the early versions were not: runs scored and classified
by an LLM judge, deterministic checks the model cannot talk its way past, calls attributed
and costed, and nothing reaching the system of record without me approving it. It runs on a
self-hosted inference stack, vLLM serving quantized Qwen on an RTX 5090, so private data
never leaves the network and cost is fixed rather than metered.

**Price tracking pipeline**: over 370,000 observations and growing, collected daily across
four public sources. One adapter per site, a normalized schema that reconciles products
named and structured differently on every one, and a validation oracle that quarantines a
run unless coverage, level and row count all pass. Analysis dashboard on top.

**[shh-paste](https://github.com/AI-IAN/shh-paste)**: open-source on-device transcription
running Whisper large-v3-turbo on a MacBook Air, no GPU and no cloud, my daily driver for
five months.

**[FabricSemanticToolkit](https://github.com/AI-IAN/FabricSemanticToolkit)**: a Python CLI
that audits semantic models: parses model metadata, maps measure dependencies and lineage,
and flags consolidation candidates as the model grows. From consulting work.

## Background

Across nine years and 20+ engagements I've owned the full analytics stack end to end. That
means gathering requirements directly from the business, designing and building the data
warehouse and ETL, building the reporting layer on top, and presenting the results to
stakeholders myself. Most recently on Microsoft Fabric.
