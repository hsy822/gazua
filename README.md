# gazua

## How to start
- 테스트 네트워크 구성
- > npm install -g ethereumjs-testrpc
- 임의의 계정 10개와 각 개정마다 100ETH 생성
- > testrpc
- localhost:8545 listening

## Smart-contract 사용시
- Remix 이용 배포
- http://remix.ethereum.org

-sample code
'''
pragma solidity ^0.4.0;

contract SimpleStorage {
    uint storedData;

    function set(uint x) public{
        storedData = x;
    }

    function get() public constant returns (uint) {
        return storedData;
    }

}
'''

- run -> environment : web3 providers -> endpoint : http://localhost:8545
