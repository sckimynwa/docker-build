# Docker Build

Docker Build Source For Kubernetis Study

## 빌드

- Build Directory
- Image Tag

## 목록

- [echo](./echo): 접속한 서버 정보를 json으로 리턴 (3000포트)
- [counter](./counter): 접속할 때마다 Counter 1씩 증가 (Redis 사용)

```
docker run --rm -p 3000:3000 ghcr.io/yeoul/echo
curl localhost:3000
```
