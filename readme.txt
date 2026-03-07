================================================================
  AI기반 공감 지도 (Empathy Map) 생성기
  나눔경영컨설팅
================================================================

[프로젝트 개요]
회사명, 제품/서비스, 고객 페르소나를 입력하면 AI(Claude)가
Empathy Map의 6가지 영역을 자동 생성하는 웹앱입니다.
고객의 시각, 청각, 사고/감정, 행동, 고충, 기대를 체계적으로
분석하여 마케팅/UX 전략 수립에 활용할 수 있습니다.

[Empathy Map 개념]
Empathy Map(공감 지도)은 고객의 경험을 6가지 관점에서
시각화하는 UX/마케팅 도구입니다. 고객을 깊이 이해함으로써
제품 개발, 마케팅 메시지, 서비스 개선에 활용됩니다.

[주요 기능]

■ 6가지 분석 영역:
  - See (보다): 고객이 보는 환경, 경쟁사 제품, 시장 트렌드
  - Hear (듣다): 고객이 접하는 채널, 콘텐츠, 주변인의 이야기
  - Think & Feel (생각과 감정): 관심사, 걱정, 꿈, 감정 상태
  - Say & Do (말과 행동): 성향, 표현 방식, 활동 커뮤니티
  - Pain (불편/고충): 두려움, 불만, 장애물, 리스크
  - Gain (기대/바람): 필요, 기대, 성공 기준, 원하는 결과

■ 입력 항목:
  - API Key, 회사명, 제품/서비스, 고객 페르소나 (4개 입력)
  - 고객 페르소나를 별도 입력하여 더 정확한 분석 가능

■ 공통 기능:
  - 중앙 페르소나 허브 (SVG 아바타 + 이름 + 설명)
  - 2x2 + 1x2 그리드 레이아웃 (색상별 시각 구분)
  - 결과 저장: PDF / HTML 다운로드 / 텍스트 복사
  - 분석 진행 상태 표시 (5단계 프로그레스 바)
  - API 키 로컬 저장 (localStorage)
  - 반응형 디자인 (모바일 3단계 breakpoint: 900/768/600px)
  - 인쇄 최적화 (CSS @media print, 색상 보존)

[파일 구성]
- Empathy-map_maker.html : 메인 웹앱 (단일 HTML 파일)
- readme.txt              : 프로젝트 설명 (이 파일)
- .gitignore               : Git 추적 제외 설정

[사용 방법]
1. 웹앱을 열고 Anthropic API 키를 입력
2. 회사명 입력 (예: 경동나비엔)
3. 주요 제품/서비스 입력 (예: 콘덴싱 보일러)
4. 고객 페르소나 입력 (예: 30대 맞벌이 부부, 신축 아파트 입주 예정)
5. "AI Empathy Map 생성하기" 버튼 클릭
6. AI가 6가지 영역의 Empathy Map을 자동 생성
7. 결과를 PDF/HTML/텍스트로 저장 가능

[기술 스택]
- 프론트엔드: HTML5, CSS3, Vanilla JavaScript (단일 파일)
- AI: Anthropic Claude Haiku 4.5 API (브라우저 직접 호출)
- 프롬프트: System Prompt + User Prompt 분리 구조
- 폰트: Pretendard (JSDelivr CDN)
- 백엔드: 없음 (GitHub Pages 배포용)

[개발 환경 및 배포]
- 소스 코드: Google Drive (01.나눔경영컨설팅 웹앱(코딩)★/005.Empathy-map_maker/)
- Git 저장소: Google Drive 폴더에서 직접 Git 관리
- GitHub: jazzmania74/Empathy-map_maker (main 브랜치)
- 배포 URL: https://jazzmania74.github.io/Empathy-map_maker/Empathy-map_maker.html
- 수정 후 배포: git add → git commit → git push origin main → GitHub Pages 자동 반영

[주의사항]
- Anthropic API 키가 필요합니다 (사용자가 직접 입력)
- API 키는 브라우저의 localStorage에만 저장되며 서버로 전송되지 않습니다
- API 호출 비용은 Anthropic 계정에 청구됩니다

================================================================
