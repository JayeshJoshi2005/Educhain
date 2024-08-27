# Blockchain-Based Property Registration

<a href="LICENSE"><img src="https://img.shields.io/static/v1?label=license&message=MIT&color=green"></a>
<img src="https://img.shields.io/badge/Ethereum-20232A?style=for-the-badge&logo=ethereum&logoColor=white">
<img src="https://img.shields.io/badge/Flutter-%2302569B.svg?style=for-the-badge&logo=Flutter&logoColor=white">

## Overview
This project provides a decentralized solution for land registration using blockchain technology. It addresses the following issues:
1. **Elimination of Middlemen**: Reduces costs and fraud by removing brokers and speeding up the registration process.
2. **Tamper-Proof Ledger**: Utilizes a distributed ledger to prevent ownership fraud.
3. **Secure Document Storage**: Stores important property registration documents securely using IPFS.

## Technology Stack
- Ethereum Blockchain
- Polygon/Matic
- Web3Dart
- IPFS
- Flutter
- Metamask

## Demo
Watch a demonstration of our Dapp [here](https://www.youtube.com/watch?v=IMkCFsI3ePA).



## Running Locally
1. Clone the repository and navigate to the project folder.
2. Install Flutter 3.0.2 and Node.js.
3. Install Ganache and Truffle:
   ```bash
   npm install -g truffle
   ```
4. Run Ganache in the background.
5. Install the Metamask Chrome extension, select the local network, and import the accounts.
6. Compile and deploy migrations:
   ```bash
   truffle compile
   truffle migrate
   ```
7. Update the `constant.dart` file with the new contract address:
   ```text
   contract address: 0xed690C24C60A48F8A9819c9A15AD75B70CFBEa5a
   ```
   Set `chainId` to `'1337'` and `rpcUrl` to `"http://127.0.0.1:7545"`.
8. Run the Flutter web app:
   ```bash
   flutter pub get
   flutter run -d web-server --web-port 5555
   ```
9. Access the Dapp at [http://localhost:5555/](http://localhost:5555/).
10. Obtain a Mapbox API key from [Mapbox](https://www.mapbox.com/) and replace the `mapBoxApiKey` in the `constant.dart` file.

## Project Flowchart
<img src="screenshots/flowchart.png" height="450">

## Screenshots
- **Home Page** | **Wallet Connect/Login**
  <img src="screenshots/Screenshot1.png" height="225"> | <img src="screenshots/Screenshot7.png" height="225">
- **Contract Owner Dashboard** | **User Registration**
  <img src="screenshots/Screenshot10.png" height="225"> | <img src="screenshots/Screenshot12.png" height="225">
- **Land Inspector Dashboard** | **User Verification**
  <img src="screenshots/Screenshot11.png" height="225"> | <img src="screenshots/Screenshot5.png" height="225">
- **User Dashboard** | **Adding Land on Map**
  <img src="screenshots/Screenshot2.png" height="225"> | <img src="screenshots/Screenshot8.png" height="225">
- **Land Gallery** | **Land Details**
  <img src="screenshots/Screenshot3.png" height="225"> | <img src="screenshots/Screenshot9.png" height="225">
- **Received Request** | **Make Payment**
  <img src="screenshots/Screenshot6.png" height="225"> | <img src="screenshots/Screenshot4.png" height="225">
- **Transfer Ownership/Seller/Buyer Photo Capture** | **Witness Info/Photo Capture/Transfer Ownership**
  <img src="screenshots/Screenshot14.png" height="225"> | <img src="screenshots/Screenshot13.png" height="225">