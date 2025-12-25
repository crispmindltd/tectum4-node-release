# Welcome to MAIN NET Tectum Blockchain Node v4.1 beta! #

## Description ##

Tectum Blockchain Node is a component of the Tectum blockchain designed to provide access to the functionality of the blockchain network. Anyone who downloads and runs this node becomes a full participant in the Tectum network and can take advantage of all its benefits.

The network node offers the following functionalities for participants:
1. Token management.
2. Transaction processing.
3. User key management.
4. Becoming a validator.
5. Token staking.
6. Viewing blockchain chains.

## Web Server ##
Tectum Blockchain Node includes a local web server that processes requests. It provides explorer functions, allowing users to view information about blocks and transactions, staking tokens, becoming a validator, performing transfers, and managing keys.

Settings for web serever in `settings.ini` section `[http]`:

```
[http]
enabled=true
port=8917
```

## Endpoints ##

Tectum Blockchain Node supports the following types of requests:

### Coin operations: ###

-   **[POST /coins/transfer](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/coin_operations/POST_coins_transfer.md)**: To transfer TET between two addresses
-   **[POST /coins/transfer/create-sign](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/coin_operations/POST_coins_transfer_create_sign.md)**: Generating a signed transaction
-   **[POST /coins/transfer/sign](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/coin_operations/POST_coins_transfer_sign.md)**: Sending a signed transaction to the network
-   **[GET /coins/transfer?id=N](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/coin_operations/GET_coins_transfers_id.md)**: Retrieve full information of transfer for the TET
-   **[GET /coins/transfers](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/coin_operations/GET_coins_transfers.md)**: Retrieve the transfer history for the TET
-   **[POST /coins/stake](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/coin_operations/POST_coins_stake.md)**: Staking TET to become a network validator
-   **[POST /coins/unstake](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/coin_operations/POST_coins_unstake.md)**: Withdrawal of funds from staking
-   **[POST /coins/migrate](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/coin_operations/POST_coins_migrate.md)**: Migrate TET to new address
-   **[GET /coins/balance/byaddress](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/coin_operations/GET_coins_balance_byAddress.md)**: Retrieve TET balance by address
-   **[GET /coins/transfers/user](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/coin_operations/GET_coins_transfers_user.md)**: Retrieve the TET transfer history for a specific user

### Token operations: ###

- **[GET /token/balance/byaddress](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/coin_operations/GET_token_balance_byAddress.md)**: Get the token balance by the cryptocurrency address
- **[POST /token/mint](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/coin_operations/POST_token_mint.md)**: Creating a new token
- **[POST /token/burn](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/coin_operations/POST_token_burn.md)**: Burn a liquidity token
- **[GET /token/info](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/coin_operations/GET_token_info.md)**: Getting token information by ticker
- **[POST /token/transfer](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/coin_operations/POST_token_transfer.md)**: Transfer tokens between two cryptocurrency addresses

### Key management: ###

-   **[GET /keys/new](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/key_management/GET_keys_generate.md)**: Generate a private/public key pair
-   **[POST /keys/recover](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/key_management/POST_keys_recovery.md)**: Recover keys using a seed phrase

### Settings: ###

-   **[GET /version](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/settings/GET_version_request.md)**: View node version
-   **[GET /net](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/settings/GET_archivers_info.md)**: Getting information about archivers

### Blocks: ###

-   **[GET /blockscount](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/blocks/GET_blocks_count.md)**: Retrieve the total count of blocks in the blockchain
-   **[GET /blocks]**: Retrieve the array of blocks
