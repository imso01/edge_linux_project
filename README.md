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

## 📂 프로젝트 구조

Omok_game/
├── client/
│   ├── client               # 클라이언트 실행 파일
│   ├── Makefile             # 클라이언트 빌드 파일
│   ├── incs/                # 클라이언트 헤더
│   │   └── *.h
│   └── srcs/                # 클라이언트 소스
│       ├── client.c         # 메인 로직
│       ├── print_board.c    # 오목판 그리기
│       ├── print_result.c   # 승패 결과 출력
│       ├── print_turn.c     # 턴 정보 출력
│       ├── print_ui.c       # UI 구성
│       ├── recvData.c       # 서버에서 데이터 수신
│       ├── sendData.c       # 서버로 데이터 전송
│       └── set_info.c       # 사용자 정보 설정

├── server/
│   ├── server               # 서버 실행 파일
│   ├── Makefile             # 서버 빌드 파일
│   ├── incs/                # 서버 헤더
│   │   └── *.h
│   └── srcs/                # 서버 소스
│       ├── init.c           # 서버 초기화
│       ├── main.c           # 서버 메인
│       ├── map.c            # 오목판 상태
│       ├── startGame.c      # 게임 시작
│       ├── startTCP.c       # TCP 통신 초기화
│       └── startThread.c    # 클라이언트 쓰레드 처리


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
