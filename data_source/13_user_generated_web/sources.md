# User-Generated Web, Blogs, and Community Text

## Why this domain matters
- 한국어 모델이 너무 교과서적이 되는 문제를 줄이려면 블로그, 커뮤니티, 위키, 댓글 같은 사용자 생성 텍스트가 필요합니다.
- 이 영역은 구어와 문어의 혼합체, 인터넷 밈, 장문 설명체, 생활 정보체를 함께 담습니다.

## Priority sources

| Source | URL | Scale | Structure | Access | Korean-specific value |
| --- | --- | --- | --- | --- | --- |
| 모두의 말뭉치 `온라인 게시 자료 말뭉치 2022` | https://kli.korean.go.kr/corpus/main/requestMain.do?lang=en | 공개 페이지에 총량 미기재 | online posts and 게시글 corpus | Request/approval | 커뮤니티형 한국어 문체의 공식 출처 |
| `minpeter/geulgyeol-blog-korean` | https://huggingface.co/datasets/minpeter/geulgyeol-blog-korean | 1.75M rows | blog-style raw text | Hugging Face | 생활형 블로그, 홍보문, 후기 문체 |
| `Dasool/DC_inside_comments` | https://huggingface.co/datasets/Dasool/DC_inside_comments | 111,546 comments | raw community comments | Hugging Face | 비격식, 인터넷 슬랭, 댓글체 |
| `korean-corpus/namu_wiki_512_char_seg` | https://huggingface.co/datasets/korean-corpus/namu_wiki_512_char_seg | 6.23M rows | segmented wiki text | Hugging Face | 나무위키 특유의 설명형/서브컬처 텍스트 |
| `HAERAE-HUB/KOREAN-WEBTEXT` | https://huggingface.co/datasets/HAERAE-HUB/KOREAN-WEBTEXT | 1.28M docs, 2.2B tokens | filtered Korean web corpus | Hugging Face | 대규모 한국어 공개 웹문서 기반 |
| `minpeter/fineweb-2-edu-korean` | https://huggingface.co/datasets/minpeter/fineweb-2-edu-korean | 2.11M rows | scored educational web text | Hugging Face | 정보성 높은 웹텍스트를 우선 확보 가능 |

## Notes
- 이 도메인은 품질 편차가 큰 대신 한국 인터넷 문체를 빠르게 넓힐 수 있습니다.
- 대규모 pretraining source로는 좋지만, 안전성·사실성 필터링을 반드시 같이 설계하는 편이 좋습니다.

