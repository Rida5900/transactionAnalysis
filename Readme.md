# Transaction Analysis

This repository is a technical guide and transaction analysis for the [SUN.io](https://sun.io/) protocol on the TRON network. SUN.io is the leading DeFi platform on TRON, encompassing core modules such as SunSwap (V1/V2/V3), Curve, and SunPump.

The project provides developers with detailed contract addresses, event, ABIs, and transaction logic analysis to facilitate efficient integration and analysis of on-chain data.

---

## 📂 Directory Structure

| File / Directory | Description |
| :--- | :--- |
| `ABIs/` | Contains contract ABI files for SunSwap (V1/V2/V3/Curve), and Smart Routers. |
| `Events_For_Liquidity_And_Exchange.md` | Covers contract addresses, liquidity change events, and transaction examples. |
| `Sunpump Contracts.md` | Details contract addresses, function interfaces, and call examples for the SunPump protocol (Bonding Curve stage). |
| `How_to_get_all_pools.md` | Explains how to traverse Factory contracts to retrieve all pair pool addresses. |
| `RPC_Info.md` | RPC configuration information for TRON network nodes. |
| `Pool_Page.md` | Pool Information Page. |

---

## 🛠 Core Content Explanation

### 1. Events_For_Liquidity_And_Exchange
This section provides an in-depth look at contract interactions and liquidity dynamics for SunSwap (V1/V2/V3) and Smart Routers:

- **Version Support**:
  - **V1**: Includes Factory addresses and event analysis for adding/removing liquidity.
  - **V2**: Includes Router and Factory addresses, supporting TRC20-TRC20 pairs.
  - **V3**: Provides addresses for Factory, Router, and NFT Position Manager.
  - **Curve**: Covers current and historical contract addresses for various stablecoin pools (e.g., USDD, USDT).

> [View Detailed Document: Events_For_Liquidity_And_Exchange.md](./Events_For_Liquidity_And_Exchange.md)

### 2. Sunpump Contracts
This document records the contract interfaces and invocation logic for the SunPump protocol during the Bonding Curve stage and after DEX listing:

- **LaunchpadProxy** Core Functions:
  - `createAndInitPurchase`: This function allows the creation of a new token and immediately initiates a purchase of the token.
  - `purchaseToken` / `saleToken`: Buying and selling tokens.
- **Helper Functions**:
  - `getPrice`: Retrieve the current price of the token in TRX.
  - `getTokenAmountByPurchaseWithFee`: This function estimates the token amount you will receive and the associated fee when purchasing tokens.
  - `getTrxAmountBySaleWithFee`: This function estimates the TRX amount you will receive and the associated fee when selling a specific amount of tokens.
- **Code Examples**: Provides complete JavaScript examples using `tronweb` for contract interaction.

> [View Detailed Document: Sunpump Contracts.md](./Sunpump%20Contracts.md)

---

## 📚 Other Reference Guides

For the following topics, please refer directly to the respective files for detailed information:

- **3. How to Get All Pools**: [How_to_get_all_pools.md](./How_to_get_all_pools.md)  
  Explains the traversal of Factory contracts to list all trading pair addresses.
- **4. RPC Node Information**: [RPC_Info.md](./RPC_Info.md)  
  API node configurations.
- **5. Pool Page Description**: [Pool_Page.md](./Pool_Page.md)  
  Pool Information Page.

---

## 🔗 Related Resources
- **Official Website**: [SUN.io](https://sun.io/)
- **Blockchain Explorer**: [TRONSCAN](https://tronscan.org/)
- **Developer Documentation**: [SUN.io Docs](https://docs.sun.io/)

---

