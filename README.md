# Hercules DEX Default Token-List Repository

Welcome to the Hercules DEX Default Token-List repository! This repository contains a list of tokens supported by the Hercules decentralized exchange. If you would like to add a new token to the list, please follow the instructions below.

## Adding a New Token

First you need to create a new branch

```bash
git branch -m "listing/<your token symbol>"
```

------------


To add a new token to the Hercules DEX token list, please open a pull request to the main branch of this repository. Follow the steps outlined below to ensure your token is added correctly:

1. Open the `src/tokens/metis-andromeda.json` file.
2. Add your token information at the end of the file in the following format:

```json
{
  "chainId": 1088,
  "symbol": "SYMBOL",
  "name": "Token name",
  "address": "0x0000000000000000000000000000000000000000",
  "logoURI": "BASE_URL/assets/<your token logo image name>.(svg|png)",
  "decimals": 0,
  "isWNative": false,
  "quote": "native"
}
```

Replace the placeholders `SYMBOL`, `Token name`, `0x0000000000000000000000000000000000000000` and `<your token logo image name>` with the appropriate information for your token.

3. Ensure you provide the correct `chainId`, `symbol`, `name`, `address`, `decimals`, `isWNative`, and `quote` for your token.

4. Upload your token logo to the `src/assets` directory and reference it in the `logoURI` field.

5. Submit your changes as a pull request to the main branch of this repository with the pull request with your branch.


## Guidelines for Token Submission

- Please ensure that the token information provided is accurate and up-to-date.
- Tokens should adhere to the ERC-20 standard.
- Token logos should be in SVG or PNG format and have a transparent background.

Thank you for contributing to the Hercules DEX token list! If you have any questions or need assistance, feel free to reach out to us.

## Disclaimer

Note opening pull request does not guarantee addition to this default token list.
We do not review token addition requests in any particular order, and we do not
guarantee that we will review your request to add the token to the default list."