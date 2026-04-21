# Social, Culture, and History

## Why this domain matters
- 한국 맥락 부족 문제는 한국사, 제도, 지역, 전통문화, 생활문화, 관광, 시대어 부족에서 자주 발생합니다.
- 문화/역사/관광 텍스트는 한국 특화 grounding source로 쓰기 좋습니다.

## Priority sources

| Source | URL | Scale | Structure | Access | Korean-specific value |
| --- | --- | --- | --- | --- | --- |
| 모두의 말뭉치 `한국언어문화 지식 그래프 2024` | https://kli.korean.go.kr/corpus/main/requestMain.do | 공개 페이지에 총량 미기재 | language/culture knowledge graph resource | Website/request | 한국 언어문화 개체와 관계 정리에 적합 |
| 모두의 말뭉치 `일상 대화 말뭉치 추출 지식그래프 2025` | https://kli.korean.go.kr/corpus/main/requestMain.do | 공개 페이지에 총량 미기재 | culture-related dialogue-derived KG base data | Request/approval | 일상 대화 속 한국 문화 키워드와 관계 추출 |
| 모두의 말뭉치 `국어 역사 자료 말뭉치 2023` | https://kli.korean.go.kr/corpus/main/requestMain.do | 1,153종 문헌 | historical Korean documents | Request/approval | 시대별 어휘와 문체 변화 확보 |
| `Open Korean Historical Corpus` | https://huggingface.co/datasets/seyoungsong/Open-Korean-Historical-Corpus | 17.7M documents, 5.1B tokens | text + year/source metadata | Hugging Face | 대규모 한국 역사/근현대 텍스트 |
| 한국관광공사 `국문 관광정보 서비스` | https://www.data.go.kr/data/15101578/openapi.do | 약 26만 건 | 관광지/행사/숙박/소개/이미지 API | OpenAPI | 지역명, 관광 설명문, 한국 장소/문화 grounding |
| 한국관광공사 `관광지 오디오 가이드정보` | https://www.data.go.kr/data/15101971/openapi.do | 포털 페이지에 총량 미기재 | audio guide metadata + descriptions | OpenAPI | 역사·문화 설명형 텍스트 확보용 |
| 한국문화정보원 `한눈에보는문화정보조회서비스` | https://www.data.go.kr/data/15138937/openapi.do | 포털 페이지에 총량 미기재 | 공연/전시/행사 metadata | OpenAPI | 현대 한국 문화행사 문체와 개체명 |
| 국가유산청 `4대궁 및 종묘 문화재 해설 정보` | https://www.data.go.kr/dataset/15028101/openapi.do | 포털 페이지에 총량 미기재 | cultural heritage descriptions | OpenAPI | 전통문화, 건축, 역사 해설 문체 |
| 행정안전부 `문화_전통사찰 조회서비스` | https://www.data.go.kr/data/15155235/openapi.do | 포털 페이지에 총량 미기재 | traditional temple metadata and descriptions | OpenAPI | 불교·사찰·전통 종교 문화 맥락 |
| 한국학중앙연구원 `고지도 고지명서비스` | https://www.data.go.kr/data/15059485/openapi.do | 포털 페이지에 총량 미기재 | old place names, source texts, map metadata | OpenAPI | 역사 지명, 옛 지명 표기, 한국학 grounding |
| 한국학중앙연구원 `고문헌자료 문헌정보서비스` | https://www.data.go.kr/dataset/3059499/openapi.do | 포털 페이지에 총량 미기재 | bibliographic info, original images, original text metadata | OpenAPI | 한국 고문헌의 문헌정보·원문텍스트 연계 |
| 국립중앙도서관 `한국 고문헌 종합목록` | https://www.data.go.kr/data/15077395/openapi.do | 약 51만 건 | bibliographic metadata for ancient Korean documents | OpenAPI | 고문헌 제목, 저자, 발행, 소장 정보 확보 |
| 국가유산청 국립무형유산원 `기록영화(16mm) 정보` | https://www.data.go.kr/data/15028218/openapi.do | 포털 페이지에 총량 미기재 | documentary film metadata on intangible heritage | OpenAPI | 전통 예능·공예·의례의 무형유산 설명 자원 |
| 국가유산청 국립무형유산원 `무형유산 기록화 정보 목록 조회 서비스` | https://www.data.go.kr/data/15094314/openapi.do | 포털 페이지에 총량 미기재 | recorded heritage documentation listing service | OpenAPI | 무형유산 기록물과 설명 텍스트 확보 |
| 독립기념관 `독립운동가 인명사전 정보 DB` | https://www.data.go.kr/data/15069139/openapi.do | 포털 페이지에 총량 미기재 | person dictionary entries with movement classifications | OpenAPI | 근현대 한국사 인물·단체·운동계열 grounding |
| 독립기념관 `국내 독립운동사적지 정보 DB` | https://www.data.go.kr/data/15037980/openapi.do | 포털 페이지에 총량 미기재 | historic site descriptions with events, persons, references | OpenAPI | 독립운동 관련 장소·사건·인물 연결 정보 |
| 독립기념관 `국외 독립운동사적지 정보 DB` | https://www.data.go.kr/data/15037982/openapi.do | 포털 페이지에 총량 미기재 | overseas historic site descriptions | OpenAPI | 재외 독립운동 네트워크와 장소 맥락 |
| 독립기념관 `독립운동 도서 목록` | https://www.data.go.kr/data/15090341/openapi.do | 포털 페이지에 총량 미기재 | book list metadata on independence movement | OpenAPI | 근현대사 참고문헌과 주제 확장 |
| `lcw99/wikipedia-korean-20240501` | https://huggingface.co/datasets/lcw99/wikipedia-korean-20240501 | 515,425 문서 | title, section_titles, section_texts, full text | Hugging Face | 현대 한국어 백과형 지식과 서술 문체 |
| `SOGANG-ISDS/K-Culture-Desc` | https://huggingface.co/datasets/SOGANG-ISDS/K-Culture-Desc | 530 MCQA | scenario-based culture benchmark | Hugging Face | 한국 문화 추론/이해 평가 |

## Notes
- 생성 데이터의 한국 맥락을 강화하려면 관광/문화 API와 역사 말뭉치를 함께 쓰는 것이 좋습니다.
- 역사 지명과 고문헌 메타데이터가 필요하면 `고지도 고지명서비스`, `한국 고문헌 종합목록`이 추가 grounding layer가 됩니다.
- 역사·문화 서술형 백과 텍스트는 `한국 위키백과 dump`가 가장 다루기 쉬운 공개 소스 중 하나입니다.
- 근현대 한국사 보강에는 `독립기념관` 계열 API 묶음이 생각보다 강한 축입니다.
- 문화 설명문은 grounding corpus로, `K-Culture-Desc`는 evaluation/reference set으로 분리하는 편이 좋습니다.
