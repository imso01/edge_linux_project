🕹️ 오목 게임 (Omok Game)
리눅스 프레임버퍼 + 클라이언트-서버 구조 기반의 임베디드 오목 게임

📌 프로젝트 소개
이 프로젝트는 C 언어를 기반으로 한 4목 규칙의 오목 게임입니다.
프레임버퍼를 활용한 UI 기반 렌더링과, 클라이언트-서버 모델을 통해 양방향 플레이가 가능합니다.
리눅스 환경에서 네트워크 통신 및 실시간 입력 처리를 경험할 수 있도록 설계되었습니다.

🛠️ 사용 기술 및 환경
Language: C

Platform: Linux (Framebuffer, Socket)

Protocol: TCP/IP

Tool: GCC, Makefile

📂 프로젝트 구조
bash
복사
편집
omok-game/
├── server.c          # 서버 실행 및 클라이언트 연결 처리
├── client.c          # 클라이언트 실행 및 사용자 입력 전송
├── board.c           # 오목판 렌더링 및 상태 관리
├── input.c           # 사용자 입력 처리
├── win_check.c       # 승리 조건 확인
├── framebuffer.c     # 프레임버퍼 출력 처리
├── common.h          # 공용 헤더 정의
├── Makefile          # 빌드 자동화
└── README.md         # 프로젝트 설명서
✅ 실행 방법
1. 서버 실행
bash
복사
편집
make server
./server
서버가 실행되면, 클라이언트의 접속을 기다립니다.

2. 클라이언트 실행
bash
복사
편집
make client
./client
클라이언트가 서버에 접속하여 게임을 시작합니다.
프레임버퍼를 통해 오목판 UI가 화면에 출력됩니다.
