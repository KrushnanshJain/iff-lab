# Iff Lab

Iff Lab is an early-stage project exploring an **AI study assistant for engineering students**. The idea is simple: a student uploads their own lecture notes, and the assistant answers questions grounded in those notes instead of giving generic answers.

## Status

**Idea / pre-product stage.** This is a solo, bootstrapped project started in October 2026. There is no live product, no users and no funding yet. This repository holds early experiments and planning.

## The problem

Engineering students collect large amounts of notes, slides and problem sets across many courses. Revising from them is slow:

- Finding where a concept was explained takes time.
- Generic chatbots don't know what a specific professor taught or which notation the course uses.
- Answers that aren't tied to the student's material are hard to trust or verify.

## What I'm exploring

A note-based question-and-answer assistant:

1. Student adds their course notes (text or PDF).
2. Notes are split into chunks and indexed for search.
3. When the student asks a question, the most relevant chunks are retrieved.
4. A language model answers using only those chunks and points back to where in the notes the answer came from.

## Planned approach

- **Model access:** [Amazon Bedrock](https://aws.amazon.com/bedrock/) for the language model and embeddings
- **Pattern:** retrieval-augmented generation (RAG) over user-provided notes
- **Prototype scope:** a small command-line or web demo that answers questions from a handful of sample notes

The stack may change as the experiments teach me what works.

## Roadmap

- [ ] Write down the target user and core use cases
- [ ] Prototype note ingestion and chunking
- [ ] Prototype retrieval and grounded answers on Amazon Bedrock
- [ ] Add source references to answers
- [ ] Test with a few real engineering course notes
- [ ] Collect feedback from other students

## Repository layout

This will grow as the project does. For now the repository contains this README and early notes.

## About

Built by [Krushnansh Jain](https://github.com/KrushnanshJain), a student exploring this idea on his own.

Feedback and ideas are welcome. Please open an issue.

## License

To be decided.
