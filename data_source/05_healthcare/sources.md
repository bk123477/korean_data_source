# Healthcare and Medical Knowledge

## Why this domain matters
- 의료 도메인은 정확성, 전문용어, 한국식 진료과/질환명 표현이 중요합니다.
- 한국형 건강상담, 문진, 설명형 응답 품질 개선에 핵심입니다.

## Priority sources

| Source | URL | Scale | Structure | Access | Korean-specific value |
| --- | --- | --- | --- | --- | --- |
| AI Hub `초거대 AI 헬스케어 질의응답 데이터` | https://www.aihub.or.kr/aihubdata/data/view.do?aihubDataSe=data&currMenu=115&dataSetSn=71762&topMenu=100 | 3,893,203 QA, 242,870,922 어절, 19 질환군/500여 질환 | question-answer JSON with disease metadata | Approval/download | 한국 질환군, 진료과, 의료 설명형 QA |
| AI Hub `의료, 법률 전문 서적 말뭉치` | https://aihub.or.kr/aihubdata/data/view.do?dataSetSn=71487 | 1억+ 어절 | books, patents, judgments-based text corpus | Download/API, approval required | 의료 전문 문체와 용어 확보 |
| `snuh/ClinicalQA` | https://huggingface.co/datasets/snuh/ClinicalQA | 1,000+ QA | clinical exam-style QA | Hugging Face | 한국 의사면허시험 수준 reference |
| `sean0042/KorMedMCQA` | https://huggingface.co/datasets/sean0042/KorMedMCQA | 7,469 문항 | multiple-choice medical QA from Korean licensing exams | Hugging Face | 한국 의사/간호/약사/치과 시험 기반 benchmark |
| 건강보험심사평가원 `비급여진료비정보조회서비스` | https://www.data.go.kr/data/15001700/openapi.do | 포털 페이지에 총량 미기재 | treatment/medical cost API | OpenAPI | 한국 의료비/항목 표현 grounding |
| 건강보험심사평가원 `의료기관별상세정보서비스` | https://www.data.go.kr/data/15001699/openapi.do | 포털 페이지에 총량 미기재 | hospital details, departments, equipment | OpenAPI | 병원/진료과/시설 관련 한국 개체명 |
| 식품의약품안전처 `의약품안전사용서비스(DUR)품목정보` | https://www.data.go.kr/data/15059486/openapi.do | 포털 페이지에 총량 미기재 | contraindications, age/pregnancy warnings, dosage cautions | OpenAPI | 한국 복약 안전 문체와 금기 정보 |
| 식품의약품안전처 `의약품개요정보(e약은요)` | https://www.data.go.kr/data/15075057/openapi.do | 포털 페이지에 총량 미기재 | efficacy, dosage, interactions, adverse effects, storage | OpenAPI | 한국어 복약지도·주의사항 설명문 |

## Notes
- 의료는 high-stakes domain이므로 실제 학습 데이터와 지식 조회 소스를 분리하는 것이 좋습니다.
- `ClinicalQA`와 `KorMedMCQA`는 raw corpus보다는 평가/전문 QA reference로 쓰는 편이 적합합니다.
- 약품 설명/복약 주의 쪽은 `DUR`와 `e약은요`를 같이 보는 편이 좋습니다.
- 서비스 목적이면 최신 제도/수가/기관 정보는 API 기반 업데이트가 필요합니다.
