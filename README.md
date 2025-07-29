# Online BTC Wallet

This project is a minimal demonstration of a web-based Bitcoin wallet that allows users to sign in with a Google account. The wallet is generated in the browser and encrypted using the Google ID token. No backend is required to get started.

## Running Locally

1. Obtain a Google OAuth Client ID for a Web application.
2. Replace `YOUR_GOOGLE_CLIENT_ID` in `index.html` with the client ID from step 1.
3. Open `index.html` in a modern browser.

Upon signing in, a new Bitcoin wallet (BIP39 mnemonic) is generated and stored encrypted in `localStorage`. On subsequent logins with the same Google account, the wallet is decrypted and reused. The page displays the first Native SegWit (P2WPKH) address derived from the wallet.

This repository intentionally keeps the implementation simple so it can be extended later with transaction creation, balance checks, and optional backend services.
