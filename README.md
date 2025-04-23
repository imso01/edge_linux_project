# 🕹️ 오목 게임 (Omok Game)

**리눅스 프레임버퍼 + 클라이언트-서버 구조 기반의 임베디드 오목 게임**

---

## 📌 프로젝트 소개

이 프로젝트는 C 언어를 기반으로 한 **4목 규칙의 오목 게임**입니다.  
프레임버퍼를 활용한 UI 기반 렌더링과, 클라이언트-서버 모델을 통해 **양방향 플레이**가 가능합니다.  
리눅스 환경에서 네트워크 통신 및 실시간 입력 처리를 경험할 수 있도록 설계되었습니다.

---

## 🛠️ 사용 기술 및 환경

- **Language:** C
- **Platform:** Linux (Framebuffer, Socket)
- **Protocol:** TCP/IP
- **Tool:** GCC, Makefile

---

## ✅ 실행 방법

### 1. 서버 실행
```bash
make server
./server
```
### 2. 클라이언트 실행
```bash
make client
./client
```
