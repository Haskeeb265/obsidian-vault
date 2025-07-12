
2025-07-11 05:12

Status: #InProgress 

Tags:[[AI]]

# What are LLMs

- An LLM excels at understanding and generating human language.
- LLMs are trained on vast amounts of text data allowing them to learn patterns, structure, and even nuance in language (consists of many millions of parameters)
- Most LLMs nowadays are build on **transformer** architecture based on the **Attention algorithm**. 

___

### Types of Transformers

1. **Encoders**: Takes input from the user and outputs a dense representation of that text. Dense representation = a vector which is for internal understanding where each number in the vector holds a meaning.
2. **Decoders**: Generates new tokens to complete a sequence. One token at a time.
3. **Seq2Seq (Encoder-Decoder)**: A pipeline which uses Encoder with Decoder. This is used to transform an input sequence into an output sequence

LLMs are typically decoder based.

___

### Principles of LLMs

The underlying principle of LLMs is simple yet highly effective:
	"**Its objective is to predict the next token, given a sequence of previous tokens**"

- LLMs works on **tokens** a token is the unit of information for an LLM
- Just like "words" in a language. LLMs language is **Tokens**.\

- Each LLMs have some **special tokens**.
- LLMs use special tokens to open and close the structured components of its generation. (For example to indicate start and end of a sequence or message)
- One of the examples of special tokens is End of Sequence(**EOS**)

___

### Understanding Next Token Prediction

- LLMs are **autoregressive** = Output of one layer is input for next layer.
- The autoregressive state continues until the model predicts that the next token is the **EOS**. Once the EOS token is predicted, the model can stop.

#### Single Decoding Loop:

1. The input text is tokenized
2. Model computes the representation of the sequence 
3. The representation sequence captures information about the meaning and the position of each token in the input sequence.
4. Representation goes into the model which then outputs scores that rank the likelihood of each token in it's vocabulary.
5. Based on the scores, we have multiple strategies to select the tokens to complete the sentence
	1. The easiest strategy is always picking the token with the highest score

___

### Attention is All You Need:

- One of the key aspects of Transformer architecture is **Attention**.
- In a user prompt, not every word holds the same importance.
- In the sentence, **The capital of Pakistan is**, **capital** and **Pakistan** holds the most meaning; Subtly indicating towards the context of the original prompt.
- The process is identifying the most relevant words to produce the next token.
- One of the features that LLMs are being pushed towards is higher and higher **context length** which would allow the LLMs to find **attention words** in longer sequences of tokens/words 

___

### Prompting the LLM:

- Basically, LLMs predict the next token by looking at all of the input tokens and deciding which of those tokens are most important, our prompts matter very much
- For better results give a prompt wh






#### References
