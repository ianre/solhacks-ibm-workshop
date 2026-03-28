# Step 1: Create the Scholarship Agent

This is your first specialist agent. It answers questions about scholarships, FAFSA, grants, and financial aid.

## You will use

- [knowledge-base/pdf/scholarships-overview.pdf](../knowledge-base/pdf/scholarships-overview.pdf)
- [knowledge-base/pdf/scholarship-faq.pdf](../knowledge-base/pdf/scholarship-faq.pdf)
- `Scholarship Agent` content from [copy-paste/agent-config.md](../copy-paste/agent-config.md)

## Create the agent

1. Log in to watsonx Orchestrate.
2. Click `Create new agent`. (Or open `Build` in the hamburger menu and select `Create Agent`)
3. Select `Create from Scratch`
3. Fill in:
   - Name: `Scholarship Agent`
   - Description: copy the `Scholarship Agent description` block from [copy-paste/agent-config.md](../copy-paste/agent-config.md)
4. Click `Create`.

## Upload knowledge

1. Open the `Knowledge` section.
2. Click `Add knowledge` -> `New Knowledge` -> `Upload files` -> `Next`.
3. Upload:
   - [knowledge-base/pdf/scholarships-overview.pdf](../knowledge-base/pdf/scholarships-overview.pdf)
   - [knowledge-base/pdf/scholarship-faq.pdf](../knowledge-base/pdf/scholarship-faq.pdf)
4. Paste the `Scholarship knowledge description` from [copy-paste/agent-config.md](../copy-paste/agent-config.md).
5. Name it something `Scholarship Knowledge` is an option.
6. Save.

## Configure behavior

Paste the `Scholarship Agent behavior` block from [copy-paste/agent-config.md](../copy-paste/agent-config.md) into the `Behavior` section.


## Quick test

Use one of the prompts from [copy-paste/test-prompts.md](../copy-paste/test-prompts.md), such as:

> What scholarships are available for Hispanic students, and when is the FAFSA deadline?

Check for three things:

1. The answer uses content from the uploaded files
2. The answer includes citations
3. The answer stays on scholarship and financial aid topics

## Deploy

1. Click `Deploy`
2. Confirm with `Deploy`

## Checkpoint

You are done with Step 1 when:

- The agent exists
- The two scholarship PDFs are attached
- `Show Agent` is off
- The quick test works
- The agent is deployed

## Next step

Go to [docs/02-campus-resources-agent.md](02-campus-resources-agent.md).
