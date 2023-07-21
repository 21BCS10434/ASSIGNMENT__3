// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract PositiveNumberCheck {
    function checkNumber(int number) public pure returns (string memory) {
        // Use require() to check if the number is positive
        require(number > 0, "Number must be positive");
        
        // Use assert() to check if the number is less than or equal to 100
        assert(number <= 100);
        
        // If the input number is positive, return "Positive"
        return "Positive";
    }
}

