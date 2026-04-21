# Korean Dataset Source Catalog Summary

## Scope
- This catalog focuses on publicly discoverable Korean-language sources that can help build Korean-first text datasets with stronger local context.
- The emphasis is on sources that improve Korean conversational style, honorific consistency, Korean cultural grounding, and domain-specific factual grounding.
- I prioritized official Korean sources first, then public benchmark or mirror sources on Hugging Face and GitHub.

## Recommended domain map
1. Conversation, honorifics, and everyday speech
2. Social, culture, and history
3. News, media, and summarization
4. Education and STEM
5. Legal and public administration
6. Healthcare and medical knowledge
7. Finance and business
8. Commerce, reviews, and consumer language
9. Language resources, dictionaries, and general Korean knowledge
10. Safety, social norms, and toxicity
11. Translation, parallel corpora, and accessibility
12. Disaster, safety, and emergency communication
13. Agriculture, food, and dietary culture
14. User-generated web, blogs, and community text

## Best starting points
- `AI Hub + 모두의 말뭉치` should be the core for high-quality Korean-first seed data.
- `공공데이터포털 API` should be the core for updatable grounding data in law, tourism, culture, health, and public information.
- `Hugging Face/GitHub` should be used for open benchmarks, mirrors, and quick experiments rather than as the only source of truth.
- `국회/국회도서관/특허/한국학중앙연구원` 계열 API도 한국 특화 전문 문체와 제도/역사 grounding 확보에 꽤 중요합니다.
- 새로 확인된 강한 축은 `재난·안전`, `농식품·레시피`, `UGC/커뮤니티 웹텍스트`입니다.
- 이번 라운드에서 특히 더 보강된 것은 `독립기념관`, `국가유산청 국립무형유산원`, `법제처 자치법규`, `식약처 의약품 안전정보`, `입시 Q&A`, `향토음식/전통주` 축입니다.

## Highest-priority sources by purpose
- Conversation quality and honorifics:
  `AI Hub 한국어 대화`, `AI Hub 감성 대화 말뭉치`, `모두의 말뭉치 일상 대화`, `SNS 멀티턴 대화`
- Korean cultural grounding:
  `한국언어문화 지식 그래프`, `일상 대화 말뭉치 추출 지식그래프`, `국어 역사 자료 말뭉치`, `한국관광공사 API`
- General Korean written quality:
  `신문 말뭉치`, `문서 요약 말뭉치`, `글쓰기 원시 자료`, `글쓰기 첨삭 인스트럭션 말뭉치`
- Domain-specialized QA:
  `법률 지식베이스`, `금융·법률 문서 기계독해`, `초거대 AI 헬스케어 질의응답`
- Public and institutional grounding:
  `국회 회의록 API`, `OpenDART`, `특허실용신안 정보 검색`, `국가학술정보 OpenAPI`
- Historical and heritage grounding:
  `독립운동가 인명사전`, `국내/국외 독립운동사적지`, `고문헌자료 문헌정보서비스`, `무형유산 기록화`
- Reference and control layer:
  `한국어기초사전`, `표준국어대사전`, `NIKLex`, `유사 문장 말뭉치`
- Accessibility and multilingual extension:
  `한국수어-한국어 병렬 말뭉치`, `묵자-점자 병렬 말뭉치`, `한국어 학습자 말뭉치`, `한국어 다국어 병렬 말뭉치`
- Emergency/public communication:
  `긴급재난문자`, `자연재난/사회재난/생활안전 국민행동요령`
- Food and regional lifestyle:
  `농업용어사전`, `인테러뱅`, `우리잡곡 웰빙 레시피`, `식품영양성분DB`
- Internet-style Korean expansion:
  `geulgyeol-blog-korean`, `DC_inside_comments`, `namu_wiki_512_char_seg`, `fineweb-2-edu-korean`

## Access pattern notes
- `AI Hub`: often downloadable only after login and approval, and some datasets show domestic-use restrictions.
- `모두의 말뭉치`: request/approval flow is common; many entries provide preview and description before access.
- `공공데이터포털`: good for APIs and metadata-rich structured sources; useful when storage is limited because you can query incrementally.
- `Hugging Face/GitHub`: easiest for quick inspection, prototyping, and benchmark baselines, but license and provenance must be checked per dataset.

## Practical collection strategy
1. Start with metadata-only cataloging, not full downloads.
2. Separate `raw source`, `instruction/reference`, and `evaluation` datasets.
3. Use official sources first where Korean context quality matters most.
4. Use APIs for dynamic domains such as law, finance, tourism, and public institutions.
5. Use dictionaries and lexical resources to control honorifics, expression correction, and paraphrase generation.

## Deliverables created
- [Conversation sources](/Users/hongminki/Github/nvidia/test/data_source/00_conversation_honorifics/sources.md)
- [Social and culture sources](/Users/hongminki/Github/nvidia/test/data_source/01_social_culture_history/sources.md)
- [News and summarization sources](/Users/hongminki/Github/nvidia/test/data_source/02_news_media_summarization/sources.md)
- [Education and STEM sources](/Users/hongminki/Github/nvidia/test/data_source/03_education_stem/sources.md)
- [Legal and public sources](/Users/hongminki/Github/nvidia/test/data_source/04_legal_public/sources.md)
- [Healthcare sources](/Users/hongminki/Github/nvidia/test/data_source/05_healthcare/sources.md)
- [Finance sources](/Users/hongminki/Github/nvidia/test/data_source/06_finance_business/sources.md)
- [Commerce and review sources](/Users/hongminki/Github/nvidia/test/data_source/07_commerce_reviews/sources.md)
- [Language resource sources](/Users/hongminki/Github/nvidia/test/data_source/08_language_resources/sources.md)
- [Safety and social norms sources](/Users/hongminki/Github/nvidia/test/data_source/09_safety_social_norms/sources.md)
- [Translation and accessibility sources](/Users/hongminki/Github/nvidia/test/data_source/10_translation_accessibility/sources.md)
- [Disaster and safety sources](/Users/hongminki/Github/nvidia/test/data_source/11_disaster_safety/sources.md)
- [Agriculture and food sources](/Users/hongminki/Github/nvidia/test/data_source/12_agriculture_food/sources.md)
- [User-generated web sources](/Users/hongminki/Github/nvidia/test/data_source/13_user_generated_web/sources.md)

## Limitation
- I cannot autonomously keep working until `2026-04-21 07:00` after this turn ends or wait for token refill on my own.
- To compensate, I created the catalog structure now so we have a solid base ready in the repository.
