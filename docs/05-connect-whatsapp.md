# Step 5: Connect the Bot to WhatsApp

This step is optional. If you are short on time, skip it and finish the workshop in web chat.

## Before you start

Make sure you have:

- A Twilio account
- Your `Account SID`
- Your `Auth Token`
- WhatsApp installed on your phone

## Create the WhatsApp channel in watsonx Orchestrate

1. Open the `Becas y Recursos Bot` agent.
2. Go to `Channels`.
3. Choose `WhatsApp with Twilio`.
4. Select `Live` environment.
5. Click `Create New`.
6. Fill in:
   - Name: `WhatsApp Integration`
   - Description: `WhatsApp Integration`
   - Account SID: your Twilio `Account SID`
   - Auth Token: your Twilio `Auth Token`
7. On the next screen, copy the **webhook URL** from watsonx Orchestrate.
8. Finish the channel setup.

Check that the channel moves to `Active`. If it stays in `Draft`, the bot will not respond.

## Configure Twilio

1. Open the Twilio Console.
2. Go to `Messaging` -> `Try it out` -> `Send a WhatsApp message`.
3. Open `Sandbox settings`.
4. In `When a message comes in`, paste the webhook URL from watsonx Orchestrate.
5. Leave the method set to `POST`.
6. Save.

## Join the sandbox from your phone

1. In Twilio, find the sandbox join code.
2. Open WhatsApp on your phone.
3. Send the join code to the Twilio sandbox number.
4. Wait for the confirmation message.

## Send test messages

Use the WhatsApp test prompts in [copy-paste/test-prompts.md](../copy-paste/test-prompts.md).

Start with:

1. `Hola, que becas hay para estudiantes latinos?`
2. `Where is the food pantry and when is it open?`
3. `I need help with FAFSA and I also need tutoring for calculus`

## Checkpoint

You are done with Step 5 when:

- The channel status is `Active`
- Twilio is pointing to the correct webhook URL
- Your phone has joined the sandbox
- The bot answers your WhatsApp messages

## Next step

Read [docs/06-troubleshooting.md](06-troubleshooting.md) if anything is not working.
