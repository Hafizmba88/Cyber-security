# Attack Types — Concise Notes

Quick, study-ready reference covering common attack types, examples, affected domains, and brief mitigation notes.

## Overview

Attacks vary in technique, scope, and impact. Many attacks overlap multiple security domains (CISSP-style): Security & Risk Management, Asset Security, Security Architecture & Engineering, Communications & Network Security, Identity & Access Management, Security Operations, and Software Development Security.

---

## Password attacks

Definition: Attempts to obtain or guess credentials to gain unauthorized access.
Common forms:

- Brute force — try every possible password until success.
- Dictionary attacks — try common or leaked passwords from lists.
- Rainbow tables — precomputed hashes to reverse weakly hashed passwords.
Mitigation:
- Use strong, unique passwords and passphrases.
- Enforce rate limiting, account lockout thresholds, multi-factor authentication (MFA).
- Salt and use slow hashing algorithms (bcrypt, Argon2).

Domain: Communications & Network Security (also Identity & Access Management for authentication controls).

---



## Social engineering attacks

Definition: Manipulation of people to divulge information or grant access.
Common forms:

- Phishing, Spear phishing, Whaling
- Smishing (SMS), Vishing (voice)
- Social media phishing
- Business Email Compromise (BEC)
- Watering hole attacks
- USB baiting, Physical social engineering
Mitigation:
- Security awareness training and phishing simulations.
- Strong email authentication (SPF, DKIM, DMARC).
- Least privilege, verification processes for sensitive requests, device policies.
Domain: Security & Risk Management (human risk), with overlaps into other domains.

---



## Physical attacks

Definition: Attacks that target physical devices or infrastructure.
Examples:

- Malicious USB cables or flash drives
- Card cloning and skimming
- Theft or tampering of hardware
Mitigation:
- Physical access controls, device control policies, endpoint protection, asset inventories.
Domain: Asset Security

---



## Adversarial artificial intelligence

Definition: Techniques that manipulate ML/AI models (poisoning, evasion) to degrade performance or bypass controls.
Examples:

- Data poisoning, adversarial inputs that fool classifiers
Mitigation:
- Secure ML pipelines, data validation, model monitoring, robust training techniques.
Domain: Communications & Network Security and Identity & Access Management (model and data integrity).

---



## Supply-chain attacks

Definition: Compromise of third-party components, libraries, or vendors to introduce malicious code or hardware.
Impact: Can affect multiple organizations simultaneously and persist across updates.
Mitigation:

- Vendor risk management, software bill of materials (SBOM), code signing, dependency scanning, least privilege for integrated services.
Domain: Security & Risk Management, Security Architecture & Engineering, Security Operations

---



## Cryptographic attacks

Definition: Attacks against cryptographic algorithms, protocols, or implementations.
Examples:

- Birthday attacks (collisions)
- Collision attacks on hashing
- Downgrade attacks (forcing weaker protocols)
Mitigation:
- Use strong, up-to-date algorithms and key lengths, implement protocol version enforcement, apply patches to crypto libraries, use forward secrecy where applicable.
Domain: Communications & Network Security

---



## Key takeaways

- Attacks often cross multiple domains; defenses should be layered (defense-in-depth).
- Human factors (social engineering) are high-risk and require training plus technical controls.
- Supply-chain and AI threats are growing; incorporate vendor and model security into risk assessments.
- Regularly review, patch, and monitor systems; use strong authentication and least privilege.

---



## Suggested practice / study activities

- Run a phishing simulation and prepare a post-sim remediation plan.
- Build a small lab: test password cracking against a deliberately weak hash (legal, isolated lab).
- Map a known supply-chain incident (e.g., SolarWinds) and list mitigations.
- Experiment with simple adversarial inputs against an open-source ML model to learn defensive approaches.



## Resources

- OWASP Top 10, OWASP Cheat Sheets
- NIST SP 800 series (authentication, supply chain, crypto)
- CIS Controls
- Vendor security advisories and CVE details

