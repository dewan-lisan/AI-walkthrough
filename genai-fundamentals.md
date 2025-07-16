# Generative AI Core Concepts

### Goals
- Deep technical understanding of LLMs for AI enthusiasts, engineers, and data scientists
- Explore the power of LLMs as a general-purpose technology
- The generative AI project lifecycle, including model training, instruction tuning, fine-tuning, and deployment

## Generative AI Project Lifecycle
#### Key Decisions:
- **Model Selection:** Choose between off-the-shelf foundation models or pre-training custom models.
- **Fine-Tuning:** Customize models for specific datasets or tasks.
- **Model Sizing:** Evaluate trade-offs between large models (100B+ parameters) for general knowledge vs. smaller models (1B or less) for specific tasks (e.g., dialogue summarization, customer service).

#### Use Case Considerations:
- **Large Models:** Ideal for broad tasks requiring general knowledge (e.g., history, philosophy, coding).
- **Small Models:** Effective for single-task applications with comparable or optimized results.

**#todo:** extend this section with sepcific example model names

## Prompt Engineering
Interaction with LLMs uses natural language prompts (text instructions) rather than formal code.
- **Context Window:** The model’s memory for processing prompts, typically holding a few thousand words (varies by model).
- **Prompt:** Input text (e.g., a question like “Where is Ganymede?”).
- **Completion:** The model’s output, including the prompt and generated text (e.g., “Ganymede is a moon of Jupiter…”).
- **Inference:** The process of generating text from a prompt.
