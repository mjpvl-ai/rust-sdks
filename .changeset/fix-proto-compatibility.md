---
livekit: patch
livekit-api: patch
livekit-uniffi: patch
---

Fix compile failures caused by changes in the `livekit-protocol` schema, specifically by:
- Initializing new `compression` and `inline_content` fields in the outgoing `Header` struct.
- Initializing the new `media` field in SIP inbound/outbound trunks.
- Adding the new `attributes` field to `RoomAgentDispatch` in `livekit-uniffi` to match the updated protocol structure.
