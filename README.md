# NoCTX

NoCTX is a context-aware heads-up display (HUD) that streamlines user experience
on the desktop. It provides instant feedback and possible actions based the
selected item and its corresponding context, allowing the user to maintain a
*flow* state without disruption.

## Design

NoCTX is based on the server/client model and communcate via RPC.

#### Frontend

The HUD should be ready at all times to reduce launch overhead, but only activate
when NoCTX is sure the user wants it.

#### Backend

The backend is written in Rust for performance reasons and build upon the
tokio framework.

## Extension

NoCTX is designed from the group up to be extendable using user provided scripts,
interacting with the backend with RPC. These custom scripts can be written in
any language as long as they are capable to communcate via RPC.
