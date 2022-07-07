# TON Wallet Smart Contracts Collection

We created a collection of well-known smart wallets to make it easy for users and developers to navigate through them. The root of the repository contains directories with the names of such contracts, and they in turn contain versions directories in sequential versioning format (i.e. `v1`, `v2`, `v3` etc.). Each version can contain revision directories(i.e. `r0`, `r1`, `r2` etc.). 

If a contract has more than one revision, its initial representation automatically becomes `r0`. Initial version of the contract `v1` (may be missing, because most wallet contracts were developed a long time ago)

Also the final directory of the contract has its own license and `README.md` files, and can be considered as a separate repository. We did not include deprecated contracts or non-secure contracts(in our view) in the repository.

Due to the fact that some third-party repositories with wallet contracts are poorly structured, we added our own description to them, some fift scripts and decomposed the files into the necessary repositories so that it would be easier for you to work with them. We don't change the FunC/Fift-ASM contracts code.

## Navigation

### `wallet`
| version | revision | src                                                |
|---------|----------|----------------------------------------------------|
| `v3`    | `r0`     | [`/wallet/v3/r0/`](wallet/v3/r0/)                  |
| `v3`    | `r2`     | [`/wallet/v3/r2/`](wallet/v3/r2/)                  |

### `highload-wallet`
| version | revision | src                                                |
|---------|----------|----------------------------------------------------|
| `v2`    | `-`      | [`/highload-wallet/v2/`](highload-wallet/v2/)      |

## Feedback

If you find a problem, or want to include your own version of the wallet, or noticed a copyright violation, or you have another reason for feedback, please just create [an issue.](https://github.com/tonstack/wallet-smcs/issues)

## Disclaimer of liability

This is a repository with repositories. TonStack assumes no responsibility for the content of user contracts and their security. You use these contracts at your own risk.

Despite this, we take a responsible approach to the addition of this repository, most of the contracts (or even all) presented here are developed by TON himself or our team.
