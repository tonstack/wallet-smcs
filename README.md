## TON Wallet Smart Contracts Collection

We created a collection of well-known smart wallets to make it easy for users and developers to navigate through them. The root of the repository contains directories with the names of such contracts, and they in turn contain versions directories in sequential versioning format (i.e. `v1`, `v2`, `v3` etc.). Each version can contain revision directories(i.e. `r1`, `r2`, `r3` etc.). 

If a contract has more than one revision, its initial representation automatically becomes `r1`. Initial version of the contract `v1` (may be missing, because most wallet contracts were developed a long time ago)

Also the final directory of the contract has its own license and `README.md` files, and can be considered as a separate repository. We did not include deprecated contracts or non-secure contracts(in our view) in the repository.

## Navigation

## Feedback

If you find a problem, or want to include your own version of the wallet, please create [an issue.](https://github.com/tonstack/wallet-smcs/issues) 