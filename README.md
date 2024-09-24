# CAIMPS: Canonical AI Model and Provider Naming System

![Carbon code (18)](https://github.com/user-attachments/assets/0a57ac1c-0a14-4bd7-b619-a01e1bdf10cf)

CAIMPS stands for Canonical AI Model and Provider Naming System. It's a framework designed to standardize how we name AI models and their providers, making it easier for everyone to find, use, and integrate these models across different platforms. Inspired by systems like DNS (Domain Name System), OpenRouter, and blockchain naming conventions, CAIMPS ensures that every AI model has a unique and easily discoverable name.

As the AI ecosystem grows, so does the number of models and providers. This can make it challenging to keep track of different models, especially when they have similar names or versions.

## How Does It Work?

CAIMPS uses a simple, hierarchical naming structure:

```
[provider/model[:extension][@hosting]]
```

Let's break down each component:

- **Provider**: The organization or individual offering the model (e.g., `openai`, `google`).
- **Model**: The specific name of the AI model (e.g., `gpt-4`, `gemini-pro`).
- **Extension (optional)**: Additional tags or variations of the model, such as beta versions or free editions (e.g., `:beta`, `:free`).
- **Hosting (optional)**: The platform or repository where the model is hosted (e.g., `@huggingface`, `@replicate`).

### Examples

- **`openai/gpt-4`**: The GPT-4 model provided by OpenAI.
- **`google/flan-t5@huggingface`**: Google's Flan-T5 model hosted on Hugging Face.
- **`mistralai/pixtral-12b:free@replicate`**: Mistral AI's Pixtral 12B free version hosted on Replicate.
- **`cohere/command-r:beta@openrouter`**: Cohere's Command R beta version available via OpenRouter.


## CAIMPS Naming in Practice

| Model Name                           | Provider                      | CAIMPS Name                                  |
| ------------------------------------ | ----------------------------- | -------------------------------------------- |
| Nous: Llama 3.1 8B Instruct          | nousresearch                  | nousresearch/llama-3.1-8b-instruct           |
| Qwen2.5 72B Instruct                 | qwen                          | qwen/qwen-2.5-72b-instruct                   |
| Qwen2-VL 72B Instruct                | qwen                          | qwen/qwen-2-vl-72b-instruct                  |
| Lumimaid v0.2 8B                     | neversleep                    | neversleep/llama-3.1-lumimaid-8b@replicate   |
| OpenAI: o1-mini                      | openai                        | openai/o1-mini                               |
| OpenAI: o1-preview                   | openai                        | openai/o1-preview                            |
| Mistral: Pixtral 12B (free)          | mistralai                     | mistralai/pixtral-12b:free@huggingface       |
| Mistral: Pixtral 12B                 | mistralai                     | mistralai/pixtral-12b                        |
| Cohere: Command R                    | cohere                        | cohere/command-r                             |
| Cohere: Command R+                   | cohere                        | cohere/command-r-plus                        |
| Google: Gemini Flash 8B 1.5 Exp.     | google                        | google/gemini-flash-8b-1.5-exp@huggingface   |
| AI21: Jamba 1.5 Large                | ai21                          | ai21/jamba-1.5-large                         |
| AI21: Jamba 1.5 Mini                 | ai21                          | ai21/jamba-1.5-mini                          |
| Phi-3.5 Mini 128K Instruct           | microsoft                     | microsoft/phi-3.5-mini-128k-instruct         |
| Nous: Hermes 3 70B Instruct          | nousresearch                  | nousresearch/hermes-3-llama-3.1-70b          |
| Nous: Hermes 3 405B Instruct (free)  | nousresearch                  | nousresearch/hermes-3-llama-3.1-405b:free    |
| OpenAI: ChatGPT-4o                   | openai                        | openai/chatgpt-4o                            |
| Google: Gemini Pro Vision 1.0        | google                        | google/gemini-pro-vision                     |
| OpenAI: GPT-4 Vision Preview         | openai                        | openai/gpt-4-vision-preview                  |
| Mistral: Mistral 7B Instruct         | mistralai                     | mistralai/mistral-7b-instruct                |



## Contributing
See the [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on how to contribute.

## License
This repository is licensed under the MIT License. See [LICENSE](LICENSE) for more information.
