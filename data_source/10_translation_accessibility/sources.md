# Translation, Parallel Corpora, and Accessibility

## Why this domain matters
- 한국어 데이터셋을 확장할 때 번역/병렬 코퍼스는 style transfer, multilingual alignment, synthetic expansion에 유용합니다.
- 점자·수어·학습자 지원 자료는 접근성과 inclusive Korean AI 설계에 중요합니다.

## Priority sources

| Source | URL | Scale | Structure | Access | Korean-specific value |
| --- | --- | --- | --- | --- | --- |
| 모두의 말뭉치 `한국어-한국수어 병렬 말뭉치 2023` | https://kli.korean.go.kr/corpus/main/requestMain.do | 공개 페이지에 총량 미기재 | Korean spoken data translated to KSL | Request/approval | 한국어와 한국수어 간 병렬 표현 확보 |
| 모두의 말뭉치 `한국수어-한국어 병렬 말뭉치 2025` | https://kli.korean.go.kr/corpus/main/requestMain.do?lang=en | 공개 페이지에 총량 미기재 | sign-language video + Korean translation | Request/approval | 수어 대화 기반 한국어 정렬 |
| 모두의 말뭉치 `한국수어 주석 말뭉치 2025` | https://kli.korean.go.kr/corpus/main/requestMain.do?lang=en | 공개 페이지에 총량 미기재 | multi-tier annotated sign-language conversation corpus | Request/approval | 수어 발화 segmentation/annotation reference |
| 모두의 말뭉치 `묵자-점자 병렬 말뭉치 2024` | https://kli.korean.go.kr/corpus/main/requestMain.do | 공개 페이지에 총량 미기재 | Korean text to braille parallel corpus | Request/approval | 한국어 점역/접근성 데이터 |
| 모두의 말뭉치 `한국어-베트남어 병렬 말뭉치 2024` | https://kli.korean.go.kr/corpus/main/requestMain.do?lang=en | 공개 페이지에 총량 미기재 | written/spoken Korean translated to Vietnamese | Request/approval | 다국어 확장 시 한국어 중심 병렬 데이터 |
| 모두의 말뭉치 `한국어-우즈베크어 병렬 말뭉치 2024` | https://kli.korean.go.kr/corpus/main/requestMain.do?lang=en | 공개 페이지에 총량 미기재 | written/spoken Korean translated to Uzbek | Request/approval | 이주민/다문화 맥락 보강 |
| 모두의 말뭉치 `한국어-인도네시아어 병렬 말뭉치 2023` | https://kli.korean.go.kr/corpus/main/requestMain.do?lang=en | 공개 페이지에 총량 미기재 | written/spoken Korean translated to Indonesian | Request/approval | 실사용 번역과 다문화 소통 확장 |
| 모두의 말뭉치 `한국어-힌디어 병렬 말뭉치 2023` | https://kli.korean.go.kr/corpus/main/requestMain.do?lang=en | 공개 페이지에 총량 미기재 | written/spoken Korean translated to Hindi | Request/approval | 한국어 중심 병렬 말뭉치 확대 |
| 모두의 말뭉치 `한국어-태국어 병렬 말뭉치 2023` | https://kli.korean.go.kr/corpus/main/requestMain.do?lang=en | 공개 페이지에 총량 미기재 | written/spoken Korean translated to Thai | Request/approval | 동남아권 한국어 학습/번역 대응 |
| 모두의 말뭉치 `한국어-필리핀 타갈로그어 병렬 말뭉치 2023` | https://kli.korean.go.kr/corpus/main/requestMain.do?lang=en | 공개 페이지에 총량 미기재 | written/spoken Korean translated to Tagalog | Request/approval | 현장 통역·상담형 데이터 seed |
| `AAILab/KSL-LEX` | https://huggingface.co/datasets/AAILab/KSL-LEX | 6,463 entries | lexical database of Korean Sign Language | Hugging Face | 한국수어 어휘와 품사 정보 |
| `lemon-mint/korean_parallel_sentences_v1.1` | https://huggingface.co/datasets/lemon-mint/korean_parallel_sentences_v1.1 | 492,564 문장쌍 | Korean-English parallel sentences | Hugging Face | 빠른 번역 baseline 구축용 |
| `lemon-mint/korean_english_parallel_wiki_augmented_v1` | https://huggingface.co/datasets/lemon-mint/korean_english_parallel_wiki_augmented_v1 | 503,245 문장쌍 | Wikipedia-derived Korean-English parallel pairs | Hugging Face | 위키 기반 지식형 병렬 데이터 |
| `Moo/korean-parallel-corpora` | https://huggingface.co/datasets/Moo/korean-parallel-corpora | 96.2k train rows | Korean-English parallel corpus | Hugging Face | 비교적 가벼운 병렬 실험용 |
| `SEACrowd/talpco` | https://huggingface.co/datasets/SEACrowd/talpco | 한국어 포함 다국어 병렬 세트 | Japanese source + Korean and others | Hugging Face | 한국어 다국어 정렬 실험에 사용 가능 |

## Notes
- 번역 병렬 코퍼스는 한국 맥락을 직접 강화하기보다는 alignment와 multilingual extension에 강점이 있습니다.
- 접근성 분야는 `점자`, `수어`, `학습자` 자료를 분리 관리하면 downstream 활용이 편합니다.
