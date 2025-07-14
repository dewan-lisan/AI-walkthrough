# Natural Language Processing (NLP)

### Syntax and Semantics
**Syntax:** Rules for structuring language (e.g., valid sentence: "Sherlock Holmes stepped briskly into the room" vs. invalid: "Sherlock Holmes nine o’clock stepped briskly the room").  

**Semantics:** Meaning of sentences (e.g., "Just before nine o’clock Sherlock Holmes stepped briskly into the room" and "A few minutes before nine, Sherlock Holmes walked quickly into the room" have similar meanings).

"Colorless green ideas sleep furiously" is syntactically valid but semantically meaningless.

### Rule-Based NLP: Context-Free Grammar (CFG)
A system of rules for generating valid sentences using terminal (words) and nonterminal symbols (e.g., N for noun, V for verb).

**Example:**  
- Sentence: NP (Noun Phrase) + VP (Verb Phrase).
- NP → N | D N (e.g., "she" or "the city").
- VP → V | V NP (e.g., "walked" or "saw the city").

**Implementation:** Use NLTK (Natural Language Toolkit) to parse sentences and generate syntax trees (e.g., cfg0.py for "she walked" or "she saw the city").  

**Limitations:** Writing rules for all possible sentences is complex and labor-intensive.
