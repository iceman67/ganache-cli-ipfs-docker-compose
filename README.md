# Truffle Ganache docker-compose

docker-compose 를 사용하여  [ganache-cli](https://github.com/trufflesuite/ganache-cli)  구동 확인 


```bash
git clone https://github.com/digitaldonkey/ganache-cli-docker-compose.git
docker-compose up
```

Truffle Ganache client 관련 디렉토리 `ganache_data` (블록체인자료 유지) 

`truffle.js` config 내용확인 필요 

```javascript
module.exports = {
  networks: {
    development: {
      host: '192.168.99.100',
      port: 8545,
      network_id: '5777'
    }
  }
}
```

동작 docker-compose 종료 

# IPFS 추가 
- Truffle Ganache docker-compose.yml 에 IPFS 반영
- data 디렉토리에 ipfs 구성이 이루어짐

```
docker-compose up
```

ipfs와 ganache 동작 확인

