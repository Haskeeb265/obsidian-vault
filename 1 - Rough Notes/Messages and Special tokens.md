
2025-07-23 23:15

Status: #InProgress 

Tags:[[AI]]

# Messages and Special tokens

- AI models does not "remember" your messages. It rereads everything every time.
- When you start a new chat, all of the prompts from **you** and the **model** with their respective `<|start_header_id|>` are stored under `<| begin_of_text |>`
- Before generating a response, the AI model rereads everything stored in the "prompt blob"

### Chat Templates

- Chat templates are used to structure and standardize the conversation between a user and ANY AI model.
- Chat templates define the context and parameters to ensure a smooth continuity of the chat with the user. (How I coded the prompt in my FYP to ensure focus on medical conditions)
- 




#### References
[[Messages and Special Tokens (Hugging face Course)]]