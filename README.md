# N-Judge

N-Judge is a lightweight, scalable online judging system for programming contests.  
It enables contest administrators to manage problems, submissions, and scoring in real time, with built-in support for distributed judge machines and secure sandboxed execution.

## Key Features
- Multi-language submission support (C++, Python, Java, etc.)
- Secure execution via Docker or Linux sandboxing
- Real-time scoreboard updates over WebSocket with authentication
- Configurable time and memory limits per problem
- Judge node auto-discovery, heartbeat, and load-aware dispatching

## Use Cases
- University programming contests
- Training platforms for competitive programming teams
- Small to medium-scale online coding competitions

## Quick Notes
- Designed to be extended: add more languages, persistent job queues, or advanced auth (mTLS/JWT).
- Recommended infra: Docker for judge sandboxes, Redis for worker registry/queue, HTTPS/WSS for transport.
- Start small (MVP) and iterate: basic submit → judge → verdict → scoreboard, then add features.
