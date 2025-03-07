# Welcome to MAINNET Tectum Blockchain Node v4.0 beta! #

## Description ##

Tectum Blockchain Node is a component of the Tectum blockchain designed to provide access to the functionality of the blockchain network. Anyone who downloads and runs this node becomes a full participant in the Tectum network and can take advantage of all its benefits.

The network node offers the following functionalities for participants:
1. Token management (in development).
2. Transaction processing.
3. User key management.
4. Becoming a validator.
5. Token staking.
6. Viewing blockchain chains.

## Web Server ##
Tectum Blockchain Node includes a local web server that processes requests. It provides explorer functions, allowing users to view information about blocks and transactions, as well as an interface for creating new tokens, staking tokens, becoming a validator, performing transfers, and managing keys.

## Endpoints ##

Tectum Blockchain Node supports the following types of requests:

### Coin operations: ###

-   **[POST /coins/transfer](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/tokens_transfer_request.md)**: To transfer TET between two addresses
-   **GET /coins/transfer?id=N**: Retrieve full information of transfer for the TET
-   **[GET /coins/transfers](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/token_transfer_history.md)**: Retrieve the transfer history for the TET
-   **[POST /coins/stake](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/tokens_stake_request.md)**: Staking TET to become a network validator
-   **POST /coins/migrate**: Migrate TET to new address
-   **[GET /coins/balance/byaddress](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/token_balance_request.md)**: Retrieve TET balance by address
-   **[GET /coins/transfers/user](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/tet_transfer_history_user.md)**: Retrieve the TET transfer history for a specific user

### Key management: ###

-   **[GET /keys/new](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/keys_generate_request.md)**: Generate a private/public key pair
-   **[POST /keys/recover](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/keys_recovery_request.md)**: Recover keys using a seed phrase

### Settings: ###

-   **[GET /version](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/version_request.md)**: View node version

### Blocks: ###

-   **[GET /blockscount](https://github.com/crispmindltd/tectum4-node-validator/tree/main/docs/block_count.md)**: Retrieve the total count of blocks in the blockchain

