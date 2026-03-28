# Step 2: Create the Campus Resources Agent

This is your second specialist agent. It answers questions about food, counseling, tutoring, health services, and emergency support.

## You will use

- [knowledge-base/pdf/campus-resources-guide.pdf](../knowledge-base/pdf/campus-resources-guide.pdf)
- [knowledge-base/pdf/campus-resources-faq.pdf](../knowledge-base/pdf/campus-resources-faq.pdf)
- `Campus Resources Agent` content from [copy-paste/agent-config.md](../copy-paste/agent-config.md)

## Create the agent

1. Open the main menu in watsonx Orchestrate.
2. Click `Create new agent`. (Or open `Build` in the hamburger menu and select `Create Agent`)
3. Select `Create from Scratch`
4. Fill in:
   - Name: `Campus Resources Agent`
   - Description: copy the `Campus Resources Agent description` block from [copy-paste/agent-config.md](../copy-paste/agent-config.md)
5. Click `Create`.

## Upload knowledge

1. Go to `Knowledge`.
2. Click `Add knowledge` -> `New Knowledge` -> `Upload files` -> `Next`.
3. Upload:
   - [knowledge-base/pdf/campus-resources-guide.pdf](../knowledge-base/pdf/campus-resources-guide.pdf)
   - [knowledge-base/pdf/campus-resources-faq.pdf](../knowledge-base/pdf/campus-resources-faq.pdf)
4. Paste the `Campus Resources knowledge description` from [copy-paste/agent-config.md](../copy-paste/agent-config.md).
5. Save.

## Configure behavior

Paste the `Campus Resources Agent behavior` block from [copy-paste/agent-config.md](../copy-paste/agent-config.md) into the `Behavior` section.

## Quick test

Use one of the prompts from [copy-paste/test-prompts.md](../copy-paste/test-prompts.md), such as:

> Donde esta la despensa de comida del campus y cuales son los horarios?

Check for three things:

1. The answer is in Spanish if the prompt is in Spanish
2. The answer cites the knowledge files
3. The answer includes practical details like location and hours

## Deploy

1. Click `Deploy`
2. Confirm with `Deploy`

## Checkpoint

You are done with Step 2 when:

- The agent exists
- The two campus resource PDFs are attached
- `Show Agent` is off
- The quick test works
- The agent is deployed

## Next step

Go to [docs/03-supervisor-agent.md](03-supervisor-agent.md).
