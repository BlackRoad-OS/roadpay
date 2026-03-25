<!-- BlackRoad SEO Enhanced -->

# roadpay

> Part of **[BlackRoad OS](https://blackroad.io)** — Sovereign Computing for Everyone

[![BlackRoad OS](https://img.shields.io/badge/BlackRoad-OS-ff1d6c?style=for-the-badge)](https://blackroad.io)
[![BlackRoad OS](https://img.shields.io/badge/Org-BlackRoad-OS-2979ff?style=for-the-badge)](https://github.com/BlackRoad-OS)
[![License](https://img.shields.io/badge/License-Proprietary-f5a623?style=for-the-badge)](LICENSE)

**roadpay** is part of the **BlackRoad OS** ecosystem — a sovereign, distributed operating system built on edge computing, local AI, and mesh networking by **BlackRoad OS, Inc.**

## About BlackRoad OS

BlackRoad OS is a sovereign computing platform that runs AI locally on your own hardware. No cloud dependencies. No API keys. No surveillance. Built by [BlackRoad OS, Inc.](https://github.com/BlackRoad-OS-Inc), a Delaware C-Corp founded in 2025.

### Key Features
- **Local AI** — Run LLMs on Raspberry Pi, Hailo-8, and commodity hardware
- **Mesh Networking** — WireGuard VPN, NATS pub/sub, peer-to-peer communication
- **Edge Computing** — 52 TOPS of AI acceleration across a Pi fleet
- **Self-Hosted Everything** — Git, DNS, storage, CI/CD, chat — all sovereign
- **Zero Cloud Dependencies** — Your data stays on your hardware

### The BlackRoad Ecosystem
| Organization | Focus |
|---|---|
| [BlackRoad OS](https://github.com/BlackRoad-OS) | Core platform and applications |
| [BlackRoad OS, Inc.](https://github.com/BlackRoad-OS-Inc) | Corporate and enterprise |
| [BlackRoad AI](https://github.com/BlackRoad-AI) | Artificial intelligence and ML |
| [BlackRoad Hardware](https://github.com/BlackRoad-Hardware) | Edge hardware and IoT |
| [BlackRoad Security](https://github.com/BlackRoad-Security) | Cybersecurity and auditing |
| [BlackRoad Quantum](https://github.com/BlackRoad-Quantum) | Quantum computing research |
| [BlackRoad Agents](https://github.com/BlackRoad-Agents) | Autonomous AI agents |
| [BlackRoad Network](https://github.com/BlackRoad-Network) | Mesh and distributed networking |
| [BlackRoad Education](https://github.com/BlackRoad-Education) | Learning and tutoring platforms |
| [BlackRoad Labs](https://github.com/BlackRoad-Labs) | Research and experiments |
| [BlackRoad Cloud](https://github.com/BlackRoad-Cloud) | Self-hosted cloud infrastructure |
| [BlackRoad Forge](https://github.com/BlackRoad-Forge) | Developer tools and utilities |

### Links
- **Website**: [blackroad.io](https://blackroad.io)
- **Documentation**: [docs.blackroad.io](https://docs.blackroad.io)
- **Chat**: [chat.blackroad.io](https://chat.blackroad.io)
- **Search**: [search.blackroad.io](https://search.blackroad.io)

---


[![GitHub](https://img.shields.io/badge/GitHub-BlackRoad-OS-purple?style=for-the-badge&logo=github)](https://github.com/BlackRoad-OS/roadpay)
[![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)](https://github.com/BlackRoad-OS/roadpay)
[![BlackRoad](https://img.shields.io/badge/BlackRoad-OS-black?style=for-the-badge)](https://blackroad.io)

# RoadPay

Payment processing platform for the BlackRoad ecosystem.

## Features

- **Stripe Integration** - Full Stripe API support
- **Subscriptions** - Recurring billing management
- **One-time Payments** - Payment intents
- **Invoicing** - Create and manage invoices
- **Checkout** - Hosted checkout sessions
- **Billing Portal** - Customer self-service
- **Webhooks** - Real-time event handling

## Quick Start

```bash
# Install
pip install -e .

# Set environment
export ROADPAY_STRIPE_SECRET_KEY=sk_test_...
export ROADPAY_STRIPE_WEBHOOK_SECRET=whsec_...

# Run
roadpay
```

## API Endpoints

### Customers
- `POST /customers` - Create customer
- `GET /customers/{id}` - Get customer
- `GET /customers/{id}/subscriptions` - Customer subscriptions

### Payments
- `POST /payments/intent` - Create payment intent
- `GET /payments/{id}` - Get payment status

### Products & Prices
- `POST /products` - Create product
- `GET /products` - List products
- `POST /prices` - Create price
- `GET /prices` - List prices

### Subscriptions
- `POST /subscriptions` - Create subscription
- `GET /subscriptions/{id}` - Get subscription
- `POST /subscriptions/{id}/cancel` - Cancel subscription

### Invoices
- `POST /invoices` - Create invoice
- `GET /invoices/{id}` - Get invoice

### Checkout
- `POST /checkout/session` - Create checkout session
- `POST /billing/portal` - Create billing portal session

## License

Proprietary - BlackRoad OS, Inc.
