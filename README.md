# AI Card Splitter

Long “wall-of-text” answers are hard to review. This add-on uses an AI model to split one long Anki card into multiple shorter Q&A cards while keeping your original note intact.

## Features
- Use AI to split long answers into multiple digestible Q&A cards.
- Keeps the original note unchanged and optionally creates new notes/cards.
- Configurable splitting strategy and card templates.
- Works in batch mode from the Browser.

## Requirements
- Anki 2.1+
- Optional AI provider (OpenAI/Gemini) for intelligent splitting. A heuristic local fallback may be available.

## Installation
1. Clone or download the repository.
2. Place the add-on folder into the Anki add-ons directory.
3. Restart Anki.

## Usage
- Select notes in the Browser that have long answers.
- Run “AI Split Selected Notes”.
- Review suggested splits and adjust if necessary, then confirm to create new cards.

## Configuration
- Choose provider and credentials (if using AI).
- Set maximum card length, minimum context overlap, and templates for generated cards.
- Option to auto-apply splits or require manual confirmation.

Example config:
```json
{
  "provider": "openai",
  "max_tokens_per_card": 150,
  "confirm_before_create": true
}
```

## Privacy & Best Practices
- Review generated cards for correctness and completeness — AI can make mistakes.
- Avoid sending sensitive information to cloud providers unless permitted.

## Troubleshooting
- If splitting fails, check API key, network connectivity, and Anki console logs.
- For odd splits, adjust the prompt or splitting parameters.

## Development
- Contributions welcome. Provide test cases and sample notes when opening an issue.

## License
MIT License — see LICENSE file.

## Contact
Author: yuwayanagitani
