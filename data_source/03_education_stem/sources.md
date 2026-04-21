# Education and STEM

## Why this domain matters
- 한국형 교육 데이터는 학년, 교과, 평가 방식, 설명형 답안, 튜터 어투를 반영할 수 있습니다.
- STEM 도메인은 수학/과학/기술 문체와 정답 중심 reasoning에 유리합니다.

## Priority sources

| Source | URL | Scale | Structure | Access | Korean-specific value |
| --- | --- | --- | --- | --- | --- |
| AI Hub `영상 교육자료 기반 문제 생성 데이터` | https://www.aihub.or.kr/aihubdata/data/view.do?aihubDataSe=data&currMenu=&dataSetSn=71808&topMenu= | 영상 3,900건, QA 12,078건 | script + problem/answer JSON | Download/API, approval required | 교과·학년 태그가 있는 교육형 QA |
| AI Hub `한국어-영어 번역 말뭉치(기술과학)` | https://aihub.or.kr/aihubdata/data/view.do?dataSetSn=124 | 150만 문장 | parallel corpus | Download/API, approval required | ICT/전기전자/기계/의학 전문 어휘 |
| 모두의 말뭉치 `글쓰기 원시 자료 말뭉치 2024` | https://kli.korean.go.kr/corpus/main/requestMain.do | 공개 페이지에 총량 미기재 | argumentative student writing | Request/approval | 한국 대학생 논증 글쓰기 |
| 모두의 말뭉치 `글쓰기 채점 자료 말뭉치 2024` | https://kli.korean.go.kr/corpus/main/requestMain.do | 공개 페이지에 총량 미기재 | writing + expert scoring | Request/approval | 평가 기준형 instruction/reference |
| 모두의 말뭉치 `글쓰기 첨삭 지원을 위한 지시문 기반 생성 말뭉치 2024` | https://kli.korean.go.kr/corpus/main/requestMain.do | 공개 페이지에 총량 미기재 | instruction-based correction corpus | Request/approval | 한국어 글쓰기 첨삭형 데이터 |
| 국립국어원 `한국어 학습자 말뭉치 나눔터` | https://kcorpus.korean.go.kr/index/goIntroduceSite.do | 1차 약 440만 어절 공개, 총 1,000만 어절 구축 목표 | learner writing/speaking corpus with learner metadata | Dedicated site | 외국인 학습자의 실제 오류와 중간언어 패턴 확보 |
| 교육부 `커리어넷 직업정보` | https://www.data.go.kr/dataset/3038863/openapi.do?lang=ko | 포털 페이지에 총량 미기재 | job, major, counseling metadata | OpenAPI | 한국 진로·직업 정보 grounding |
| 국회도서관 `국가학술정보 OpenAPI 검색 서비스` | https://www.data.go.kr/data/15040835/openapi.do | 포털 페이지에 총량 미기재 | scholarly search metadata, subjects, researchers | OpenAPI | 한국 학술 주제어와 연구 메타데이터 확보 |
| 국회도서관 `국가학술정보 OpenAPI 분석 서비스` | https://www.data.go.kr/data/15040836/openapi.do | 포털 페이지에 총량 미기재 | related researchers, journals, topics, trends | OpenAPI | 학술 지식 그래프형 확장에 유용 |
| 대구경북과학기술원 `대학 입시 질의응답 정보` | https://www.data.go.kr/data/15068993/openapi.do | 포털 페이지에 총량 미기재 | title, content, answer, links, date, views | OpenAPI | 한국 대학 입시 질의응답 문체와 FAQ 구조 |
| 대구경북과학기술원 `대학원 입시 질의응답 정보` | https://www.data.go.kr/data/15069005/openapi.do | 포털 페이지에 총량 미기재 | title, content, answer, links, date, views | OpenAPI | 대학원 입시/행정 문의 문체와 응답 패턴 |
| `neuralfoundry-coder/aihub-korean-education-instruct-sample` | https://huggingface.co/datasets/neuralfoundry-coder/aihub-korean-education-instruct-sample | 6,000 rows sample | Chat-style conversations + category metadata | Hugging Face | AI Hub 교육 데이터 재가공 샘플 확인용 |
| `klue/klue` | https://huggingface.co/datasets/klue/klue | 205,608 rows total | NLI, MRC, RE, DST, etc. | Hugging Face | 한국어 NLU benchmark 전반 |
| `kakaobrain/kor_nli` | https://huggingface.co/datasets/kakaobrain/kor_nli | 약 95만 문장쌍 규모 | premise, hypothesis, entailment/contradiction/neutral | Hugging Face | 한국어 추론형 benchmark, 문장 이해 reference |
| `dkoterwa/kor-sts` | https://huggingface.co/datasets/dkoterwa/kor-sts | 8,532 문장쌍 | sentence pair + similarity score | Hugging Face | 의미 유사도와 표현 변환 평가 |

## Notes
- 실제 학습용 raw source와 benchmark를 분리하는 것이 좋습니다.
- 학습자 말뭉치는 native Korean corpus와 결합하면 한국어 교육/교정 assistant seed로 특히 좋습니다.
- 입시 Q&A 계열은 작더라도 실제 한국 행정·상담형 교육 문체를 얻는 데 도움이 됩니다.
- 교육 도메인은 한국 학교급/교과 체계가 반영된 source를 우선순위로 두는 편이 안전합니다.
