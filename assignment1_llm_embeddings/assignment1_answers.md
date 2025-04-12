# Assignment 1: Thinking Critically - Answers

## 1. Evolution of Embeddings
- TF-IDF only counted words, so it couldn't understand that "car" and "automobile" mean the same thing. Word2Vec fixed this by learning word meanings from context.
- LSTMs struggled with long sentences. Transformers fixed this by letting the model look at all words at once, no matter how far apart they are.

## 2. BERT's Contribution
BERT could learn from both directions (before and after a word) at once. Earlier models only looked in one direction, which limited their understanding of context.

## 3. BERT vs. Ada (OpenAI) Comparison
BERT (Local):
- Free to use
- Data stays private
- Needs setup and good hardware
- Can be customized

Ada (OpenAI):
- Pay per use
- Sends data to cloud
- Super easy to use
- No setup needed
- Can't be customized

## 4. Chunking Scenario
- Needed because models can only handle short pieces of text (like 512 tokens)
- Two strategies:
  1. Split by paragraphs (simple but effective)
  2. Split by fixed size (like 500 tokens) with some overlap
- Choose size based on: model limits, type of content, and how specific you need the answers to be

## 5. Model Selection
- Startup FAQ chatbot → Use OpenAI Ada (quick to set up, no maintenance)
- Hospital patient records → Use BERT locally (keeps sensitive data private)
- Personal note app → Use BERT locally (free, runs on your PC, no ongoing costs)
