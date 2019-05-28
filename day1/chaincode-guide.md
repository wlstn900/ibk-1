## chaincode 가이드
- chaincode는 shim package를 이용하여 state에 접근합니다.
https://godoc.org/github.com/hyperledger/fabric/core/chaincode/shim
<br><br><br>

## chaincode의 종류
- CSCC : Configuration System Chaincode<br>
- LSCC : Life Cycle System Chaincode<br>
- QSCC : Query System Chaincode<br> 
- ESCC : Endorser System Chaincode <br>
- VSCC : Validator System Chaincode<br>
<br><br>


## chaincode 내 주요 API
- func Init :  Instantiate/Upgrade 수행시 호출<br>
- func main : Golang의 시작점<br>
- func Invoke : function을 호출하기 위한 상위 function<br>
<br><br>

## shim package 주요 API
- PutState : 저장
- GetState : 조회
- DelState : 삭제