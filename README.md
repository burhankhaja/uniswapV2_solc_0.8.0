## Disclaimer
**`These smart contracts are being provided as the refactored versions of uniswapV2 core contracts. No guarantee, representation or warranty is being made, expressed or implied, as to the safety or correctness of the user interface or the smart contracts. They have not been audited and as such there can be no assurance they will work as intended, and users may experience delays, failures, errors, omissions, loss of transmitted information or loss of funds. The creators are not liable for any of the foregoing. Users should proceed with caution and use at their own risk.`**

## Acknowledgements
- [**`uniswap`**](https://github.com/Uniswap) 
- [**`v2-core`**](https://github.com/Uniswap/v2-core/tree/master/contracts)


## About

- These smart contracts are the refactored versions of uniswap v2-core contracts.
- I have changed the older version to 0.8.0 and refactored accordingly
- **`Things that i have modified from original codebase to make it solc_0.8.0 compatible are`**:
  - assembly based chainId updation to *block.chainid*
  - removed duplicate interface declarations to avoid inheritance conflicts
  - Adding *override* identifier to overriding functions, *not required in older versions*
  - changed type conversion of uint(-1) to type(uint256).max, *though you could also change it to uint(int(-1))* <br>

  
**`I don't guarentee i have only changed these components, may be i have forgotten to mention so I take no responsibility`**


## Agenda
- Only reason i refactored it is for only educational purposes.
- I was learning indepth about uniswapV2 but I had lot of issues while unit testing original [**`v2-core`**](https://github.com/Uniswap/v2-core/tree/master/contracts) using foundry.
- There were lot of things constantly breaking. Even a small change led to chain of whole different errors.
- So i thought why not refactor it to higher versions like 0.8.0 to make it easily testable. <br>
**`Your only goal while using it should be to learn uniswapv2 easily using foundry. Do not use these contracts in production, there can be lot of covert bugs, one of them may be shadowed function type issues have arisen due to refactoring, so i don't guarentee anything.`**

## FOLLOW ME ON X
[**`@burhan_khaja`**](https://twitter.com/burhan_khaja)

