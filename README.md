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
