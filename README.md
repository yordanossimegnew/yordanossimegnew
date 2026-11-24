### Hi, I'm Yordanos 👋

AI engineer in Addis Ababa, Ethiopia · open to AI engineering roles · [LinkedIn](https://www.linkedin.com/in/yordanos-muche)

I build LLM applications end to end:
- **Agents** that use tools and pause for human approval.
- **RAG** that answers with verified citations.
- **Evaluation pipelines** that catch a prompt or retrieval regression before it ships.
- **The backend around them:** durable job queues, a multi-provider gateway, PostgreSQL / pgvector.

Every project below is a complete, runnable app: a FastAPI backend, a Streamlit UI, automated
tests and a demo GIF in the README.

**Stack:** Python · LangGraph · LangChain · Claude API · FastAPI · PostgreSQL / pgvector · Streamlit · Docker · pytest

#### Production LLM infrastructure
- **[durable_agent_jobs](https://github.com/yordanossimegnew/durable_agent_jobs)**: crash-proof agent jobs on PostgreSQL: leased workers, checkpoint resume, retries and human approval. Kill a worker mid-job and another one picks it up.
- **[llm-gateway](https://github.com/yordanossimegnew/llm-gateway)**: one OpenAI-compatible endpoint over Anthropic, OpenAI-compatible servers and Ollama, with fallback chains, circuit breakers, 429 cooldowns, budgets per key and a full request log.

#### Evals and RAG
- **[prompt-regression-tester](https://github.com/yordanossimegnew/prompt-regression-tester)**: prompts versioned in git, checks plus a calibrated LLM judge, significance-tested verdicts that fail CI.
- **[retrieval-eval-lab](https://github.com/yordanossimegnew/retrieval-eval-lab)**: benchmarks retrieval choices (vector, keyword, hybrid, chunking, reranking, HyDE) on synthetic and SciFact questions.
- **[rag-freshness-pipeline](https://github.com/yordanossimegnew/rag-freshness-pipeline)**: keeps a RAG index in sync with changing websites: 304s, chunk-level re-embedding, staleness SLAs and alerts.
- **[document-qa-citations](https://github.com/yordanossimegnew/document-qa-citations)**: document Q&A with hybrid search and page-level citations verified against the source.

#### Agents
[coding_agent](https://github.com/yordanossimegnew/coding_agent) ·
[browser_agent](https://github.com/yordanossimegnew/browser_agent) ·
[streaming_agent_shell](https://github.com/yordanossimegnew/streaming_agent_shell) ·
[multi_agent_code_review](https://github.com/yordanossimegnew/multi_agent_code_review) ·
[local-model-eval-harness](https://github.com/yordanossimegnew/local-model-eval-harness)

Earlier work: classical ML and deep learning, including BERT fine-tuning, LSTM sentiment analysis,
mammography classification and recommender systems.
