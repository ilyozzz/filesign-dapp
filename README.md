# Filesign dApp

Decentralized app that allows to store file hashes and signatures in polkadot blockchain

Main functions:
- file creation
- auditor assignment
- signing file
- file info explorer

## Main flow

There must be at least 2 addresses: a (file) owner and auditor(s)
- owner uploads a file blob and store it's hash in the blockchain
- owner assigns auditor(s) which has an access to sign that file
- auditor signs the file

Also it's neccessary to see file info at any stage of the flow

## Quick Start

1. Run command `bash up_node.sh`
2. Run command `bash up_explorer.sh`

Run command `yarn && yarn start` for starting dev server. You also need to install polkadot browser extension for your browser for using this project: https://polkadot.js.org/extension/

You can find available node commands using node explorer via http://localhost

## Tasks

1. Implement polkadot address selection from polkadot extension and store it in localstorage (use antd selector);
2. Implement functions assignAuditor and signLatestVersion. You can use functions from src/hooks/usePolkadot as an example;
3. Create pages for showing file data, auditor assignment, creating and signing a file. Addresses for creation and signing file must be different;
4. Page for creating file should have file uploader component and be able to calculate file hash which must be saved into the blockchain.

## Bonus tasks

1. Create navigation between pages

## Tips

1. Actual polkadot-js documentation is available here: https://polkadot.js.org/docs/substrate
2. You can use polkadot explorer to test queries/extrinsics before implementing them
3. You can create any polkadot address via polkadot extension. You must have at least 2 to solve task 3
4. You can use any component from ant.design framework
