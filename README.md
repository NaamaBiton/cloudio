# Cloudio — Cloud Storage Recovery

A simulated cloud storage incident response. A photo-hosting server failed and customer data became inaccessible. This project recovers the data — first manually for a single account, then via an automated Python script scaled across all customers.

---

## Scenario

- Cloud server hosting customer photos crashes
- Photos are still present on the server but the normal access layer is broken
- Goal: recover all customer photos with minimal manual effort

---

## Two-phase approach

**Phase 1 — Manual recovery**
Connected directly to the compromised server and manually retrieved photos for a single customer. This established the recovery procedure and validated that the underlying data was intact.

**Phase 2 — Automated batch recovery (`cloudio.py`)**
Automated the Phase 1 procedure in Python to scale across all customer accounts — no manual intervention needed per account.

---

## Tech stack

Python · File I/O · Server access · Automation scripting
