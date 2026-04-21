# Finance and Business

## Why this domain matters
- 한국 금융/비즈니스 문서는 보고서, 공시, 경제 기사, 제도명, 지표 설명 등 특화 문체가 강합니다.
- 기업 공시, 경제 뉴스, 금융 상담형 응답 데이터의 기반이 됩니다.

## Priority sources

| Source | URL | Scale | Structure | Access | Korean-specific value |
| --- | --- | --- | --- | --- | --- |
| AI Hub `금융, 법률 문서 기계독해 데이터` | https://aihub.or.kr/aihubdata/data/view.do?dataSetSn=71610 | 공개 페이지에 총량 미기재 | document/table QA over ODT/HWP/PDF | Download/API, approval required | 한국 금융 문서 독해 |
| OpenDART 오픈API | https://opendart.fss.or.kr/intro/main.do | 상장/비상장 공시 원문 대량 | filing XML, company metadata, financial statements | API | 한국 기업 공시 원문과 재무 텍스트 |
| 금융감독원 `공시정보_공시검색` | https://www.data.go.kr/data/3075133/openapi.do | 포털 페이지에 총량 미기재 | disclosure search API | OpenAPI | 공시 탐색 및 메타데이터 |
| 금융감독원 `공시정보_공시서류원본파일` | https://www.data.go.kr/data/15060602/openapi.do | 포털 페이지에 총량 미기재 | original filing files | OpenAPI | 원문 문서 수집용 |
| `KRX-Data/Won-Instruct` | https://huggingface.co/datasets/KRX-Data/Won-Instruct | 86,007 rows | prompt + responses | Hugging Face | KRX/BOK/FSC 등 공개 한국 금융 source 기반 |
| `FISA-conclave/news-sentiment-dataset` | https://huggingface.co/datasets/FISA-conclave/news-sentiment-dataset | 45,544 samples | sentence + label | Hugging Face | 기업 관련 한국어 뉴스 문장 감성 |

## Notes
- 최신성 중요도가 높아서 장기적으로는 `OpenDART + 경제 뉴스 + 정책/기관 문서` 조합이 유리합니다.
- 금융 데이터는 법률/규제 영역과 중첩되므로 `04_legal_public`과 함께 보는 것이 좋습니다.

