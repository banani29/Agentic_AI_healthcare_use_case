# Agentic_AI_healthcare_use_case

In this simulation, we operationalized the core logic of two clinical agents—Patient Check-In Agent and SOAP Compiler Agent - using a controlled data setup and modular execution pipeline. Following steps were implemented:

1. Simulated Clinical Dataset Construction

2. Defined a set of interconnected functions that mirror a production-grade agentic architecture:
2.1 supervisor_agent(intent, payload) - Decodes user intent and delegates to specific agents.
2.2 code_interpreter(data) - Performs preprocessing (e.g., cleaning transcripts or queue events).
2.3 query_knowledge_base(query_text) - Simulates semantic search using OpenSearch-like indexing.
2.4 action_group_execute(model_type, input) - Orchestrates different model calls (e.g., LSTM, XGBoost, ClinicalBERT).
2.5 update_memory(patient_id, key, value, memory_type) - Writes session data into simulated memory layers.

3. Agent Logic Implementation : Two primary agents were implemented.
3.1 patient_checkin_agent
3.2 soap_compiler_agent

4. Above functions were called and output was retrieved
5. Implemented feedback loop for continual learning

