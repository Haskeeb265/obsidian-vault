
2025-07-11 05:12

Status: #InProgress 

Tags:[[AI]]

# What are LLMs

- An LLM excels at understanding and generating human language.
- LLMs are trained on vast amounts of text data allowing them to learn patterns, structure, and even nuance in language (consists of many millions of parameters)
- Most LLMs nowadays are build on **transformer** architecture based on the **Attention algorithm**. 

___

### TYPES OF TRANSFORMERS:

1. **Encoders**: Takes input from the user and outputs a dense representation of that text. Dense representation = a vector which is for internal understanding where each number in the vector holds a meaning.
2. **Decoders**: Generates new tokens to complete a sequence. One token at a time.
3. **Seq2Seq (Encoder-Decoder)**: A pipeline which uses Encoder with Decoder. This is used to transform an input sequence into an output sequence

LLMs are typically decoder based.

___

### PRINCIPLE OF LLMs

The underlying principle of LLMs is simple yet highly effective:
	"**Its objective is to predict the next token, given a sequence of previous tokens**"

- LLMs works on **tokens** a token is the unit of information for an LLM



#### References
