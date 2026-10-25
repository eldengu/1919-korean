# 1919-korean

한국 건국 시기의 문서를 쉬운 현대 한국어로 옮기는 저장소입니다. 미국 건국 문서를 옮기는 [eldengu/1776-korean](https://github.com/eldengu/1776-korean)의 자매 저장소입니다.

- 첫 작품: 이승만(李承晩, Syngman Rhee)의 박사학위 논문 『미국이 중립에 끼친 영향』(*Neutrality as Influenced by the United States*, 1912) — 번역 진행 중

## 폴더

- [`rhee-neutrality-1912/`](rhee-neutrality-1912/) — 『미국이 중립에 끼친 영향』 한국어 번역, 용어집, 저작권 검토, 읽기용 HTML

## 『미국이 중립에 끼친 영향』 (1912)

이승만(1875–1965)이 1910년 프린스턴대학교에 제출해 철학박사 학위를 받고 1912년 프린스턴대학교 출판부에서 펴낸 논문 *Neutrality as Influenced by the United States*를 쉬운 현대 한국어로 새로 옮깁니다. 이 번역은 1912년 영어 원문에서 직접 옮긴 독립 번역이며, 기존에 출간된 한국어 번역본은 참고하지 않았습니다.

### 진행 상황

| 파일 | 내용 | 상태 |
|---|---|---|
| [`00-front-matter.md`](rhee-neutrality-1912/translation/00-front-matter.md) | 속표지, 감사의 말, 목차 | 공개 |
| [`01-neutrality-down-to-1776.md`](rhee-neutrality-1912/translation/01-neutrality-down-to-1776.md) | 제1장 서기 1776년까지의 중립의 역사 | 공개 |
| [`02-neutrality-from-1776-to-1793.md`](rhee-neutrality-1912/translation/02-neutrality-from-1776-to-1793.md) | 제2장 1776년부터 1793년까지의 중립의 역사 | 공개 |
| [`03-neutrality-from-1793-to-1818.md`](rhee-neutrality-1912/translation/03-neutrality-from-1793-to-1818.md) | 제3장 1793년부터 1818년까지의 중립의 역사 | 공개 |
| [`04-neutrality-from-1818-to-1861.md`](rhee-neutrality-1912/translation/04-neutrality-from-1818-to-1861.md) | 제4장 1818년부터 1861년까지의 중립의 역사 | 공개 |
| [`05-neutrality-from-1861-to-1872.md`](rhee-neutrality-1912/translation/05-neutrality-from-1861-to-1872.md) | 제5장 1861년부터 1872년까지의 중립의 역사 | 공개 |
| 제6장 | 요약 | 예정 (내일 공개) |

읽기용 HTML: [`rhee-neutrality-1912/html/`](rhee-neutrality-1912/html/index.html)

### 구성

```
rhee-neutrality-1912/
  translation/   한국어 번역 (Markdown, 장별 파일)
  html/          읽기용 HTML (tools/build_html.py로 생성)
  tools/         빌드 스크립트
  glossary.md    용어집 (영어–한국어 대조, 인명·지명·서명)
  RIGHTS.md      저작권 검토 요약
```

HTML 다시 만들기: `python3 rhee-neutrality-1912/tools/build_html.py` (필요: `markdown-it-py`, `mdit-py-plugins`).

### 원문

- Syngman Rhee, *Neutrality as Influenced by the United States: A Dissertation Presented to the Faculty of Princeton University in Candidacy for the Degree of Doctor of Philosophy*. Princeton: Princeton University Press, 1912.
- 원문 스캔(공개 열람): Internet Archive — https://archive.org/details/neutralityasinf00rheegoog
- HathiTrust — https://hdl.handle.net/2027/hvd.32044038566824

이 저장소에는 영어 원문을 싣지 않습니다(아래 '라이선스와 저작권' 참고). 원문은 위 링크에서 보십시오.

### 번역 원칙

- 합니다체의 쉬운 문장, 소리 내어 읽기 좋은 문장. 긴 영어 문장은 나누되 뜻은 빠짐없이 옮깁니다.
- 영어 단락과 한국어 단락을 1:1로 맞춰 대조 검토가 쉽도록 했습니다.
- 각주의 서지 사항은 원문대로 두고 짧은 한국어 설명을 붙였습니다. 번역자의 설명은 [역주]로 구분합니다.
- 용어는 [`glossary.md`](rhee-neutrality-1912/glossary.md)를 따릅니다.

### 작업 방식

- **초벌 번역:** Claude 모델로 만들었습니다(앞부분·제1장 claude-opus-5-5, 제2장부터 claude-sonnet-5-5).
- **문체 다듬기:** humanize-korean 도구로 번역투와 어색한 문장을 보수적으로 다듬었습니다(뜻·용어·각주는 그대로 유지).
- **검토:** AI 어시스턴트가 영어 원문과 단락별로 대조해 검토·수정했습니다. 사람 전문가의 검수는 아직 거치지 않았으므로, 오류를 발견하시면 이슈로 알려 주십시오.

## 라이선스와 저작권

- **한국어 번역문, 역주, 용어집:** © 2026 1919-korean 번역 프로젝트 (eldengu), [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.ko). 재사용할 때는 "원저 이승만(1912), 번역 1919-korean 번역 프로젝트 (eldengu), CC BY 4.0"과 같이 원저자와 번역자, 라이선스를 밝혀 주십시오. 전문은 [LICENSE](LICENSE)를 보십시오.
- **영어 원문:** 미국에서는 퍼블릭 도메인입니다(1912년 미국 출판). 한국에서는 2035년 12월 31일까지 보호되는 것으로 보이므로 이 저장소에 원문을 싣지 않고 위 링크(Internet Archive, HathiTrust)로 안내합니다.
- CC BY 4.0은 번역자가 가진 권리에만 적용되며, 이승만의 원저작물에 대한 권리를 부여하지 않습니다. 자세한 내용은 [RIGHTS.md](rhee-neutrality-1912/RIGHTS.md)를 보십시오.
