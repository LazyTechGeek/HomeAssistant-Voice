# 🔊 Part 1 - Home Assistant Voice PE Step-By-Step Guide

In this video, I walk you through setting up the Home Assistant Voice PE device from start to finish — adding devices, exploring the menus, using templates, creating automations, and even a demo with LED control.

▶️ [Watch part 1 here](https://youtu.be/nS5a4xbTdxA)  

### 💡 LED Automation files used in this video

- **[Basic LED Automation](https://github.com/LazyTechGeek/HomeAssistant-Voice/blob/main/Basic_LED_Automation.yaml)**
- **[KITT LED Automation](https://github.com/LazyTechGeek/HomeAssistant-Voice/blob/main/KITT_LED_Automation.yaml)**

### 🌡️ Template used for weather with temperature:

- **[Weather with Temperature](https://github.com/LazyTechGeek/HomeAssistant-Voice/blob/main/weather-temperature.yaml)**

# 🔊 Part 2 – Home Assistant Voice + OpenAI Conversation Integration

In Part 2, we install and configure the OpenAI Conversation integration in Home Assistant Voice to create a smarter, more natural assistant. This includes creating an API key, adding it to Home Assistant, setting up a Conversation Agent, and assigning a personality with custom prompts.

▶️ [Watch part 2 here](https://youtu.be/wFsG-9-7JJQ)

### Prompt Examples
---
- **[Rogue AI Prompt](https://github.com/LazyTechGeek/HomeAssistant-Voice/blob/main/rogue_ai_prompt.txt)**
- **[KITT AI Prompt](https://github.com/LazyTechGeek/HomeAssistant-Voice/blob/main/KITT_ai_prompt.txt)**

---

### OpenAI Models & Rate Limits (as of September 2025)

<details>
<summary><strong>Model rate limits (Tier 1)</strong></summary>

| Family       | Model                      | TPM       | RPM  | RPD   | TPD       | Notes              |
|--------------|----------------------------|----------:|-----:|------:|----------:|--------------------|
| Chat         | gpt-3.5-turbo              | 200,000   | 500  | 10,000 | 2,000,000 |                    |
| Chat         | gpt-3.5-turbo-instruct     | 90,000    | 3,500| —     | 200,000   |                    |
| Chat         | gpt-4                      | 10,000    | 500  | 10,000 | 100,000   |                    |
| Chat         | gpt-4-turbo (shared)       | 30,000    | 500  | —     | 90,000    | includes preview models |
| Chat         | gpt-4.1 (shared)           | 30,000    | 500  | —     | 900,000   |                    |
| Chat         | gpt-4.1 (long context)     | 200,000   | 100  | —     | 2,000,000 |                    |
| Chat         | gpt-4.1-mini (shared)      | 200,000   | 500  | —     | 2,000,000 |                    |
| Chat         | gpt-4.1-mini (long context)| 400,000   | 200  | —     | 4,000,000 |                    |
| Chat         | gpt-4.1-nano (shared)      | 200,000   | 500  | —     | 2,000,000 |                    |
| Chat         | gpt-4.1-nano (long context)| 400,000   | 200  | —     | 4,000,000 |                    |
| Chat         | gpt-4o (shared)            | 30,000    | 500  | —     | 90,000    | includes audio previews |
| Chat         | gpt-4o-audio-preview-2025-06-03 | 250,000 | 3,000| —     | —         |                    |
| Chat         | gpt-4o-mini (shared)       | 200,000   | 500  | 10,000 | 2,000,000 | includes audio/search |
| Chat         | gpt-4o-mini-search-preview | 6,000     | 100  | —     | —         |                    |
| Chat         | gpt-4o-mini-transcribe     | 50,000    | 500  | —     | —         |                    |
| Chat         | gpt-4o-search-preview      | 6,000     | 100  | —     | —         |                    |
| Chat         | gpt-4o-transcribe          | 10,000    | 500  | —     | —         |                    |
| Chat         | gpt-5 (shared)             | 30,000    | 500  | —     | 900,000   | includes latest/preview |
| Chat         | gpt-5-mini                 | 200,000   | 500  | —     | 2,000,000 |                    |
| Chat         | gpt-5-nano                 | 200,000   | 500  | —     | 2,000,000 |                    |
| Chat         | gpt-audio                  | 250,000   | 3,000| —     | —         | includes preview   |
| Chat         | gpt-realtime               | 250,000   | 3,000| —     | —         | includes preview   |
| Text         | babbage-002                | 250,000   | 3,000| —     | —         |                    |
| Text         | davinci-002                | 250,000   | 3,000| —     | —         |                    |
| Text         | chatgpt-4o-latest          | 500,000   | 200  | —     | —         |                    |
| Text         | codex-mini-latest          | 200,000   | 500  | —     | 2,000,000 |                    |
| Text         | o1                         | 30,000    | 500  | —     | 90,000    | includes variants  |
| Text         | o1-mini                    | 200,000   | 500  | —     | 2,000,000 | includes variants  |
| Text         | o1-pro (shared)            | 30,000    | 500  | —     | 90,000    |                    |
| Text         | o3 (shared)                | 30,000    | 500  | —     | 90,000    |                    |
| Text         | o3-mini (shared)           | 200,000   | 500  | —     | 2,000,000 |                    |
| Text         | o4-mini (shared)           | 200,000   | 500  | —     | 2,000,000 | includes deep-research |
| Text         | text-embedding-3-large     | 1,000,000 | 3,000| —     | 3,000,000 |                    |
| Text         | text-embedding-3-small     | 1,000,000 | 3,000| —     | 3,000,000 |                    |
| Text         | text-embedding-ada-002     | 1,000,000 | 3,000| —     | 3,000,000 |                    |
| Realtime     | gpt-4o-mini-realtime-preview| 40,000   | 200  | 1,000 | —         | shared limits      |
| Realtime     | gpt-4o-realtime-preview    | 40,000    | 200  | 1,000 | —         | shared limits      |
| Moderation   | omni-moderation-latest     | 10,000    | 500  | 10,000| —         |                    |
| Moderation   | text-moderation-latest     | 150,000   | 1,000| —     | —         |                    |
| Moderation   | text-moderation-stable     | 150,000   | 1,000| —     | —         |                    |
| Image        | dall-e-2                   | —         | 500  | —     | —         | 5 images/min       |
| Image        | dall-e-3                   | —         | 500  | —     | —         | 5 images/min       |
| Image        | gpt-image-1                | 100,000   | 500  | —     | —         | 5 images/min       |
| Audio        | gpt-4o-mini-tts            | 50,000    | 500  | —     | —         |                    |
| Audio        | tts-1                      | —         | 500  | —     | —         | includes variants  |
| Audio        | whisper-1                  | —         | 500  | —     | —         |                    |
| Fine-tune Inference | babbage-002 (FT)    | 250,000   | 3,000| —     | —         | shares base limits |
| Fine-tune Inference | davinci-002 (FT)    | 250,000   | 3,000| —     | —         | shares base limits |
| Fine-tune Inference | gpt-3.5-turbo-0125 (FT) | 200,000 | 500  | —     | —         | shares base limits |
| Fine-tune Inference | gpt-4-0613 (FT)     | 10,000    | 500  | —     | —         | shares base limits |
| Other        | Default (others)           | 250,000   | 3,000| —     | —         | catch-all default  |

</details>
