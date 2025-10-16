# Simple-NLP-PII-detector
To build a lightweight PII detection system for ServiceNow ticket data using traditional NLP techniques (tokenization, pattern matching, and rule-based entity recognition).
The goal is to automatically flag any PII (Personally Identifiable Information) such as:

Email IDs
Phone numbers
Names
Policy or account numbers
Addresses or ID-like patterns

2. Approach

The system uses a hybrid of regex + NLP-based entity extraction.
It does not rely on deep learning or transformer models — instead, it uses classical NLP tools like spaCy, regex, and keyword heuristics.

Steps:

Data Input: Random ticket data (from ServiceNow export or mock JSON).

Preprocessing: Clean and normalize text (remove special symbols, lowercase).

Regex Matching: Detect structured patterns (emails, phone numbers, policy numbers).

NER with spaCy: Detect person names, organizations, locations, etc.

Scoring: Assign a “PII risk level” to each ticket.

Output: Display detected entities and flag high-risk tickets.
