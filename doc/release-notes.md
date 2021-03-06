# Asynx version 0.2.0 Release Notes

## List of Changes
* Update to C++17
* Refactor P2P message processing
* Return immediately after processing a P2P reject message
* Fix potential race condition in ActivateBestChain()
* Update Gitian build process
* Remove support for 32-bit & ARM builds
* Remove Magnetic Upgrade activation code
* Improve MSVC compatability
* Refactor block file storage
* Remove limitation on max size of block storage file, enable storage of blocks > configured max blockfile size
* Add Jenkinsfile for automated CI tests
* Refactor log messages to NET category, remove log spamming
* Remove ABC forced obsolescence code
* Update ZeroMQ library version
* Ignore unsolicited ADDR messages
* Set default tx broadcast delay to 150ms
* Add option to ignore P2P mempool requests from non-whitelisted peers
* Implementation of new mining API - RPC calls `getminingcandidate` & `submitminingsolution`
* Add CPU miner from BU for mining on test networks
* Refactor BlockAssembler, add abstract interface class
* Refactor CBlockTemplate - shared pointer for Block
* Update of license to Open BSV license
* Add capability to define network magic bytes for test networks
* Remove duplicate call to CheckBlock when validating a new block template
* Use static hasher when checking transactions
* Add capability to schedule changes to default block size parameters
* Schedule Quasar protocol upgrade
* Set default allowed size for data carrier transactions to 100kb
* Support Scaling Test Network reset
* getblock optionally returns rpc transaction details
* Fix to univalue read to mitigate memory issues. 
* New parameter (-factorMaxSendQueuesBytes) which limits total size of blocks currently in queue for sending to peers.
* Help message for "-preload" options moved to another section.
* libgen.h included unconditionally in vmtouch.cpp.
* Fixes for Mac and Windows builds.
* Minor refactoring and potential bug fixes.
* Remove Bitcoin ABC cashaddr address format.
* Increase UTXO cache default to hold the entire UTXO set in cache.
* Calls to TestBlockValidity() call are now configurable using -blockcandidatevaliditytest option.
* Support for OP_FALSE OP_RETURN as a standard transactions
* Pyhton code: Fix for array.tostring deprecated warning
* Update the OpenBSV license for Testnet/Regnet/STN

## Scaling Test Network Reset
The Scaling Test Network has been reset at block height 2951. This block has hash 
`0000000076b49c5857b2daf2b363478a799f95a18852155113bbace94321b0d0`.

# Previous Releases
* [Version 0.1.0](release-notes-v0.1.0.md) - [Source](https://github.com/Theoretix/Asynx/tree/v0.1.0) - 2018-10-15