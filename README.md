//# Smart-contract-1
// Ethereum blochain smart contract 2

pragma solidity ^0.7.5;

contract trading
{
    function spot() public pure returns(string memory)
    {
        return "Cryptocurrency";
    }
}



// another way by doing global scope function calling


pragma solidity ^0.7.5;



contract trading
{
    string message = "CRYPTOCURRENCY";

    function spot() public view returns(string memory)
    {
        return message;
    }
}


// you can also do this way such that your string message box will be public and can be shown differently from your function

// SPDX-License-Identifier: MIT
pragma solidity ^0.7.5;



contract trading
{
    string public message = "CRYPTOCURRENCY";

    function spot() public view returns(string memory)
    {
        return message;
    }
}
