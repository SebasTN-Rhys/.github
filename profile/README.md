<div align="center">

# Sebastn

**Stripe Connect, batteries included.**

Payments infrastructure for GitHat-platform apps — Stripe Connect Express, next-day payouts, marketplace splits, Stripe Tax.

[**🌐 sebastn.com**](https://sebastn.com)&nbsp;&nbsp;·&nbsp;&nbsp;[**🔌 api.sebastn.com**](https://api.sebastn.com)&nbsp;&nbsp;·&nbsp;&nbsp;[**🏠 GitHat platform**](https://githat.io)

</div>

---

## What Sebastn is

Sebastn is the payments-as-a-service layer for the [GitHat](https://githat.io) platform. We own the Stripe Connect platform `acct_1QUAtoP61QTCwfMg` and onboard apps as connected accounts — so they get Stripe Connect Express with one integration, every payment method.

- **Connect Express** onboarding in < 5 minutes
- **Marketplace splits** with application_fee_amount
- **Next-day payouts** on the platform's schedule
- **Stripe Tax** automatic tax calculation in 40+ jurisdictions
- **Identity verification** via Stripe Identity
- **Refunds + disputes** dashboard

## Who uses it

- **[ClickReserv](https://github.com/ClickReserv)** — booking platform, businesses are Stripe connected accounts under Sebastn
- **[Quantl](https://github.com/QuantLinc)** — subscriptions for paid tiers
- Any [GitHat-platform](https://github.com/GitHat-IO) app that needs payments without re-implementing Stripe Connect

## Authentication

Sebastn auth is delegated to GitHat (`api.githat.io`). All operator login, MFA, OAuth, passkeys, and audit log live there — Sebastn never holds its own auth surface.

## Security

- ✅ Verified domain (`sebastn.com`, `www.sebastn.com`)
- ✅ AWS-native edge: Route 53 → CloudFront (ACM cert) → EC2 (Caddy → Node)
- ✅ Same-origin `/api/githat` proxy for httpOnly cookie auth (no localStorage tokens)
- ✅ PCI-compliant payment flows via Stripe Elements
- ✅ Webhook signature verification, idempotency keys, advisory locks
- ✅ CAA records, signed commits, secret scanning

## Contact

Security: [security@sebastn.com](mailto:security@sebastn.com)
Support: [hello@sebastn.com](mailto:hello@sebastn.com)
