# GIPs

GEB Improvement Proposals (GIPs) describe standards for the Generalized Ethereum Bonds framework, including the current implementation of RAI, future reflex bond R&D, client APIs and keeper upgrades.

# Contributing

 1. Review [GIP-1](GIPS/gip-1.md).
 2. Fork the repository by clicking "Fork" in the top right.
 3. Add your GIP to your fork of the repository. There is a [template GIP here](gip-X.md).
 4. Submit a Pull Request to Reflexer's [GIPs repository](https://github.com/reflexer-labs/GIPs).

# GIP Statuses

 * **DRAFT** - a GIP that is still being developed.
 * **LAST CALL** - a GIP that is done with its initial iteration and ready for review by a wide audience.
 * **DELAYED** - a GIP will be re-analyzed after the core team deploys the first GEB on mainnet Ethereum. This is a temporary step that will be removed after the first production system is up and running. It is also here in order to focus discussion on *Core GIP Areas* (described below) and allow the core team to allocate their resources in an efficient way (pre-mainnet).
 * **APPROVED** - a core GIP that has been in Last Call for at least 3 weeks and any technical changes that were requested have been addressed by the author. The process for the core team to decide whether to add a GIP to the larger GEB framework is not part of the GIP process. If such a decision is made, the GIP will be Implemented.
 * **IMPLEMENTED** - a GIP that has been released to mainnet.
 * **REJECTED** - a GIP that has been rejected.

# Core GIP Areas

 * **PID Control** - designs and ideas about how to implement an on-chain PI/D controller
 * **Collateral Auctions / Liquidations** - capital efficient auction & liquidation engines for CDPs
 * **Oracle Design** - sustainable (paying for themselves) and hard to manipulate oracle mechanisms
 * **RAI Liquidity** - mechanisms for incentivizing RAI liquidity
