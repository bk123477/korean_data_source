# Conversation, Honorifics, and Everyday Speech

## Why this domain matters
- Korean conversational quality depends heavily on honorifics, turn-taking, ellipsis, indirectness, and role-sensitive phrasing.
- This domain should be the first reference set when building Korean chat or assistant datasets.

## Priority sources

| Source | URL | Scale | Structure | Access | Korean-specific value |
| --- | --- | --- | --- | --- | --- |
| AI Hub `한국어 대화` | https://aihub.or.kr/aidata/85 | 50만 건 이상 대화 | intent, entity, thesaurus, multi-domain dialogue | Download/API, approval required | 민원·소상공인 대화라서 한국식 문의, 요청, 존칭 패턴이 강함 |
| AI Hub `한국어 대화 데이터셋` | https://www.aihub.or.kr/aihubdata/data/view.do?aihubDataSe=extrldata&currMenu=118&dataSetSn=272&topMenu=100 | 응급 748 멀티턴, 오피스 10,202 멀티턴, 46,414 대화쌍 | scenario-based multi-turn dialogue | Download, approval required | 상황형 한국어 대화, 업무/응급 맥락 |
| AI Hub `감성 대화 말뭉치` | https://www.aihub.or.kr/aihubdata/data/view.do?aihubDataSe=data&currMenu=115&dataSetSn=86&topMenu=100 | 코퍼스 27만 문장, 음성 1만 문장 | utterance + emotion-oriented conversation | Download/API, approval required | 세대별 감성 표현, 위로/공감 어투 |
| AI Hub `생성형AI 한국어 SNS 멀티턴 대화 데이터` | https://www.aihub.or.kr/aihubdata/data/view.do?aihubDataSe=&currMenu=115&dataSetSn=71694&topMenu=100 | 196,235 세션, 3,246,886 발화 | CSV/JSON, 2~3인 SNS-style dialogue | Download, approval required | 구어체, 축약, 온라인 대화체 보강에 유리 |
| 모두의 말뭉치 `일상 대화 말뭉치 2024` | https://kli.korean.go.kr/corpus/main/requestMain.do | 공개 페이지에 총량 미기재 | daily conversation corpus | Request/approval | 실제 일상 대화 기반, 한국어 구어 전사 참고용 |
| 모두의 말뭉치 `일상 대화 말뭉치 2023` | https://kli.korean.go.kr/corpus/main/requestMain.do?lang=en | 공개 페이지에 총량 미기재 | dialogue transcription corpus | Request/approval | 연도별 축적이라 세대/상황 표현 비교에 좋음 |
| 모두의 말뭉치 `일상 대화 말뭉치 2021` | https://kli.korean.go.kr/corpus/main/requestMain.do?lang=en | 공개 페이지에 총량 미기재 | dialogue transcription corpus | Request/approval | 협력적 대화 요약 원천으로도 활용 가능 |
| 모두의 말뭉치 `온라인 대화 말뭉치` | https://kli.korean.go.kr/corpus/main/requestMain.do?lang=en | 공개 페이지에 총량 미기재 | online text-message style conversations | Request/approval | 메신저/채팅체, 축약, 비격식 표현 보강 |
| 모두의 말뭉치 `무형 대용어 복원 말뭉치 2024` | https://kli.korean.go.kr/corpus/main/requestMain.do?lang=en | 공개 페이지에 총량 미기재 | zero-anaphora restoration corpus | Request/approval | 주어·목적어 생략이 잦은 한국어 대화 보정에 유용 |
| 모두의 말뭉치 `지역어 말뭉치 2021` | https://kli.korean.go.kr/corpus/main/requestMain.do?lang=en | 10개 지역, 3세대 조사 기반 | oral dialect survey corpus | Request/approval | 표준어 편향을 줄이고 지역 구어 특성 반영 가능 |
| 모두의 말뭉치 `협력적 대화 요약 말뭉치 2025` | https://kli.korean.go.kr/corpus/main/requestMain.do | 510건 | conversation + per-speaker and global summaries | Request/approval | 장문 대화 흐름, 화자별 요약, 협력적 상호작용 |
| 모두의 말뭉치 `대화 맥락 추론 말뭉치 2025` | https://kli.korean.go.kr/corpus/main/requestMain.do | 공개 페이지에 총량 미기재 | dialogue context + inference annotations | Request/approval | 생략, 함축, 맥락 추론, 정규적/적대적 해석 |
| `songys/ChatbotData` | https://huggingface.co/datasets/songys/ChatbotData | 약 11.8k 문답 | question, answer, label | Hugging Face | 가벼운 일상/감정형 챗봇 문답 seed |
| `jojo0217/korean_safe_conversation` | https://huggingface.co/datasets/jojo0217/korean_safe_conversation | 26,979 rows | instruction, input, output JSONL | Hugging Face | 한국어 친화적 응답체와 안전 응답 스타일 참고용 |
| `AIWORKX/KoSGD` | https://huggingface.co/datasets/AIWORKX/KoSGD | 84,594 turns | schema-guided task-oriented dialogue | Hugging Face | 다중 서비스 도메인의 한국어 목적지향 대화 |
| `NLPBada/korean-persona-chat-dataset` | https://huggingface.co/datasets/NLPBada/korean-persona-chat-dataset | 8.26k train | persona + session dialogue | Hugging Face | 페르소나 반영 대화체 실험용 |

## Notes
- 존댓말 일관성 검증에는 `일상 대화`, `한국어 대화`, `감성 대화`, `SNS 멀티턴`을 함께 보는 편이 좋습니다.
- 한국어 대화체를 더 자연스럽게 만들려면 `온라인 대화`, `무형 대용어 복원`, `지역어 말뭉치`를 같이 보는 편이 좋습니다.
- 안전하고 무난한 assistant tone reference가 필요하면 `korean_safe_conversation`도 보조 seed로 쓸 수 있습니다.
- 실제 학습용 raw corpus와 별개로 `대화 맥락 추론`과 `협력적 대화 요약`은 evaluation/reference 세트로 매우 유용합니다.
