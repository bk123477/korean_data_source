# Legal and Public Administration

## Why this domain matters
- 한국 법률/행정 데이터는 제도명, 법령명, 민원 표현, 판례 문체 등 매우 한국 특화된 신호를 제공합니다.
- 환각 억제와 도메인 grounded QA에 특히 중요합니다.

## Priority sources

| Source | URL | Scale | Structure | Access | Korean-specific value |
| --- | --- | --- | --- | --- | --- |
| AI Hub `법률 지식베이스` | https://www.aihub.or.kr/aihubdata/data/view.do?dataSetSn=99 | 약 27만 건 | law terms, ontology, relations, legal knowledge base | Download/API, approval required | 법률 용어/개체/관계 구조화 |
| AI Hub `의료, 법률 전문 서적 말뭉치` | https://aihub.or.kr/aihubdata/data/view.do?dataSetSn=71487 | 102,300,332 어절 | txt + JSON labels, books/patents/judgments | Download/API, approval required | 전문 문어체 대규모 corpus |
| AI Hub `금융, 법률 문서 기계독해 데이터` | https://aihub.or.kr/aihubdata/data/view.do?dataSetSn=71610 | 공개 페이지에 총량 미기재 | document/table MRC QA | Download/API, approval required | 한국형 문서 QA, 정답 유형 다양 |
| 국가법령정보 공동활용 | https://open.law.go.kr/LSO/information/guide.do | API 191종 가이드 노출 | current laws, revisions, interpretations, KB APIs | OpenAPI, approval required | 법령 원문과 변경 이력, 일상용어-법령용어 연계 |
| 법제처 `생활법령 백문백답` | https://www.data.go.kr/data/15000335/openapi.do | 12개 분야 수준 | Q&A style life-law content | OpenAPI | 일반 국민 질의형 법률 문체 |
| 법제처 `모바일 자치법규 본문 조회` | https://www.data.go.kr/data/15057909/openapi.do | 포털 페이지에 총량 미기재 | ordinance/article-level full text API | OpenAPI | 지방자치단체 조례·규칙의 실제 한국 행정 문체 |
| 국민권익위원회 `민원정책 질의응답조회서비스` | https://www.data.go.kr/data/15074671/openapi.do | 포털 페이지에 총량 미기재 | policy/civil complaint Q&A JSON API | OpenAPI, auto-approved | 국민신문고 기반 민원·정책 질의응답 |
| 국회 국회사무처 `본회의 회의록` | https://www.data.go.kr/data/15126007/openapi.do | 포털 페이지에 총량 미기재 | plenary session transcript API | OpenAPI, unrestricted use listed | 법안·정책 관련 정제된 공식 발화 텍스트 |
| 국회 국회사무처 `위원회 회의록` | https://www.data.go.kr/data/15126038/openapi.do | 포털 페이지에 총량 미기재 | committee meeting transcript API | OpenAPI, unrestricted use listed | 전문위원·의원 질의응답, 제도 논의 문체 |
| 국회 국회사무처 `공청회 회의록` | https://www.data.go.kr/data/15126156/openapi.do | 포털 페이지에 총량 미기재 | hearing transcript API | OpenAPI, unrestricted use listed | 법/정책 쟁점 토론형 텍스트 |
| 국회 국회사무처 `인사청문회 회의록` | https://www.data.go.kr/data/15126144/openapi.do | 포털 페이지에 총량 미기재 | confirmation hearing transcript API | OpenAPI, unrestricted use listed | 질의·답변·검증형 공적 대화 |
| 국회 국회사무처 `대통령시정연설 포함 회의록` | https://www.data.go.kr/data/15126148/openapi.do | 포털 페이지에 총량 미기재 | speech/transcript API | OpenAPI, unrestricted use listed | 공식 연설체, 정책 메시지, 국정 문체 |
| 지식재산처 `특허실용신안 정보 검색 서비스` | https://www.data.go.kr/data/15058788/openapi.do | 포털 페이지에 총량 미기재 | patent metadata, title, abstract, IPC, applicant | OpenAPI | 한국 특허 문체와 기술 요약 텍스트 |
| `ducut91/korean-court-judgments` | https://huggingface.co/datasets/ducut91/korean-court-judgments | 163,546 판결문 | structured judgment text | Hugging Face | 판결문 요약/검색/QA reference |
| `JusWis/korean-legal-terminology` | https://huggingface.co/datasets/JusWis/korean-legal-terminology | 17,484 samples | term-definition style data | Hugging Face | 법률 용어 설명 학습용 |
| `neuralfoundry-coder/korean-legal-instruction-sample` | https://huggingface.co/datasets/neuralfoundry-coder/korean-legal-instruction-sample | sample 4.92k rows, 전체 설명 약 23.3만 건 | instruction/output + metadata | Hugging Face | AI Hub 법률 데이터 재가공 확인용 |

## Notes
- 실제 서비스용이면 최신성 문제 때문에 법령 원문은 API 연동을 우선 고려하는 편이 좋습니다.
- 법률/행정 grounding을 넓히려면 `법령 + 회의록 + 생활법령 + 특허`를 같이 잡는 편이 좋습니다.
- 한국 행정 민원체를 보강하려면 `민원정책 질의응답조회서비스`가 실무적으로 꽤 유용합니다.
- 중앙법령 외에 `자치법규`까지 넣으면 지역 행정 문체를 더 현실적으로 커버할 수 있습니다.
- 법률 분야는 라이선스와 재배포 조건을 별도 검토해야 합니다.
