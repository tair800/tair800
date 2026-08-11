# Tahir Aslanli

**AI automation engineer.** I build workflows that take a real business process end to end — Python and n8n on top of LLM APIs, RAG and internal REST services — and then keep them running in production. Currently at PASHA Insurance; before that, backend services and REST APIs for enterprise banking at Kapital Bank.

Based in Rome (CET). Working remotely.

---

### What I actually do

At PASHA Insurance I own six end-to-end automation workflows connecting seven internal systems and APIs — internal REST services, an enterprise AI gateway, LLM endpoints, Dataiku, SQL Server and PostgreSQL. Where no usable interface existed, I wrote the REST service myself.

The interesting half of that work isn't the model, it's everything around it:

- **Structured output under a schema**, so downstream code can rely on the shape
- **Guardrails, fallbacks, retries with backoff** — because these workflows touch claims and operations data
- **RAG** with chunking, embeddings and metadata-filtered vector search, so retrieval narrows *before* similarity ranking
- **An internal MCP server** over one of our systems. The protocol turned out to be the easy part; the real question is where the trust boundary sits once a model can call a live operation.
- **Human-in-the-loop routing** for the cases the pipeline shouldn't decide alone

My honest view of LLMs after building on them: the model is the cheap part. Almost all of the engineering is validation, failure handling, and knowing when *not* to use it.

That work is closed source, so what's public here is my own projects and study work.

---

### Stack

**Daily:** Python · C# / .NET · ASP.NET Core Web API · REST API design · n8n · PostgreSQL · SQL Server · Git · Docker
**Python:** FastAPI · Django · Requests · HTTPX · Pydantic · Pandas · pytest · asyncio
**AI:** LLM APIs (OpenAI-compatible) · RAG · embeddings · vector search · MCP · prompt engineering · structured outputs
**Front end:** React · TypeScript · JavaScript · Tailwind

**Learning / not yet production for me:** Kubernetes · AWS and cloud-native patterns · Kafka. I'd rather list these here than imply otherwise.

---

### Projects worth your time

**[cv-screening-pipeline](https://github.com/tair800/cv-screening-pipeline)** — Python
A CV screening pipeline built so its decisions can survive an audit. LLM extraction with schema validation and evidence checks, scoring kept deterministic in code rather than delegated to a model, bias parity testing over matched pairs, and an append-only audit trail of human overrides. Synthetic data only. The README documents what broke and what the limitations still are — including that six matched pairs is not enough to claim generalisable fairness.

**[Hospital](https://github.com/tair800/Hospital)** · live at [ahpbca.webonly.io](https://ahpbca.webonly.io)
Hospital management system delivered solo: reference data, record statuses, role-based access, and an admin panel meant for non-technical staff.

**[webonly](https://github.com/tair800/webonly)** · live at [softechweb.webonly.io](https://softechweb.webonly.io)
Client e-commerce platform, end to end — database schema, REST API, React front end, deployment.

**[YoutubeApi-OnionCQRS](https://github.com/tair800/YoutubeApi-OnionCQRS)** — C#
Onion architecture with CQRS over a .NET API. Study project, kept because the layering is clean.

**[microservices-dotnet8](https://github.com/tair800/microservices-dotnet8)** — C#
A .NET 8 microservices reference build — Ocelot gateway, three services, an event consumer, Redis cache-aside, Docker Compose. **This is a learning project, not production experience**: I put it together to work through the patterns, and I don't claim Kafka or Redis in production on my CV.

---

### Languages

Azerbaijani (native) · Russian (C2) · English (C1, IELTS 7.0) · Spanish (C1) · Italian (B1)

My first degree is Spanish Philology — which is why multilingual document and text processing has never been the hard part of any of this.

---

### Reach me

[LinkedIn](https://www.linkedin.com/in/tahir-aslanli-075b4924b) · tair.aslanli800@gmail.com · Telegram [@tairrr8](https://t.me/tairrr8)
