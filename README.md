# compare-models

Ask the same question to multiple LLM models side by side and rate their answers, using [promptfoo](https://github.com/promptfoo/promptfoo).

## Setup on Mac

1. Install promptfoo: `brew install promptfoo`
2. Create a `.env` file in this folder with your API key:
   ```
   OPENAI_API_KEY=sk-proj-...
   ANTHROPIC_API_KEY=sk-ant-...
   ```
   Make sure `.env` is gitignored to never commit your keys.

## Usage

```
promptfoo eval                                   # ask the question to all models
promptfoo view                                   # rate and comment in the browser
promptfoo export eval latest -o raw_export.json  # save everything to JSON
```

Edit the question and models in `promptfooconfig.yaml`.
