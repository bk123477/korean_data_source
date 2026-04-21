# Language Resources, Dictionaries, and General Korean Knowledge

## Why this domain matters
- 한국어 존댓말, 맞춤법, 의미 구분, 용례, 표현 교정은 사전·어휘 자료 없이 안정적으로 만들기 어렵습니다.
- 이 영역은 raw corpus라기보다 grounding/reference layer에 가깝습니다.

## Priority sources

| Source | URL | Scale | Structure | Access | Korean-specific value |
| --- | --- | --- | --- | --- | --- |
| 한국어기초사전 Open API | https://krdict.korean.go.kr/eng/openApi/openApiInfo | 포털 페이지에 총량 미기재 | dictionary entries, examples | OpenAPI | 학습자 친화 설명, 용례, 다국어 연계 |
| 표준국어대사전 Open API | https://www.data.go.kr/data/3057780/openapi.do | 포털 페이지에 총량 미기재 | standard dictionary entries | OpenAPI | 규범 국어 기준 |
| 21세기 세종계획 | https://kli.korean.go.kr/corpus/main/requestMain.do?lang=en | 대규모 국어 기초 말뭉치 묶음 | written, spoken, POS, syntax, semantics resources | Application bulletin board | 한국어 기초 언어자원의 장기 표준 축 |
| `hac541309/basic_korean_dict` | https://huggingface.co/datasets/hac541309/basic_korean_dict | 74,936 rows | machine-readable Korean Basic Dictionary | Hugging Face | 사전 정보를 학습 친화적으로 사용 가능 |
| 모두의 말뭉치 `어휘 관계 자료: NIKLex` | https://kli.korean.go.kr/corpus/main/requestMain.do | 공개 페이지에 총량 미기재 | synonym/antonym/hypernym evaluations | Request/approval | 어휘 관계 학습/평가 |
| 모두의 말뭉치 `유사 문장 말뭉치` | https://kli.korean.go.kr/corpus/main/requestMain.do | 공개 페이지에 총량 미기재 | human/computer paraphrases | Request/approval | paraphrase, rewriting, semantic similarity |
| 모두의 말뭉치 `국어 지식 기초 자료 2024` | https://kli.korean.go.kr/corpus/main/requestMain.do | 공개 페이지에 총량 미기재 | question-answer / explanation / example style language knowledge | Request/approval | 표현 오류, 표기, 어문 규범 설명 |
| 모두의 말뭉치 `문법성 판단 말뭉치` | https://kli.korean.go.kr/corpus/main/requestMain.do?lang=en | 공개 페이지에 총량 미기재 | grammaticality/acceptability judgments | Request/approval | 문장 자연스러움과 비문 판별 기준 |
| 모두의 말뭉치 `형태 분석 말뭉치` | https://kli.korean.go.kr/corpus/main/requestMain.do?lang=en | 공개 페이지에 총량 미기재 | morpheme-level POS-tagged corpus | Request/approval | 한국어 조사/어미/활용 분석 기반 |
| 모두의 말뭉치 `개체명 분석 말뭉치 2022` | https://kli.korean.go.kr/corpus/main/requestMain.do?lang=en | 공개 페이지에 총량 미기재 | NE boundaries + semantic categories | Request/approval | 한국 개체명 인식과 grounding entity layer |
| 모두의 말뭉치 `감성 분석 말뭉치 2020` | https://kli.korean.go.kr/corpus/main/requestMain.do?lang=en | 공개 페이지에 총량 미기재 | sentiment annotations on subjective expressions | Request/approval | 감정 표현과 어조 조절 reference |
| 모두의 말뭉치 `추론_확신성 분석 말뭉치 2020` | https://kli.korean.go.kr/corpus/main/requestMain.do?lang=en | 공개 페이지에 총량 미기재 | commitment bank style inference corpus | Request/approval | 화자의 확신도와 함의 추론 |
| `klue/klue` | https://huggingface.co/datasets/klue/klue | 205,608 rows | multiple Korean NLU tasks | Hugging Face | general Korean benchmark/reference |
| `ko-nlp/Korpora` | https://github.com/ko-nlp/Korpora | aggregator | downloader and corpus index | GitHub | 산재한 한국어 공개 코퍼스 탐색 허브 |
| `eaglewatch/Korean_Wikipedia_Dataset_for_GPT2_August_2022` | https://huggingface.co/datasets/eaglewatch/Korean_Wikipedia_Dataset_for_GPT2_August_2022 | 418,025 문서 | full Korean Wikipedia text | Hugging Face | 범용 한국어 백과 지식 source |
| `mansiksohn/opendict-korean-proverb` | https://huggingface.co/datasets/mansiksohn/opendict-korean-proverb | 수천 개 규모 속담 CSV | proverb text collection | Hugging Face | 속담·관용 표현과 문화적 은유 보강 |
| `korean-corpus/namu_wiki_512_char_seg` | https://huggingface.co/datasets/korean-corpus/namu_wiki_512_char_seg | 6.23M rows | namu wiki text segmented into chunks | Hugging Face | 백과/서브컬처/인터넷 지식형 한국어 대규모 확보 |

## Notes
- 사전/어휘 자료는 직접 pretraining source라기보다 post-processing, evaluation, synthetic generation control에 특히 유용합니다.
- 규범·형태·개체명·감성·확신성 코퍼스는 데이터 생성 후 품질 통제용 reference layer로 가치가 큽니다.
- `위키백과 + 나무위키 세그먼트`는 공개 지식형 한국어 확장에 유용하지만, 출처와 라이선스 분리를 신경 써야 합니다.
- honorific normalization, correction, lexical variation control에 이 레이어가 중요합니다.
