# Safety, Social Norms, and Toxicity

## Why this domain matters
- 한국어 데이터셋이 사회적 규범과 맥락을 반영하지 못하면, 무례함/혐오/부적절 발언 처리에서 흔들리기 쉽습니다.
- 한국 사회 맥락에 맞는 moderation/reference 세트가 필요합니다.

## Priority sources

| Source | URL | Scale | Structure | Access | Korean-specific value |
| --- | --- | --- | --- | --- | --- |
| 모두의 말뭉치 `부적절 발언 탐지 말뭉치 2023` | https://kli.korean.go.kr/main/requestMain.do?lang=ko | 공개 페이지에 총량 미기재 | inappropriate utterance + explicitness/context/intensity/domain annotations | Request/approval | 한국어 부적절 발언의 맥락형 라벨 |
| `kocohub/korean-hate-speech` | https://github.com/kocohub/korean-hate-speech | labeled 9,381, unlabeled 2,033,893 | comments + bias/hate labels | GitHub | 연예 뉴스 댓글 기반 한국 온라인 독성 표현 |
| `adlnlp/K-MHaS` | https://github.com/adlnlp/K-MHaS | 109,692 utterances | multi-label hate categories | GitHub/HF | 정치/출신/성별/종교 등 세분화 라벨 |
| `ssu-humane/K-HATERS` | https://github.com/ssu-humane/K-HATERS | repository-based corpus release | target-specific hate speech ratings | GitHub | 타깃별 정밀 평가 reference |
| 모두의 말뭉치 `대화 맥락 추론 말뭉치 2025` | https://kli.korean.go.kr/corpus/main/requestMain.do | 공개 페이지에 총량 미기재 | dialogue + normative/adversarial inference | Request/approval | 명시되지 않은 태도/맥락 추론 평가 |

## Notes
- safety set은 pretraining보다 evaluation, filtering, classifier training에 더 적합합니다.
- 존댓말 일관성과 안전성은 분리하지 말고 함께 보는 편이 좋습니다.

