# Personal Number Rights (PNR)

**A Proposal for Revocable Phone Number Permissions**

*Version 0.1 – Draft*  
*October 2026*

---

## 1. Introduction

Phone numbers are one of the most persistent and poorly controlled forms of personal data in everyday life. Once shared, a number can remain in other people’s contact lists, backups, and databases indefinitely. The owner has almost no practical ability to revoke access.

This paper proposes **Personal Number Rights (PNR)** — a system that treats reachability as a revocable permission rather than a permanent gift.

## 2. The Core Problem

- Sharing a phone number currently transfers permanent reachability.
- Numbers remain on other people’s devices even after relationships or circumstances change.
- There is no simple, reliable way for an individual to withdraw permission.
- Data-based messaging applications (WhatsApp, Signal, Telegram, etc.) create additional channels that bypass traditional call/SMS controls.
- Industrial robocalling and spam operate from large databases, making personal contact-list control insufficient on its own.

The result is a lasting loss of control over who can reach you.

## 3. Proposed Solution: Personal Number Rights

Personal Number Rights reframes a phone number as something the owner **grants** and can later **revoke**.

Instead of permanently giving someone your number, you issue a permission (a “lease”). When that permission is revoked, supporting systems stop allowing the other party to reach you.

## 4. Two-Phase Approach

### 4.1 Version 1 – Permission Layer

- Number owners issue digitally signed leases when sharing their number.
- Supporting carriers, networks, and applications check for a valid lease before completing calls or SMS.
- Revocation invalidates the lease so that further attempts to reach the number fail on supporting channels.
- Can be implemented without requiring changes to mobile operating system contact databases.

Version 1 delivers practical control over traditional telephony while remaining relatively lightweight to adopt.

### 4.2 Version 2 – Native Contact Integration

- Mobile operating systems treat contacts as revocable records.
- When a lease is revoked, the number is removed from the local contacts database.
- Restoring a backup does not reinstate the revoked number.
- Provides stronger protection across both traditional and data-based communication channels.

Version 2 requires cooperation from major platform vendors and represents the fuller realisation of the concept.

## 5. Technical Direction

The system should be designed as a decentralised permission layer:

- **Decentralised registry**: Lease and revocation records live on a distributed network with no single point of control or failure.
- **Geo-sharding**: Nodes primarily handle numbers for their own country or region, improving lookup performance for local traffic.
- **Cryptographic signatures**: Leases and revocations are digitally signed by the number owner.
- **Open verification**: Any supporting network or application can verify the current status of a lease.

This approach prioritises resilience, user control, and practical performance.

## 6. Governance

A neutral, independent foundation should act as steward of the protocol and reference implementations.

Recommended characteristics:
- Non-profit or public-benefit status
- Transparent and diverse governance
- Clear mission focused on user control and open standards
- Ability to employ staff while remaining independent of any single commercial operator

The foundation provides oversight and maintenance, not commercial telecom services.

## 7. Scope and Limitations

**Version 1** improves control over traditional calls and SMS where the permission layer is respected. It does not automatically block contact via data applications unless those applications also implement the standard.

Industrial robocalling is only partially addressed. A cryptographic Do-Not-Call capability can help, but should not be positioned as a complete anti-spam solution.

Existing numbers can continue to operate as they do today. New numbers may be issued with Personal Number Rights capabilities enabled.

## 8. Call to Action

Personal Number Rights is released as an open proposal. We invite privacy organisations, developers, carriers, messaging platforms, and operating-system vendors to examine, critique, and build upon these ideas.

The goal is to return meaningful control of personal reachability to the individual.

---

*This is an early draft intended to start discussion. Feedback and contributions are welcome.*
