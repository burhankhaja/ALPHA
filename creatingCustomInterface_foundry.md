**command**
```sh
forge inspect ./path/:ContractName abi --pretty > filename.sol
```

*example: let's say i wanna interface of Curves contract within path src/Curves.sol*

`forge inspect src/Curves.sol:Curves abi --pretty > ICurves.sol`
