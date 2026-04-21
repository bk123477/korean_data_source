# News, Media, and Summarization

## Why this domain matters
- 뉴스는 문어체, 시사어, 기관명, 사회 이슈, 논증 구조를 빠르게 확보할 수 있는 핵심 소스입니다.
- 요약 데이터는 instruction tuning과 평가에 모두 유용합니다.

## Priority sources

| Source | URL | Scale | Structure | Access | Korean-specific value |
| --- | --- | --- | --- | --- | --- |
| 모두의 말뭉치 `신문 말뭉치 2024` | https://kli.korean.go.kr/main/requestMain.do?lang=ko | 공개 페이지에 총량 미기재 | copyright-cleared newspaper articles | Request/approval | 고품질 한국어 문어체와 시사 표현 |
| 모두의 말뭉치 `신문 말뭉치 2022` | https://kli.korean.go.kr/corpus/main/requestMain.do?lang=en | 2021년 생산 기사 기반, 총량 미기재 | machine-analyzable newspaper corpus | Request/approval | 연도별 뉴스체 변화와 저작권 정리된 기사 원문 |
| 모두의 말뭉치 `온라인 게시 자료 말뭉치 2022` | https://kli.korean.go.kr/corpus/main/requestMain.do?lang=en | 공개 페이지에 총량 미기재 | online communities and SNS posts | Request/approval | 기사체와 다른 한국 온라인 문어/반구어 혼합체 |
| 모두의 말뭉치 `문서 요약 말뭉치 2024` | https://kli.korean.go.kr/corpus/main/requestMain.do | 공개 페이지에 총량 미기재 | article + abstractive summaries | Request/approval | 한국어 뉴스 요약 reference |
| 모두의 말뭉치 `문서 요약 평가 말뭉치 2024` | https://kli.korean.go.kr/corpus/main/requestMain.do | 공개 페이지에 총량 미기재 | summary + human evaluation | Request/approval | 요약 품질 평가 기준 확보 |
| 모두의 말뭉치 `논증적 글 요약 말뭉치 2025` | https://kli.korean.go.kr/corpus/main/requestMain.do | 1,008건 | editorial article + selected key sentences + abstractive summary | Request/approval | 논증형 문체와 요약 학습 |
| 모두의 말뭉치 `논증적 글 요약 평가 말뭉치 2025` | https://kli.korean.go.kr/corpus/main/requestMain.do | 2,016건 평가 | summary evaluation corpus | Request/approval | 논설/사설 요약 평가 |
| `daekeun-ml/naver-news-summarization-ko` | https://huggingface.co/datasets/daekeun-ml/naver-news-summarization-ko | train 22.2k rows | date, category, press, title, document, summary | Hugging Face | 한국 뉴스 기사 요약 실험용 공개 세트 |
| `klue/klue` `ynat` subset | https://huggingface.co/datasets/klue/klue | ynat 54.8k rows | news title + label | Hugging Face | 뉴스 제목 분류, 짧은 시사 텍스트 |
| `FISA-conclave/news-sentiment-dataset` | https://huggingface.co/datasets/FISA-conclave/news-sentiment-dataset | 45,544 문장 | sentence + sentiment label | Hugging Face | 기업/경제 뉴스 문장 감성 |
| `HAERAE-HUB/KOREAN-WEBTEXT` | https://huggingface.co/datasets/HAERAE-HUB/KOREAN-WEBTEXT | 1.28M docs, 2.2B tokens | web text corpus with source metadata | Hugging Face | 뉴스 외 일반 한국어 웹문서 확장 |
| `eliceai/korean-webtext-edu` | https://huggingface.co/datasets/eliceai/korean-webtext-edu | 1M+ class | educationally filtered web text | Hugging Face | 설명형/사실형 한국어 텍스트 보강 |
| `minpeter/fineweb-2-edu-korean` | https://huggingface.co/datasets/minpeter/fineweb-2-edu-korean | 2.11M rows | text, url, date, score, language metadata | Hugging Face | 교육성 점수 기반 정제 한국어 웹텍스트 |
| `minpeter/geulgyeol-blog-korean` | https://huggingface.co/datasets/minpeter/geulgyeol-blog-korean | 1.75M rows | raw blog-style Korean text | Hugging Face | 블로그/홍보/생활형 문어와 반구어 혼합체 |

## Notes
- 뉴스 원문은 저작권 이슈가 있으므로 모두의 말뭉치처럼 이용 허락이 정리된 소스를 우선 검토하는 것이 안전합니다.
- 기사체만이 아니라 `온라인 게시 자료 말뭉치`를 같이 쓰면 댓글/커뮤니티형 온라인 한국어도 함께 커버할 수 있습니다.
- 순수 뉴스 외 공개 웹문서 확장은 `KOREAN-WEBTEXT`, `fineweb-2-edu-korean`, `geulgyeol-blog-korean` 조합이 유용합니다.
- `신문 말뭉치 -> 요약 말뭉치 -> 요약 평가 말뭉치` 흐름은 summarization pipeline 설계에 유용합니다.
