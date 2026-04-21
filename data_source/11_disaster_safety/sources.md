# Disaster, Safety, and Emergency Communication

## Why this domain matters
- 한국형 안전 안내는 짧고 직접적인 경보 문체, 행동요령 문체, 기관별 대응 표현이 뚜렷합니다.
- 재난문자, 행동요령, 경보 통계는 한국 사회 맥락형 공공 커뮤니케이션 데이터를 보강하는 데 유용합니다.

## Priority sources

| Source | URL | Scale | Structure | Access | Korean-specific value |
| --- | --- | --- | --- | --- | --- |
| 행정안전부 `긴급재난문자` | https://www.data.go.kr/data/15134001/openapi.do | 시간범위 2023년-2025년 1월 표기 | emergency alert message JSON API | OpenAPI via safetydata | 실제 한국 재난문자 문체와 지역/유형별 경보 표현 |
| 행정안전부 `자연재난 국민행동요령` | https://www.data.go.kr/data/15139401/openapi.do | 포털 페이지에 총량 미기재 | natural disaster action guide API | OpenAPI | 태풍·호우·폭염 등 한국형 재난 대응 문체 |
| 행정안전부 `사회재난 국민행동요령` | https://www.data.go.kr/data/15139402/openapi.do | 포털 페이지에 총량 미기재 | social disaster action guide API | OpenAPI | 화재·붕괴·감염병 등 위기 대응 설명문 |
| 행정안전부 `생활안전 국민행동요령` | https://www.data.go.kr/data/15139403/openapi.do | 포털 페이지에 총량 미기재 | daily safety guide API | OpenAPI | 일상형 안전 안내와 교육성 문체 |
| 행정안전부 `연도별 재난경보 및 재난예방 방송` | https://www.data.go.kr/data/15107242/openapi.do | 포털 페이지에 총량 미기재 | annual disaster warning statistics | OpenAPI | 재난경보/방송 체계 메타데이터 |
| 행정안전부 `지역별 재난경보 및 재난예방 방송` | https://www.data.go.kr/data/15107241/openapi.do | 포털 페이지에 총량 미기재 | regional disaster warning statistics | OpenAPI | 지역 기반 안전/재난 관리 맥락 |
| 행정안전부 `연도별 지역축제 안전사고` | https://www.data.go.kr/data/15107192/openapi.do | 포털 페이지에 총량 미기재 | annual local festival safety accident statistics | OpenAPI | 지역행사/축제 안전 맥락과 공공 안전 표현 |
| 농촌진흥청 `농업기계 안전정보` | https://www.data.go.kr/data/15002002/openapi.do | 포털 페이지에 총량 미기재 | safety guidance + accident prevention info | OpenAPI | 농촌 작업 안전과 장비 관련 한국어 안내 문체 |

## Notes
- 이 도메인은 long-form 지식보다 `짧고 직접적인 지시형 공공 문체` 확보에 강점이 있습니다.
- 일반 대화 데이터와 함께 쓰면 공공 경고, 안전 안내, 생활형 assistant 응답을 더 한국답게 만들 수 있습니다.
- `지역축제 안전사고` 같은 통계성 API도 안전 안내 도메인의 배경지식으로 쓸 수 있습니다.
