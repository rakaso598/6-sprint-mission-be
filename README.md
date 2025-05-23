## 프로젝트 작업 내역 (날짜별, 시간별 정리)

**2025년 05월 09일 (금)**

- (미정) Multer 설정 완료 (`app.js`).
- (미정) MVC (Model-View-Controller) 패턴 기반 API 서버 구축 목표 설정 (controllers/services/models).
- (미정) **컨트롤러:** Request 수신 및 에러 처리 확인 (request-response 동작 확인, 로직 오류 가능성 존재).
- (미정) **DB 연결:** Prisma Studio (포트 5555)를 통한 DB 구조 및 CRUD 기능 확인 완료.
- (미정) **API 테스트:**
  - (미정) `GET http://localhost:3000/articles/:id`를 통한 특정 게시물 조회 및 없는 목록 조회 기능 확인 완료.
  - (미정) "Please authenticate" 메시지를 통해 게시물 등록 시 인증/인가 구현 필요성 확인.
- (미정) **인증/인가:** 회원가입 및 로그인 후 획득한 토큰을 사용하여 게시물 등록 기능 구현 완료 (auth.middleware.js 사용).
- (미정) **MVC 패턴 개선:**
  - (미정) 기존 컨트롤러에 집중된 로직 분리 필요성 인식.
  - (미정) Prisma 클라이언트 관련 코드를 **model 레이어**로 이동 계획.
  - (미정) **컨트롤러 레이어:** 사용자 요청 수신, 서비스 레이어 호출 및 응답 처리 집중.
  - (미정) **서비스 레이어:** 컨트롤러로부터 전달받은 데이터 활용, 모델 레이어 호출 (기본 형태).
  - (미정) 추가적인 서비스 로직은 서비스 레이어에 작성 계획.
  - (미정) Request 처리 흐름 구체화: `routes (미들웨어 적용) -> controller -> service -> model`.
- (미정) **Express MVC 구조 명확화:**
  - (미정) **routes Layer:** 엔드포인트 정의 및 컨트롤러 연결 (미들웨어 적용 가능).
  - (미정) **controller Layer:** routes 호출 처리, service Layer 호출.
  - (미정) **service Layer:** controller 호출 처리, model Layer 호출.
  - (미정) **model Layer:** Prisma 클라이언트 활용, DB 요청 및 응답 처리.

**2025년 05월 12일 (월)**

- (미정) HTTP 파일 작성 및 필요한 API (product) 우선 작성 후 테스트 및 MVC 분리 진행 계획.
- (미정) 상품 등록 및 조회 API의 MVC 패턴 분리 완료 (등록 기능 포함).
- (미정) Conventional Commits 확장 사용 경험: 커밋 메시지 작성 편의성 향상 (긍정적).
- (미정) **다음 작업:** 상품 수정/삭제 API 진행 및 프론트엔드 연동 필요성 검토 (구현 요구사항 문서 확인).
- (오후 13:30) 상품 수정/삭제 API 진행 및 테스트 완료. 프론트엔드 기능 연결 여부 확인 위해 구현 요구사항 문서 검토 필요.
