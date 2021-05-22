# Bugs

## High Importance (Potential loss of funds)
| Type | Description | Link | Action |
| ---  | ---         | ---  | ---    |
| Bug  | No Backup   | https://github.com/sparrowwallet/sparrow/issues/53   | 6102 to try and replicate     |
| Bug  | Possible external address shown to user | https://github.com/sparrowwallet/sparrow/issues/125 | Awaiting clarification from user | 

## Medium Importance (Serious Frustration / Annoyance / Confusion)
| Type | Description | Link | Status |
| ---  | ---         | ---  | ---    |
| Bug | Electrum can't verify sparrow sigs | https://github.com/sparrowwallet/sparrow/issues/39 | Add note that electrum can't verify sparrow sigs | 

## Low Importance (Minor Inconvenience)
| Type | Description | Link | Action |
| ---  | ---         | ---  | ---    |
| Bug | Font  | https://github.com/sparrowwallet/sparrow/issues/19 | Monitor [openjdk issue](Monitor openjdk issue and update when fixed) and update when fixed | 
| Bug | Slow indexing of large wallets | https://github.com/sparrowwallet/sparrow/issues/28 | Run tests to benchmark speed |
| Bug | Connection issues | https://github.com/sparrowwallet/sparrow/issues/29 | More clearly display server has hit max retries in UI | 
| Bug | Tor to Non-Tor connection switch or VPN to Non-VPN switch causes issues | https://github.com/sparrowwallet/sparrow/issues/29 | Switching could restart sparrow? |

## Unclear
| Type | Description | Link | Action |
| ---  | ---         | ---  | ---    |
| Bug | Wallet in inconsistent state | https://github.com/sparrowwallet/sparrow/issues/33 | Electrum error messaging has been fixed |
| Bug | Abandoned unconfirmed tx causes crash | https://github.com/sparrowwallet/sparrow/issues/74 | Identify whether problem still exists. Identify whether fix can be applied to bwt and if so talk to shesek. |

## Check fixed in next release
| Type | Description | Link | Fix |
| ---  | ---         | ---  | ---    |
| Bug | Scaling issue | https://github.com/sparrowwallet/sparrow/issues/117 | https://github.com/sparrowwallet/sparrow/commit/c5b09189df65ce51c340af11429912ff8fd5bc16 |

-----

# Features

## High Importance (Solves a significant issue)
| Type | Description | Link | Action |
| ---  | ---         | ---  | ---    |
| Feature | Store labels | High | https://github.com/sparrowwallet/sparrow/issues/109 | Store labels locally to avoid loosing a label. | 


## Medium Importance (Broadly Useful)
| Type | Description | Link | Action |
| ---  | ---         | ---  | ---    |
| Feature | Show hash of message when signing |  https://github.com/sparrowwallet/sparrow/issues/39 | Add note that electrum can't verify sparrow sigs | 
| Feature | Key rotation option on changing a keystore |  https://github.com/sparrowwallet/sparrow/issues/128 | Identify whether key rotation is a desirable feature. If so, identify how to best implement and do so. |
| Feature | Custom OpReturn output when spending | https://github.com/sparrowwallet/sparrow/issues/97 | Identify way of adding OpReturn functionality without compromising UI |
| Feature | Hex Formatting | https://github.com/sparrowwallet/sparrow/issues/99 | Format HEX into 4 columns of 8 bytes |
| Feature | SLIP39 (Shamir) |  https://github.com/sparrowwallet/sparrow/issues/103 | Research tradeoffs between SSKH vs SLIP39 (I suspect SSKH is preferable) and implement. | 
| Feature | SSKR (Shamir) | https://github.com/sparrowwallet/sparrow/issues/103#issuecomment-821004439 | 6102 - Seems more robust https://github.com/BlockchainCommons/Research/blob/master/papers/bcr-2020-011-sskr.md | 
| Feature | Checkbox utxo selection | https://github.com/sparrowwallet/sparrow/issues/115 | Uses space, CTRL/CMD-Click works, Could be made more obvious | 
| Feature | Add AEZEED (LND) Import | https://github.com/sparrowwallet/sparrow/issues/120 | Nice to have. May be significant work for a niche feature |
| Feature | Connect to Core with RPC not BWT | https://github.com/sparrowwallet/sparrow/issues/83 | ProofOfKeags to steward the requisite PRs in the
dependencies and revisit when the deps are ready | 

## Low Importance (Niche)
| Type | Description | Link | Action |
| ---  | ---         | ---  | ---    |
| Feature | AppImage | https://github.com/sparrowwallet/sparrow/issues/1 | Add AppImage Release | 
| Feature | Unclear when server is connected | https://github.com/sparrowwallet/sparrow/issues/69 | Could add indication that server has successfully connected? |
| Feature | Different constants for int/ext chains | https://github.com/sparrowwallet/sparrow/issues/81 | Monitor interest in this feature to determine whether to add this functionality |
| Feature | bip85 table | https://github.com/sparrowwallet/sparrow/issues/112 | Allow encryption & storage of a small amount of additional structured data with a wallet | 
| Feature | Multiple schemes per wallet | https://github.com/sparrowwallet/sparrow/issues/57 | Access multiple wallets in a single file without compromising sparrow's UI architecture |
| Feature | Multiple accounts in one wallet | https://github.com/sparrowwallet/sparrow/issues/92 | Access multiple wallets in a single file without compromising sparrow's UI architecture (as per #57). |
| Feature | Remote Broadcast Indication | https://github.com/sparrowwallet/sparrow/issues/130 | Add Broadcast Toggle? |

## Unclear
| Type | Description | Link | Action |
| ---  | ---         | ---  | ---    |
| Feature | Trimmed QR codes | https://github.com/sparrowwallet/sparrow/issues/78 | Identify an example of a PSBT that fails to scan. |


## NACK'd by Craig
| Type | Description | Link | Status |
| ---  | ---         | ---  | ---    |
| Feature | bip39 word suggestions stop if prefix of desired word is a valid word (e.g. you & youth) | https://github.com/sparrowwallet/sparrow/issues/20 | Decided this was a feature, not a bug |
| Feature | Create new electrum seed | https://github.com/sparrowwallet/sparrow/issues/59 | Isolated standard & confusing having two wordlists - Avoid | 
| Feature | Import paper wallet WIF | https://github.com/sparrowwallet/sparrow/issues/91 | many documented issues with paper wallets. It's a lot of work for a relatively niche use case. | 
