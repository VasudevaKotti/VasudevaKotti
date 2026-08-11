# Vasudeva Kotti

I architect production AI systems — and I build them with AI. Models write much of
the code under my direction, and I answer for every line of it.

Twenty-eight years of building software for institutions that cannot afford to be wrong:
eleven years of banking infrastructure as a Vice President at J.P. Morgan, enterprise
cloud at SAP Labs after that, Oracle and PeopleSoft before, and PowerBuilder against
Sybase back when that was a reasonable sentence.

For the past two years I have been the architect of an
**air-gapped, bilingual (Arabic/English) AI platform for a government water ministry** —
no internet, no cloud APIs, no data leaving the building — delivered through
AI-augmented engineering: models wrote a substantial share of the code, under an
architecture, a review discipline, and build-failing quality gates that I own. Grounded document Q&A over a
retrieval index, natural-language dashboard generation executed inside a resource-governed
sandbox, a hydrological forecasting engine where ten model families compete against
trivial baselines, and a water-security digital twin that turns a minister's what-if
question into a mass-balance simulation. A quarter of a million lines of Python behind a
React front end, 27 API routers, more than 1,300 tests, and every interface string
mirrored in English and Arabic — 2,012 of each.

The platform itself is client work and stays private. The architecture decisions are
mine to share, and they are public here:

**[sovereign-llm-architecture](https://github.com/VasudevaKotti/sovereign-llm-architecture)** —
field notes on building LLM systems where the network cable does not exist.

## What I have come to care about

A few principles, learned in production rather than adopted from talks:

- Exactly one module in the application core may call a model. An architecture test fails the build if a second one tries.
- AI interprets and narrates; every number comes from a deterministic engine. Trust is an architecture property.
- Bilingual is not a translation task. If Arabic is not first-class in the embeddings, the gates, and the tests, it is not in the product.
- A model's output is a claim, not a result. Parse strictly, repair deliberately, and record where every figure came from.
- An honest dashboard tells you what it left out.

## Elsewhere

I write regularly about building AI under constraint on
[LinkedIn](https://www.linkedin.com/in/vasudeva-kotti/), one essay a week — model
screening gates, structured-output contracts, the economics of air-gapped inference,
and why the simple model keeps winning.

Reachable at vasudevakotti@gmail.com.
