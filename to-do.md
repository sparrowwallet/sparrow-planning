# Bugs

## High Importance (Potential loss of funds)
| Type | Description | Link | Status |
| ---  | ---         | ---  | ---    |
| NA   | NA          | NA   | NA     |

## Medium Importance (Serious Frustration / Annoyance / Confusion)
| Type | Description | Link | Status |
| ---  | ---         | ---  | ---    |
| Bug | Electrum can't verify sparrow sigs | https://github.com/sparrowwallet/sparrow/issues/39 | Add note that electrum can't verify sparrow sigs | 

## Low Importance (Minor Inconvenience)
| Type | Description | Link | Status |
| ---  | ---         | ---  | ---    |
| Bug | Font  | https://github.com/sparrowwallet/sparrow/issues/19 | Upstream bug https://bugs.openjdk.java.net/browse/JDK-8236689 | 
| Bug | Slow indexing of large wallets | https://github.com/sparrowwallet/sparrow/issues/28 | Upstream issue (Electrs), ElectrumX is faster |
| Bug | Connection issues | https://github.com/sparrowwallet/sparrow/issues/29 | Server had hit max retries | 
| Bug | Tor to Non-Tor connection switch or VPN to Non-VPN switch causes issues | https://github.com/sparrowwallet/sparrow/issues/29 | Switching could restart sparrow? |

## Unclear
| Type | Description | Link | Status |
| ---  | ---         | ---  | ---    |
| Bug | Wallet in inconsistent state | https://github.com/sparrowwallet/sparrow/issues/33 | Fixed? |
| Bug | Abandoned unconfirmed tx causes crash | https://github.com/sparrowwallet/sparrow/issues/74 
| Bug | Selecting all but one UTXO does not include Other | https://github.com/sparrowwallet/sparrow/issues/115#issue-873570263 | Unclear what this bug is | 
| Bug | Scaling issue | https://github.com/sparrowwallet/sparrow/issues/117 | Unclear |
| Bug | native image camera capture library is not being loaded | https://github.com/sparrowwallet/sparrow/issues/87#issuecomment-817359279 | Lack of further information | 
| Bug | hdCapture crash | https://github.com/sparrowwallet/sparrow/issues/87 | Solved? |

-----

# Features

## High Importance (Solves a significant issue)
| Type | Description | Link | Status |
| ---  | ---         | ---  | ---    |
| Feature | Store labels | High | https://github.com/sparrowwallet/sparrow/issues/109 | Labels can be dropped if unconfirmed and tx gets dropped. Should be stored locally to avoid loosing a label. | 


## Medium Importance (Broadly Useful)
| Type | Description | Link | Status |
| ---  | ---         | ---  | ---    |
| Feature | Show hash of message when signing |  https://github.com/sparrowwallet/sparrow/issues/39 | Good idea | 
| Feature | Key rotation option on changing a keystore |  https://github.com/sparrowwallet/sparrow/issues/53#issuecomment-753321834 | Good idea |
| Feature | Custom OpReturn output when spending | https://github.com/sparrowwallet/sparrow/issues/97 | Lack of space makes this a UI challenge |
| Feature | Hex Formatting | https://github.com/sparrowwallet/sparrow/issues/99 | Good idea |
| Feature | SLIP39 (Shamir) |  https://github.com/sparrowwallet/sparrow/issues/103 | 6102 - SSKR seems more robust | 
| Feature | SSKR (Shamir) | https://github.com/sparrowwallet/sparrow/issues/103#issuecomment-821004439 | 6102 - Seems more robust https://github.com/BlockchainCommons/Research/blob/master/papers/bcr-2020-011-sskr.md | 
| Feature | Checkbox utxo selection | https://github.com/sparrowwallet/sparrow/issues/115 | Uses space, CTRL/CMD-Click works, Could be made more obvious | 
| Feature | Add AEZEED (LND) Import | https://github.com/sparrowwallet/sparrow/issues/120 | Could be useful? |

## Low Importance (Niche)
| Type | Description | Link | Status |
| ---  | ---         | ---  | ---    |
| Feature | AppImage | https://github.com/sparrowwallet/sparrow/issues/1 | .deb/.rpm/.tar.gz are available | 
| Feature | Unclear when server is connected | https://github.com/sparrowwallet/sparrow/issues/69 | Could add indication that server has successfully connected? |
| Feature | Different constants for int/ext chains | https://github.com/sparrowwallet/sparrow/issues/81 | Waiting to see if anyone else requires this functionality before merging pull |
| Feature | bip85 table | https://github.com/sparrowwallet/sparrow/issues/112 | Good idea but niche | 

## Unclear
| Type | Description | Link | Status |
| ---  | ---         | ---  | ---    |
| Feature | Trimmed QR codes | https://github.com/sparrowwallet/sparrow/issues/78 | Unclear |


## NACK'd by Craig
| Type | Description | Link | Status |
| ---  | ---         | ---  | ---    |
| Feature | bip39 word suggestions stop if prefix of desired word is a valid word (e.g. you & youth) | https://github.com/sparrowwallet/sparrow/issues/20 | Decided this was a feature, not a bug |
| Feature | Multiple schemes per wallet | https://github.com/sparrowwallet/sparrow/issues/57 | Bad fit for sparrow - use separate wallet files for each scheme |
| Feature | Create new electrum seed | https://github.com/sparrowwallet/sparrow/issues/59 | Isolated standard & confusing having two wordlists - Avoid | 
| Feature | Connect to Core with RPC not BWT | https://github.com/sparrowwallet/sparrow/issues/83 | Sparrow uses the Electrum server protocol to remain independent from the Bitcoin Core wallet. | 
| Feature | Multiple accounts in one wallet | https://github.com/sparrowwallet/sparrow/issues/92 | Using accounts to manage utxo privacy rather than labeling utxos is a very different model. |
| Feature | Import paper wallet WIF | https://github.com/sparrowwallet/sparrow/issues/91 | many documented issues with paper wallets. It's a lot of work for a relatively niche use case. | 
