# Project Title

Simple overview of use/purpose.
This projects will check if the value you enter was an error and approve if was correct.  

## Description

it uses to set a value of a number that has a start value which is 10 and has a end value of 1000

## Getting Started

### Installing
 How/where to download your program
 Any modifications needed to be made to files/folders
* go to https://remix.ethereum.org/
* create an account
* make a folder
* create a code

### Executing program

How to run the program
  Step-by-step bullets
* create a code
* compile it
* deploy
* check if it's running
```
code blocks for commands
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.25;
contract SmartContract {
    uint public value;
    function setValue(uint256 _newValue) external {
        require(_newValue >= 10 && _newValue <= 1000, "You can only enter up to 10 but cannot be above 1000");
        value = _newValue;
    }
    function assertValue(uint256 _num) external pure returns (uint256) {
        assert(_num >= 10 && _num <=1000);
        return _num;
    }
    function revertValue(uint256 _num) external pure returns (uint256) {
        if (_num >= 10 && _num <= 1000) {
            revert("Value must between 10 and 1000");
        }
        return _num;
    }
}
```

## Help
