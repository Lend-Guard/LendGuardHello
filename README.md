# LendGuardHello
Welcome to the comprehensive documentation for the LendGuard Protocol—a personalized guardian for lending protocols in the DeFi space. LendGuard empowers users to configure their security preferences, set health factors, notification thresholds, and deploy custom guards for enhanced security while managing lending activities hassle-free.

http://lendguard.xyz

## Navigation
- [**LendGuard**](https://github.com/Lend-Guard/LendGuard) - Contains the core contracts powering LendGuard's functionalities.
- [**LendGuardOracle**](https://github.com/Lend-Guard/LendGuardOracle) - he keeper module responsible for monitoring guards. Users can fork it and customize it for their specific keeper implementation in the Guard's contract.
- [**LendGuardDApp**](https://github.com/Lend-Guard/LendGuardDapp) - Backend and frontend components for the LendGuard application.

## Key concepts
- Target Health Factor - The Target Health Factor (THF) signifies the health factor within a lending protocol, serving as the base for all threshold calculations. For example, if you set `THF=1.5` and configure a notification alert at 10%, the alert will trigger at `1.1 * 1.5` = 1.65 HF.
- Guard - A Guard refers to the specific contract configured and deployed by a user. It plays a pivotal role in managing positions and executing keeper-related actions.
- Keeper/Oracle - The Keeper or Oracle is an off-chain program responsible for monitoring Guards and executing pre-approved deposits or repayments for selected tokens.
- Push Notification - LendGuard utilizes the [Push Protocol's](https://app.push.org/) notification system, which the Keeper employs to send alerts and notifications to users.

## Deployed contracts

### Arbitrum Mainnet
- Implementation: 0x4b325C41e1DaC67b068FF7c476fb794AC7e136C6
- GuardFactory: 0x272Ded7510786F266a3C1D8D0ad0EaCcA308B593
- Push Channel: Cooming Soon!

### Arbitrum Testnet Goerli
- Implementation: 0x2895Bd93d452A55A0963E2B8d845e1D197759871
- GuardFactory: 0x400765A72458D7f33F5d19369C63d45b999Dacf1
- Push Channel: 0x03db46E504fe334200bfa77DC0C0D6f411253B70
