# CAIMPS: Canonical AI Model and Provider Naming System

CAIMPS is a framework designed to standardize the naming conventions of AI models and their providers. Inspired by existing standards like DNS, OpenRouter, and blockchain naming systems, CAIMPS ensures that AI models are unique, easily discoverable, and structured for interoperability across different platforms.

## Goals
- **Uniqueness**: Guarantee unique names for every registered AI model.
- **Interoperability**: Facilitate easy interaction across various AI service providers.
- **Discoverability**: Provide a clear system for users to find and identify AI models and their versions.

## Structure
CAIMPS follows a hierarchical structure:

```
[provider/model[:extension][@hosting]]
```

- **Provider**: The entity providing the model.
- **Model**: The name of the model.
- **Extension (optional)**: Additional tags or variations of the model (e.g., beta, free, extended).
- **Hosting (optional)**: The platform or repository where the model is hosted (e.g., `huggingface`, `replicate`, `openrouter`).

### **Examples**:
- `openai/gpt-4`
- `google/flan-t5@huggingface`
- `mistralai/pixtral-12b:free@replicate`
- `cohere/command-r:beta@openrouter`

## Models with CAIMPS Naming

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
