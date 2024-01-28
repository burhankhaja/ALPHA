## how to get the storage slot layout of contract?

```c
solc --storage-layout path_to_file.sol
```

## applications
__`private variables are not accessed on inheritence, you can use assembly with storage layout to workaround`__



```
pragma solidity 0.8.21;

contract one {
 uint number = 4;
 uint private num = 7;
}

contract two is one {
 function getNumberFromOne() public view returns(uint) {
    uint num;
    assembly {
      num := sload(1)
    }
    return num;
 }
}
```
