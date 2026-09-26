# Security policy

## Repository scope

This repository contains the public profile, project links, artwork, and the contribution-graph GitHub Actions workflow. It does not contain the applications linked from the profile or an application server. Report product-specific issues through the affected project's own security policy.

Relevant concerns include accidental publication of credentials or private data, malicious link or artwork changes, and workflow changes that could expose the repository token or alter published content. The graph workflow invokes a third-party action and has repository write permission. Treat its action references and output as part of the publication boundary.

## Private reporting

Email <contact@magrathean.uk> with subject `SECURITY: Magrathean UK Profile`. This is the reporting address in the existing policy. If GitHub shows a private reporting option for this repository, that is another private route; its availability is not assumed here.

Include the affected file or URL, commit if known, reproduction steps, likely impact, and redacted evidence. Do not publish credentials, private keys, database dumps, signing certificates, or exploit details in public issues or pull requests.

This profile has no software release support matrix. This policy does not establish support periods for the products it links to.

## Scope & Safe Harbour

Magrathean UK Ltd. will not pursue a good-faith researcher for security disclosures that:
- Target non-production test systems or researcher-owned environments;
- Avoid persistence, destructive changes, denial of service, and access to personal or customer data;
- Report promptly and permit reasonable time for remediation;
- Do not condition non-disclosure on financial compensation.

## Excluded Conduct

No safe harbour covers phishing, credential stuffing, accessing private production infrastructure, large-scale scanning, denial of service, or unlawful conduct.
