# Too recent pragma version used 

## Summary 
A pragma version that is very recent can have bugs that might have gone unnoticed and also be in compatible with other chains(i.e Arbitrum)

## Vulnerability Details
Pragma version has been set to 0.8.21.The problem with this is that Arbitrum is NOT compatible with 0.8.20 and newer. Contracts compiled with those versions will result in a nonfunctional or potentially damaged version that won't behave as expected.

## Impact
Contracts compiled with those versions or newer will result in a nonfunctional or potentially damaged version that won't behave as expected.
Refer to the docs for more : https://docs.arbitrum.io/for-devs/concepts/differences-between-arbitrum-ethereum/solidity-support

## Tools Used
Manual review 

## Recommendations
Change the pragma version to some newer verison 