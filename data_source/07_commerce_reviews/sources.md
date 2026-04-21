# Commerce, Reviews, and Consumer Language

## Why this domain matters
- 리뷰와 소비자 언어는 비표준어, 축약, 감정 표현, 상품 속성 표현을 빠르게 확보하는 데 좋습니다.
- 전자상거래 assistant, 추천, 상품 QA, 감성 분석, 요약 등에 활용할 수 있습니다.

## Priority sources

| Source | URL | Scale | Structure | Access | Korean-specific value |
| --- | --- | --- | --- | --- | --- |
| `e9t/nsmc` | https://github.com/e9t/nsmc | 총 200k reviews | id, document, label | GitHub | 한국어 리뷰 감성 분석의 대표 공개 세트 |
| `kocohub/korean-hate-speech` | https://github.com/kocohub/korean-hate-speech | labeled 9,381, unlabeled 2,033,893 comments | comment, title, bias/hate labels | GitHub | 온라인 댓글체, 비정형 구어체 확보 |
| `adlnlp/K-MHaS` | https://github.com/adlnlp/K-MHaS | 109,692 utterances | multi-label hate speech annotations | GitHub/HF | 뉴스 댓글 기반 한국 온라인 표현 |
| `nayohan/SimKoR` | https://github.com/nayohan/SimKoR | README 발췌 기준 규모 미기재 | shopping review similarity pairs | GitHub | 쇼핑 리뷰 기반 유사도/검색 참고 |
| `kakao1513/shopping-intent-dataset` | https://huggingface.co/datasets/kakao1513/shopping-intent-dataset | 8,228 rows | text, label, label_id | Hugging Face | 쇼핑몰 제어/의도 분류 한국어 발화 |
| `Dasool/DC_inside_comments` | https://huggingface.co/datasets/Dasool/DC_inside_comments | 111,546 comments | raw unlabeled comments | Hugging Face | 한국 커뮤니티 댓글체, 비격식 표현, 밈성 표현 |

## Notes
- `NSMC`는 영화 리뷰라서 도메인 편향이 있으므로 일반 commerce review raw source로 보기보다 baseline/reference로 보는 편이 좋습니다.
- 실제 한국 전자상거래 corpus가 필요하면 공개 약관을 검토한 뒤 쇼핑몰 리뷰 크롤링 후보를 별도 설계해야 합니다.
- 커뮤니티 댓글체까지 함께 보고 싶으면 `DC_inside_comments`를 보조 raw corpus로 둘 수 있습니다.
