# BUG-008 — New Chat Temporarily Shows Previous Conversation

## Summary

When the user starts a **New Chat**, the previous conversation is temporarily displayed before the new conversation state is initialized.

## Preconditions

* User has access to AI Chat.
* An existing conversation contains previous messages.

## Steps to Reproduce

1. Open **AI Chat**.
2. Open an existing conversation containing messages.
3. Select **New Chat**.
4. Immediately observe the conversation area before entering a new message.
5. Enter a new message.
6. Observe the conversation again.

## Actual Result

After selecting **New Chat**, messages from the previous conversation are temporarily displayed.

The previous conversation remains visible until the user enters a new message, after which the new conversation state is displayed.

## Expected Result

After selecting **New Chat**, the previous conversation should be cleared immediately.

The user should see a clean new conversation state before entering the first message.

## Severity

**Medium**

## Environment

**Staging / Preview**

## Related Test Case

**TC-022 — AI Chat: Start New Chat**

## Status

**Open**

## Reproduction

**Reproduced during manual testing.**

## Notes

Displaying messages from a previous conversation when starting a new Chat can cause confusion and may make the user believe that the previous conversation is still active.

The new Chat state should be initialized before the conversation area is displayed to the user.
