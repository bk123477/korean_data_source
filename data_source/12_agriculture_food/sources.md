# Agriculture, Food, and Korean Dietary Culture

## Why this domain matters
- 농업·식품 데이터는 한국 식재료, 전통 음식, 조리법, 생활문화, 건강/영양 표현을 함께 담고 있습니다.
- 한국형 food assistant, recipe QA, 지역 먹거리/식생활 grounding에 특히 유용합니다.

## Priority sources

| Source | URL | Scale | Structure | Access | Korean-specific value |
| --- | --- | --- | --- | --- | --- |
| 농촌진흥청 `농업용어사전` | https://www.data.go.kr/data/3061058/openapi.do | 포털 페이지에 총량 미기재 | term dictionary API | OpenAPI | 농업 전문어와 한국 농촌 맥락 용어 |
| 농촌진흥청 `농업농촌종합정보(인테러뱅)` | https://www.data.go.kr/data/15002055/openapi.do | 포털 페이지에 총량 미기재 | issue/explanatory agricultural articles | OpenAPI | 농업 기술과 농촌 이슈 설명형 텍스트 |
| 농촌진흥청 `농업경영종합정보_회계박사_질의응답` | https://www.data.go.kr/data/15123445/fileData.do | 44행 | CSV/XML/JSON Q&A board export | File/OpenAPI metadata | 농업 회계·실무 질의응답의 실제 상담형 문체 |
| 농촌진흥청 국립식량과학원 `우리잡곡 웰빙 레시피` | https://www.data.go.kr/data/15151499/openapi.do | 포털 페이지에 총량 미기재 | recipe name, ingredients, cooking method, effects | OpenAPI | 잡곡 중심 한국 레시피와 생활 건강 문체 |
| 농촌진흥청 국립식량과학원 `농식품 식단관리 음식정보 제공` | https://www.data.go.kr/data/15141900/openapi.do | 포털 페이지에 총량 미기재 | food information API | OpenAPI | 한국 음식명과 식단 관리 표현 |
| 농촌진흥청 국립식량과학원 `농식품 식단관리(메뉴젠) 음식 및 조리정보` | https://www.data.go.kr/data/15143468/openapi.do | 포털 페이지에 총량 미기재 | food + cooking information API | OpenAPI | 조리 단계와 재료 설명형 데이터 |
| 농촌진흥청 국립식량과학원 `농식품 식단관리(메뉴젠) 음식 및 재료 정보` | https://www.data.go.kr/data/15143500/openapi.do | 포털 페이지에 총량 미기재 | food + ingredient API | OpenAPI | 한국 식재료명과 음식-재료 관계 |
| 식품의약품안전처 `식품영양성분DB정보` | https://www.data.go.kr/data/15127578/openapi.do | 포털 페이지에 총량 미기재 | food item + nutrient composition API | OpenAPI | 한국 식품명, 영양 성분, 식품 분류 체계 |
| 식품의약품안전처 `건강기능식품정보` | https://www.data.go.kr/data/15056760/openapi.do | 포털 페이지에 총량 미기재 | health functional food product API | OpenAPI | 한국 건강기능식품 제품 정보와 섭취 문체 |
| 전북특별자치도 `향토음식점서비스` | https://www.data.go.kr/data/15106765/openapi.do | 포털 페이지에 총량 미기재 | local restaurant/heritage food service metadata | OpenAPI | 지역 향토음식, 메뉴, 관광형 음식 맥락 |
| 경기도 `전통주 주류제조면허 추천서 발급 현황` | https://www.data.go.kr/data/15057688/openapi.do | 포털 페이지에 총량 미기재 | traditional liquor production license metadata | OpenAPI | 전통주 종류와 지역 양조 산업 맥락 |
| `Jaeuk-Han/korean-traditional-liquor-dataset` | https://huggingface.co/datasets/Jaeuk-Han/korean-traditional-liquor-dataset | dataset card 기준 structured release | traditional liquor schema/text metadata | Hugging Face | 한국 전통주 종류, 역사, 재료, 용도 정리 |

## Notes
- 이 도메인은 `문화`, `의료`, `관광` 도메인과 겹치는 만큼 cross-domain grounding source로 가치가 큽니다.
- 음식 데이터는 `레시피`, `영양`, `향토음식점`, `전통주`를 묶어 볼 때 한국 생활문화 색이 더 잘 살아납니다.
- 실제 상업 활용 전에는 각 API의 이용허락 범위를 다시 확인하는 것이 좋습니다.
