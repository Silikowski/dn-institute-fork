---
date: 2024-06-22
target-entities: CoinStats
entity-types:
  - Wallet
attack-types:
  - Wallet Hack
title: "CoinStats Security Incident Exposes 1,590 Wallets and Leads to $2.2 Million Theft"
loss: 2200000
---

## Summary

On June 22, 2024, CoinStats disclosed a security incident affecting wallets created directly within CoinStats Wallet. The company said the incident did not affect externally connected wallets or exchange accounts used only for portfolio tracking, but it did affect 1,590 CoinStats Wallets and led to thefts totaling about $2.2 million.

In its later incident report, CoinStats said unauthorized access affected parts of its infrastructure and external service providers, and that the attacker accessed private keys through a combination of intrusions across multiple services. CoinStats also warned users on June 22 about a malicious push notification and in-app message that promoted a fake 14.2 ETH reward and directed some users toward a drainer page. Public materials document both the notification lure and the confirmed incident affecting CoinStats-created wallets, but they do not publicly establish the exact technical relationship between those events or whether they reflected one intrusion path or parallel abuse during the same incident window.

## Attackers

The attacker or attackers were not publicly identified.

CoinStats stated, after work with law enforcement and external researchers, that its evidence pointed to Lazarus Group or a related organization with nation-state-level capabilities. The cited public materials do not independently substantiate that attribution as a third-party forensic conclusion.

CoinStats said its response involved Security Alliance, ZachXBT, and Tay from MetaMask, and that the incident was reported to local law enforcement and the FBI.

## Losses

CoinStats said exactly *1,590 CoinStats Wallets* were affected and that about *$2.2 million* in cryptocurrency was stolen.

The company separately published a [Google Sheet of affected wallet addresses](https://docs.google.com/spreadsheets/d/1Lwxpy2T6W7aptjBJUio0Z01zihsqknXn6KPhzawQLVI/). Public reporting noted that the majority of the stolen funds appeared to be concentrated in a small number of wallets, but CoinStats did not publish a full official asset-by-asset breakdown in the incident report.

## Timeline

- **June 22, 2024, 18:00 UTC:** CoinStats said it detected abnormal transfer activity involving wallets created directly within CoinStats Wallet.
- **June 22, 2024, 18:17 UTC:** CoinStats posted on [X](https://x.com/CoinStats/status/1804579591698120760) that some iOS users had received a scam notification and that it was investigating that notification issue.
- **June 22, 2024, 19:57 UTC:** CoinStats posted on [X](https://x.com/CoinStats/status/1804604741197893739) that it was experiencing a separate confirmed security incident affecting wallets created directly within CoinStats and advised users with exported private keys to move funds immediately.
- **June 22, 2024, about 23:00 UTC:** CoinStats published an [update on X](https://x.com/CoinStats/status/1804633869372559788) stating that the application had been temporarily shut down, that 1,590 wallets were affected, and that it had published a list of impacted addresses.
- **June 24, 2024:** Unchained reported that CoinStats had temporarily shut down after 1,590 wallets were drained and that CEO Narek Gevorgyan estimated the losses at around $2 million.
- **July 12, 2024:** CoinStats published its formal [security incident report](https://coinstats.app/blog/security-incident-report/), stating the later $2.2 million loss figure and describing unauthorized access to infrastructure and third-party services.

## Security Failure Causes

**Infrastructure and Third-Party Service Compromise, According to CoinStats:** CoinStats said the incident involved unauthorized access affecting parts of its infrastructure and external service providers, including HashiCorp Vault data and wallet-service APIs. The cited report does not provide a full public forensic reconstruction of how each accessed system contributed to the wallet thefts.

**Private-Key Access for CoinStats-Generated Wallets, According to CoinStats:** CoinStats said that, through a combination of intrusions spanning multiple services, the attacker managed to access private keys for exactly 1,590 CoinStats Wallets.

**Notification Abuse Was Publicly Reported but Not Fully Causally Mapped:** CoinStats separately acknowledged that some users received a malicious push notification and in-app message promoting a fake 14.2 ETH reward. Public materials did not fully document whether that notification abuse was a direct extension of the same intrusion path, a parallel abuse vector, or simply a concurrent malicious event during the same incident window.

## References

- [CoinStats X update: scam notification investigation](https://x.com/CoinStats/status/1804579591698120760)
- [CoinStats X update: wallets created directly within CoinStats affected](https://x.com/CoinStats/status/1804604741197893739)
- [CoinStats X update: 1,590 wallets affected](https://x.com/CoinStats/status/1804633869372559788)
- [CoinStats: Security Incident Report](https://coinstats.app/blog/security-incident-report/)
- [Affected CoinStats Wallet Addresses](https://docs.google.com/spreadsheets/d/1Lwxpy2T6W7aptjBJUio0Z01zihsqknXn6KPhzawQLVI/)
- [Unchained: CoinStats Temporarily Shuts Down After 1,590 Wallets Drained](https://unchainedcrypto.com/coinstats-temporarily-shuts-down-after-1590-wallets-drained/)
