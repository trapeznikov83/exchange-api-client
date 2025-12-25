# exchange-api-client
Unified async client for centralized crypto exchanges (REST &amp; WebSocket) with normalized models, explicit rate-limit handling, and predictable behavior.

## Overview
Exchange API Client is a unified asynchronous client for centralized crypto exchanges (CEX).
It provides normalized access to REST and WebSocket APIs with explicit handling of rate limits,
timeouts, and retries.

The goal of this project is to abstract away exchange-specific API details and provide
a predictable interface for market data consumption.

## Supported Exchanges
- Bybit (REST, WebSocket – market data)
- Binance (planned)

## Features
- Unified REST and WebSocket interfaces
- Normalized market data models
- Explicit rate-limit control
- Retry and timeout handling
- Async-first design

## Architecture
The project is structured around a clear separation of responsibilities:

- **Transport layer** — low-level REST and WebSocket communication
- **Exchange clients** — exchange-specific adapters
- **Domain models** — normalized internal representations
- **Utilities** — rate limiting, retries, and time handling