
2025-07-23 23:15

Status: #Finished 

Tags:[[AI]]

# Messages and Special tokens

- AI models does not "remember" your messages. It rereads everything every time.
- When you start a new chat, all of the prompts from **you** and the **model** with their respective `<|start_header_id|>` are stored under `<| begin_of_text |>`
- Before generating a response, the AI model rereads everything stored in the "prompt blob"

### Chat Templates

- Chat templates are used to structure and standardize the conversation between a user and ANY AI model.
- Chat templates define the context and parameters to ensure a smooth continuity of the chat with the user. (How I coded the prompt in my FYP to ensure focus on medical conditions)

### Messages

1. **System Messages:** Also known as "System prompts", these define how a model should behave. Persistent instructions.
	In context of Agents, System Messages also define the role and the available tools that an agent can use to perform its respective tasks
2. **Conversation**: These are the messages/prompts that are exchanged between the user and the AI model

#### References
[[Messages and Special Tokens (Hugging face Course)]]