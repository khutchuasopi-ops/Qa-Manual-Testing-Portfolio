# BUG-008 — New Chat Temporarily Displays the Previous Conversation

## Title
New Chat temporarily displays the previous conversation

## Preconditions
- User is logged in.
- An existing AI Chat conversation contains messages.

## Steps to Reproduce
1. Open AI Chat.
2. Open an existing conversation containing messages.
3. Click `New Chat`.
4. Observe the conversation area before entering any new text.
5. Enter a new message.
6. Observe the conversation area again.

## Expected Result
Clicking `New Chat` should immediately open a clean conversation with no messages from the previous chat.

## Actual Result
After clicking `New Chat`, the previous conversation remains visible temporarily.

After entering a new message, the chat refreshes and the previous conversation disappears.

## Priority
Medium

## Severity
Minor

## Environment
- Environment: Staging / Preview
- Testing type: Manual QA
- Area: AI Chat

## Evidence
Screen recording showing the previous conversation remaining visible immediately after clicking New Chat, followed by the state after entering a new message.

## Status
Open
