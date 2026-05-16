# B2B Content Topic Research Skill

B2B 클라우드 IaaS 서비스의 월간 콘텐츠 주제와 발행 일정을 만드는 Codex Skill입니다.

## 문제 정의

B2B 마케터는 매월 고객의 구매 여정에 맞는 콘텐츠 주제를 반복해서 발굴해야 합니다. 이 Skill은 SMB 고객, C레벨 의사결정자, 개발 팀장 구매 영향자를 기준으로 월 4~5건의 콘텐츠 주제와 발행 일정을 제안합니다.

## 사용 시나리오

- 이번 달 B2B 콘텐츠 주제 4~5건 발굴
- 구매 여정 1~3단계별 콘텐츠 주제 분배
- 주 1회 발행 일정 작성
- 담당 서비스 마케터 확인 전 후보 주제 정리

## 폴더 구조

```text
.
├── README.md
├── SKILL.md
├── references/
│   ├── audience-and-rules.md
│   ├── research-workflow.md
│   └── output-template.md
└── mock-data/
    └── monthly-brief-sample.md
```

## 실행 방법

Codex에게 아래처럼 요청합니다.

```text
b2b-content-topic-research Skill을 사용해서 2026년 6월 B2B 클라우드 IaaS 콘텐츠 주제 4~5건과 발행 일정을 만들어줘. 입력은 mock-data/monthly-brief-sample.md를 참고해줘.
```

## 입력

- 대상 월
- 서비스/브랜드 정보
- 현재 캠페인 또는 강조 메시지
- 고객 질문, 키워드, 기존 콘텐츠

예시 입력은 [mock-data/monthly-brief-sample.md](mock-data/monthly-brief-sample.md)에 있습니다.

## 출력

- 후보 주제 목록
- 월간 발행 일정
- 구매 여정 단계
- 페르소나
- 검색 의도
- CTA
- 완료 전 검증 체크리스트

## 검증 결과

- `SKILL.md` 구조 검증: 통과
- 필수 파일 확인: 통과
- `references/*.md` 확인: 통과
- mock data 포함: 통과
- 비밀값 패턴 검색: 노출 항목 없음

## 비밀값 처리

이 저장소에는 실제 인증값을 포함하지 않습니다. 필요한 경우 실제 값 대신 환경 변수명만 문서화합니다.

예시:

```text
OPENAI_API_KEY
GITHUB_TOKEN
SLACK_WEBHOOK_URL
```

## 제한 사항

- 최종 콘텐츠 주제는 담당 서비스 마케터 확인 후 확정해야 합니다.
- 경쟁사 이름은 직접 언급하지 않고 A사, B사처럼 대체합니다.
- 보안/장애 관련 직접 표현은 사용하지 않습니다.
