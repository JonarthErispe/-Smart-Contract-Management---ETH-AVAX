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

// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract ErrorHandling {
   uint256 public value;    
    function setValue(uint256 _value) public {
        require(_value > 100, "Value must be greater than 100.");
        value = _value;
    }

    function doubleValue() public {
        uint256 oldValue = value;
        value = value * 2;
        assert(value == oldValue * 2);
    }
    
    function resetValue() public {
        if (value == 100) {
            revert("Value is already 100.");
        }
        value = 0;
    }
}

        return _num;
    }
}
```

## Help
