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

CoinStats also published a [Google Sheet of affected wallet addresses](https://docs.google.com/spreadsheets/d/1Lwxpy2T6W7aptjBJUio0Z01zihsqknXn6KPhzawQLVI/) after the incident. The public list includes both Ethereum and Bitcoin addresses. Examples from that list include Ethereum addresses [0xa78a1943a1785De25d7dA4Fe56F961409123B3B3](https://etherscan.io/address/0xa78a1943a1785De25d7dA4Fe56F961409123B3B3), [0x84AC64a923343Dd06F22b58B370bd5Eb73723872](https://etherscan.io/address/0x84AC64a923343Dd06F22b58B370bd5Eb73723872), and [0x16B8E436106996C1D2c71e05d4cCC5F665e23795](https://etherscan.io/address/0x16B8E436106996C1D2c71e05d4cCC5F665e23795), alongside Bitcoin addresses such as [1N8DVn2hFJaFcjDH5eSA7uezdDFLXJrhR3](https://www.blockchain.com/explorer/addresses/btc/1N8DVn2hFJaFcjDH5eSA7uezdDFLXJrhR3) and [14QZYWozEHbV6amQGoP8RxWYgVCM4WReDP](https://www.blockchain.com/explorer/addresses/btc/14QZYWozEHbV6amQGoP8RxWYgVCM4WReDP).

Representative Ethereum drain transactions from those listed wallets also expose recipient wallets on-chain. Examples include [0xeb4419a3b1c4e115883f69b74efe97af8a1b33919ec3164eb9556bc944932640](https://etherscan.io/tx/0xeb4419a3b1c4e115883f69b74efe97af8a1b33919ec3164eb9556bc944932640), which moved funds from listed wallet [0xa78a1943a1785De25d7dA4Fe56F961409123B3B3](https://etherscan.io/address/0xa78a1943a1785De25d7dA4Fe56F961409123B3B3) to recipient [0x0e70FD0271B41Ca77A2Efdcb07Ab178602122D8c](https://etherscan.io/address/0x0e70FD0271B41Ca77A2Efdcb07Ab178602122D8c), [0x102552794a6606a9590b21340b31f731ec3c6d5b77841982ae292bae9a0b6300](https://etherscan.io/tx/0x102552794a6606a9590b21340b31f731ec3c6d5b77841982ae292bae9a0b6300), which moved funds from listed wallet [0x84AC64a923343Dd06F22b58B370bd5Eb73723872](https://etherscan.io/address/0x84AC64a923343Dd06F22b58B370bd5Eb73723872) to recipient [0x00b03FE97B4D7b1f8948b68D0065344D37AaD193](https://etherscan.io/address/0x00b03FE97B4D7b1f8948b68D0065344D37AaD193), and [0x4d01a86d3deaa629d5a1bb45daa48869fb1d4188ee210892465f05b3d15c7116](https://etherscan.io/tx/0x4d01a86d3deaa629d5a1bb45daa48869fb1d4188ee210892465f05b3d15c7116), which moved funds from listed wallet [0x16B8E436106996C1D2c71e05d4cCC5F665e23795](https://etherscan.io/address/0x16B8E436106996C1D2c71e05d4cCC5F665e23795) to recipient [0xe0eB698Cc1359884A482096AE732E3A309f615E0](https://etherscan.io/address/0xe0eB698Cc1359884A482096AE732E3A309f615E0).

## Losses

CoinStats said exactly *1,590 CoinStats Wallets* were affected and that about *$2.2 million* in cryptocurrency was stolen.

The company separately published a [Google Sheet of affected wallet addresses](https://docs.google.com/spreadsheets/d/1Lwxpy2T6W7aptjBJUio0Z01zihsqknXn6KPhzawQLVI/). Public reporting noted that the majority of the stolen funds appeared to be concentrated in a small number of wallets, but CoinStats did not publish a full official asset-by-asset breakdown in the incident report.

## Timeline

- **June 22, 2024, 18:00 UTC:** CoinStats said it detected abnormal transfer activity involving wallets created directly within CoinStats Wallet.
- **June 22, 2024, 18:17 UTC:** CoinStats posted on [X](https://x.com/CoinStats/status/1804579591698120760) that some iOS users had received a scam notification and that it was investigating that notification issue.
- **June 22, 2024, 19:57 UTC:** CoinStats posted on [X](https://x.com/CoinStats/status/1804604741197893739) that it was experiencing a separate confirmed security incident affecting wallets created directly within CoinStats and advised users with exported private keys to move funds immediately.
- **June 22, 2024, about 23:00 UTC:** CoinStats published an [update on X](https://x.com/CoinStats/status/1804633869372559788) stating that the application had been temporarily shut down, that 1,590 wallets were affected, and that it had published a list of impacted addresses.
- **June 23, 2024:** Public on-chain activity from addresses later included in CoinStats' affected-wallet sheet showed funds moving out of listed wallets. Representative Ethereum transactions include [0xeb4419a3b1c4e115883f69b74efe97af8a1b33919ec3164eb9556bc944932640](https://etherscan.io/tx/0xeb4419a3b1c4e115883f69b74efe97af8a1b33919ec3164eb9556bc944932640) from listed address [0xa78a1943a1785De25d7dA4Fe56F961409123B3B3](https://etherscan.io/address/0xa78a1943a1785De25d7dA4Fe56F961409123B3B3), [0x102552794a6606a9590b21340b31f731ec3c6d5b77841982ae292bae9a0b6300](https://etherscan.io/tx/0x102552794a6606a9590b21340b31f731ec3c6d5b77841982ae292bae9a0b6300) from listed address [0x84AC64a923343Dd06F22b58B370bd5Eb73723872](https://etherscan.io/address/0x84AC64a923343Dd06F22b58B370bd5Eb73723872), and [0x4d01a86d3deaa629d5a1bb45daa48869fb1d4188ee210892465f05b3d15c7116](https://etherscan.io/tx/0x4d01a86d3deaa629d5a1bb45daa48869fb1d4188ee210892465f05b3d15c7116) from listed address [0x16B8E436106996C1D2c71e05d4cCC5F665e23795](https://etherscan.io/address/0x16B8E436106996C1D2c71e05d4cCC5F665e23795).
- **June 24, 2024:** [Unchained reported](https://unchainedcrypto.com/coinstats-temporarily-shuts-down-after-1590-wallets-drained/) that CoinStats had temporarily shut down after 1,590 wallets were drained and that CEO Narek Gevorgyan estimated the losses at around $2 million.
- **July 12, 2024:** CoinStats published its formal [security incident report](https://coinstats.app/blog/security-incident-report/), stating the later $2.2 million loss figure and describing unauthorized access to infrastructure and third-party services.

## Security Failure Causes

**Infrastructure and Third-Party Service Compromise, According to CoinStats:** CoinStats said the incident involved unauthorized access affecting parts of its infrastructure and external service providers, including HashiCorp Vault data and wallet-service APIs. The cited report does not provide a full public forensic reconstruction of how each accessed system contributed to the wallet thefts.

**Private-Key Access for CoinStats-Generated Wallets, According to CoinStats:** CoinStats said that, through a combination of intrusions spanning multiple services, the attacker managed to access private keys for exactly 1,590 CoinStats Wallets.

**Notification Abuse Was Publicly Reported but Not Fully Causally Mapped:** CoinStats separately acknowledged that some users received a malicious push notification and in-app message promoting a fake 14.2 ETH reward. Public materials did not fully document whether that notification abuse was a direct extension of the same intrusion path, a parallel abuse vector, or simply a concurrent malicious event during the same incident window.

