# Troubleshooting

Use this page when something breaks during the live workshop.

## If watsonx Orchestrate is slow

- Wait 10 to 15 seconds before clicking again
- Avoid double-clicking through agent creation or deploy screens
- If the platform is unusable, switch to an instructor-led demo and keep students following the flow conceptually

## If file upload fails

- Make sure you are using the PDFs in [knowledge-base/pdf](../knowledge-base/pdf)
- Try uploading one file at a time
- Confirm the files are not still open in another program that is locking them
- If uploads keep failing, continue without knowledge files and focus on the orchestration pattern

## If the supervisor does not appear in chat

- Open the supervisor agent and confirm `Show Agent` is `ON`
- Open each specialist agent and confirm `Show Agent` is `OFF`
- Redeploy the supervisor after changing the channel settings

## If routing looks wrong

- Re-check the supervisor behavior instructions in [copy-paste/agent-config.md](../copy-paste/agent-config.md)
- Make sure both specialist agents were added in the supervisor `Toolset`
- Retry with a cleaner prompt that only asks about one topic

## If citations are missing

- Confirm the knowledge files were uploaded successfully
- Wait for any indexing or processing to finish if the platform shows that state
- Test each specialist agent directly before testing the supervisor

## If WhatsApp replies with the Twilio echo message

- The watsonx Orchestrate WhatsApp channel is probably still in `Draft`
- Re-open the channel and check that it is `Active`
- Re-copy the webhook URL into Twilio with no extra spaces


