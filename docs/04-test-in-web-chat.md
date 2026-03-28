# Step 4: Test in Web Chat

This is the moment where you confirm the multi-agent system actually works.

## Open the chat

1. Open the main menu in watsonx Orchestrate.
2. Click `Chat`.
3. In the agent dropdown, choose `Becas y Recursos Bot`.

Only the supervisor should appear in the dropdown if you turned `Show Agent` off for the two specialist agents.

## Run three tests

Use the prompts in [copy-paste/test-prompts.md](../copy-paste/test-prompts.md).

### Test 1: Scholarships in English

> What scholarships are available for first-generation Hispanic students?

### Test 2: Campus resources in Spanish

> Necesito ayuda. No tengo suficiente comida esta semana. Que recursos hay en el campus?

### Test 3: Multi-agent routing

> I need to find scholarships for next semester and I also want to know about tutoring services.

## What to look for

1. Scholarship questions should be answered from the scholarship documents
2. Campus support questions should be answered from the campus resources documents
3. Multi-topic questions should be answered in one combined response
4. The bot should match the language of the student
5. Citations should still appear in the specialist responses

## Use reasoning if available

If your instance includes `Show Reasoning`, open it while testing. This helps you see how the supervisor decided which agent to use.

## Checkpoint

You are done with Step 4 when:

- The supervisor responds in chat
- The bot routes each test correctly
- The bilingual behavior works

## Next step

Go to [docs/05-connect-whatsapp.md](05-connect-whatsapp.md).
