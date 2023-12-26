
# DODO V3 update contest details

- Join [Sherlock Discord](https://discord.gg/MABEWyASkp)
- Submit findings using the issue page in your private contest repo (label issues as med or high)
- [Read for more details](https://docs.sherlock.xyz/audits/watsons)

# Q&A

### Q: On what chains are the smart contracts going to be deployed?
mainnet, Arbitrum, Optimism, BNB, Polygon
___

### Q: Which ERC20 tokens do you expect will interact with the smart contracts? 
any
___

### Q: Which ERC721 tokens do you expect will interact with the smart contracts? 
none
___

### Q: Do you plan to support ERC1155?
no
___

### Q: Which ERC777 tokens do you expect will interact with the smart contracts? 
none
___

### Q: Are there any FEE-ON-TRANSFER tokens interacting with the smart contracts?

none
___

### Q: Are there any REBASING tokens interacting with the smart contracts?

no
___

### Q: Are the admins of the protocols your contracts integrate with (if any) TRUSTED or RESTRICTED?
RESTRICTED
___

### Q: Is the admin/owner of the protocol/contracts TRUSTED or RESTRICTED?
TRUSTED
___

### Q: Are there any additional protocol roles? If yes, please explain in detail:
No
___

### Q: Is the code/contract expected to comply with any EIPs? Are there specific assumptions around adhering to those EIPs that Watsons should be aware of?
No
___

### Q: Please list any known issues/acceptable risks that should not result in a valid finding.
none
___

### Q: Please provide links to previous audits (if any).
https://audits.sherlock.xyz/contests/89
___

### Q: Are there any off-chain mechanisms or off-chain procedures for the protocol (keeper bots, input validation expectations, etc)?
No
___

### Q: In case of external protocol integrations, are the risks of external contracts pausing or executing an emergency withdrawal acceptable? If not, Watsons will submit issues related to these situations that can harm your protocol's functionality.
No
___

### Q: Do you expect to use any of the following tokens with non-standard behaviour with the smart contracts?
Missing Return Values
Upgradable Tokens
Tokens with Blocklists
___

### Q: Add links to relevant protocol resources
none
___



# Audit scope


[dodo-v3 @ 78c5cb6ea2fb1cd8ee675a1cebcaf6332faaf99a](https://github.com/DODOEX/dodo-v3/tree/78c5cb6ea2fb1cd8ee675a1cebcaf6332faaf99a)
- [dodo-v3/contracts/DODOV3MM/D3Pool/D3Funding.sol](dodo-v3/contracts/DODOV3MM/D3Pool/D3Funding.sol)
- [dodo-v3/contracts/DODOV3MM/D3Pool/D3MM.sol](dodo-v3/contracts/DODOV3MM/D3Pool/D3MM.sol)
- [dodo-v3/contracts/DODOV3MM/D3Pool/D3Maker.sol](dodo-v3/contracts/DODOV3MM/D3Pool/D3Maker.sol)
- [dodo-v3/contracts/DODOV3MM/D3Pool/D3Storage.sol](dodo-v3/contracts/DODOV3MM/D3Pool/D3Storage.sol)
- [dodo-v3/contracts/DODOV3MM/D3Pool/D3Trading.sol](dodo-v3/contracts/DODOV3MM/D3Pool/D3Trading.sol)
- [dodo-v3/contracts/DODOV3MM/D3PoolNoBorrow/D3MMNoBorrow.sol](dodo-v3/contracts/DODOV3MM/D3PoolNoBorrow/D3MMNoBorrow.sol)
- [dodo-v3/contracts/DODOV3MM/D3PoolNoBorrow/D3MakerFreeSlot.sol](dodo-v3/contracts/DODOV3MM/D3PoolNoBorrow/D3MakerFreeSlot.sol)
- [dodo-v3/contracts/DODOV3MM/D3Vault/D3Vault.sol](dodo-v3/contracts/DODOV3MM/D3Vault/D3Vault.sol)
- [dodo-v3/contracts/DODOV3MM/D3Vault/D3VaultFunding.sol](dodo-v3/contracts/DODOV3MM/D3Vault/D3VaultFunding.sol)
- [dodo-v3/contracts/DODOV3MM/D3Vault/D3VaultLiquidation.sol](dodo-v3/contracts/DODOV3MM/D3Vault/D3VaultLiquidation.sol)
- [dodo-v3/contracts/DODOV3MM/D3Vault/D3VaultStorage.sol](dodo-v3/contracts/DODOV3MM/D3Vault/D3VaultStorage.sol)
- [dodo-v3/contracts/DODOV3MM/D3Vault/Errors.sol](dodo-v3/contracts/DODOV3MM/D3Vault/Errors.sol)
- [dodo-v3/contracts/DODOV3MM/D3Vault/periphery/D3PoolQuota.sol](dodo-v3/contracts/DODOV3MM/D3Vault/periphery/D3PoolQuota.sol)
- [dodo-v3/contracts/DODOV3MM/D3Vault/periphery/D3RateManager.sol](dodo-v3/contracts/DODOV3MM/D3Vault/periphery/D3RateManager.sol)
- [dodo-v3/contracts/DODOV3MM/D3Vault/periphery/D3Token.sol](dodo-v3/contracts/DODOV3MM/D3Vault/periphery/D3Token.sol)
- [dodo-v3/contracts/DODOV3MM/D3Vault/periphery/D3UserQuota.sol](dodo-v3/contracts/DODOV3MM/D3Vault/periphery/D3UserQuota.sol)
- [dodo-v3/contracts/DODOV3MM/lib/CloneFactory.sol](dodo-v3/contracts/DODOV3MM/lib/CloneFactory.sol)
- [dodo-v3/contracts/DODOV3MM/lib/DODOMath.sol](dodo-v3/contracts/DODOV3MM/lib/DODOMath.sol)
- [dodo-v3/contracts/DODOV3MM/lib/DecimalMath.sol](dodo-v3/contracts/DODOV3MM/lib/DecimalMath.sol)
- [dodo-v3/contracts/DODOV3MM/lib/Errors.sol](dodo-v3/contracts/DODOV3MM/lib/Errors.sol)
- [dodo-v3/contracts/DODOV3MM/lib/InitializableOwnable.sol](dodo-v3/contracts/DODOV3MM/lib/InitializableOwnable.sol)
- [dodo-v3/contracts/DODOV3MM/lib/MakerTypes.sol](dodo-v3/contracts/DODOV3MM/lib/MakerTypes.sol)
- [dodo-v3/contracts/DODOV3MM/lib/PMMPricing.sol](dodo-v3/contracts/DODOV3MM/lib/PMMPricing.sol)
- [dodo-v3/contracts/DODOV3MM/lib/PMMRangeOrder.sol](dodo-v3/contracts/DODOV3MM/lib/PMMRangeOrder.sol)
- [dodo-v3/contracts/DODOV3MM/lib/Types.sol](dodo-v3/contracts/DODOV3MM/lib/Types.sol)
- [dodo-v3/contracts/DODOV3MM/periphery/D3MMFactory.sol](dodo-v3/contracts/DODOV3MM/periphery/D3MMFactory.sol)
- [dodo-v3/contracts/DODOV3MM/periphery/D3MMLiquidationRouter.sol](dodo-v3/contracts/DODOV3MM/periphery/D3MMLiquidationRouter.sol)
- [dodo-v3/contracts/DODOV3MM/periphery/D3Oracle.sol](dodo-v3/contracts/DODOV3MM/periphery/D3Oracle.sol)
- [dodo-v3/contracts/DODOV3MM/periphery/D3Proxy.sol](dodo-v3/contracts/DODOV3MM/periphery/D3Proxy.sol)


