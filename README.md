# 최종 책임은 인간이 진다

*Final Liability Rests with the Human*

**AI 에이전트 시대, 거버넌스를 갖춘 AI를 위한 실무 안내서**

**백선우**
GRC Solutions Korea 대표이사(CEO)

**v0.3.2 · 2026년 11월 26일 · 라이선스: [CC BY-NC-SA 4.0](LICENSE.md) · 변경 기록: [CHANGELOG.md](CHANGELOG.md) · [English edition](https://github.com/rolldabones/final-liability-rests-with-the-human-book-wip)**

> **번역 및 검토 현황: 초벌 번역, 저자 검토 중 (machine draft under the author's review).** 이 저장소의 한국어판은 영문 원고를 AI로 번역한 초벌 번역본으로, 현재 저자의 검토가 진행 중입니다. 아직 최종 번역본은 아니며, 검토가 완료되기 전까지는 영어 원문을 공식 기준으로 합니다. 한국어판과 영어 원문 사이에 차이가 있는 경우 영어 원문이 우선합니다.

[English below](#english)

---

## 이 저장소에 관하여

이 저장소는 『Final Liability Rests with the Human』의 한국어판을 제공합니다. 영어판은 [final-liability-rests-with-the-human-book-wip](https://github.com/rolldabones/final-liability-rests-with-the-human-book-wip)에 있습니다.

한국어판은 2026년 11월 10일자 영문 원고 v1.12.0을 기준으로 번역했습니다. 다만 제15장은 2026년 11월 16일자 영문 원고 v1.12.3의 정정 사항을 반영했으며, 여기에는 2026년 8월 13일 *Boeing* 관련 결정이 포함됩니다. 같은 날 영문 원고 v1.12.4부터 v1.12.6까지의 정정 사항도 번역하여 반영했고, 반영 범위는 [CHANGELOG.md](CHANGELOG.md)에 기록되어 있습니다.

이 책은 비상업적 목적으로 무료로 공개됩니다.

이 책의 세 가지 핵심 원칙인 **Slow AI**(슬로우 AI), **Informed Intent**(정보에 기반한 의도), **Final Liability**(최종 책임)는 영문 명칭을 그대로 사용하되, 각 파일에서 처음 등장할 때 한국어 설명을 덧붙였습니다. 각 원칙의 규범적 내용은 계정 전체의 기준 문서인 [DOCTRINE.md](https://github.com/rolldabones/rolldabones/blob/main/DOCTRINE.md)에서 확인할 수 있습니다.

## 파일

| 파일 | 내용 |
|---|---|
| [`Final_Liability_Rests_with_the_Human_KO.md`](Final_Liability_Rests_with_the_Human_KO.md) | 원고의 기준 파일입니다. 인용하거나 내려받을 때는 이 파일을 사용합니다. 서문, 22개 장, 결론, 에필로그, 부록 D, E, F, H, K, L, N |
| [`manuscript/`](manuscript/README.md) | 브라우저에서 읽기 위한 33개 부분입니다. 영어판의 같은 이름 부분과 하나씩 대응하며, 모두 합치면 기준 파일과 바이트 단위까지 같아집니다 |
| [`AI_Audit_Due_Diligence_Checklist_v5_3_KO.md`](AI_Audit_Due_Diligence_Checklist_v5_3_KO.md) | 부록 I, AI 감사 및 실사 체크리스트 v5.3 |
| [`AI_GRC_Master_Reference_v7_14_KO.md`](AI_GRC_Master_Reference_v7_14_KO.md) | 부록 J, AI GRC 마스터 레퍼런스 v7.14의 기준 파일입니다. 읽기용 6개 부분은 [`master-reference/`](master-reference/README.md)에 있습니다 |

부록 M(GRC 워크북)은 영어판으로만 [grc-workbook](https://github.com/rolldabones/grc-workbook)에 있습니다.

## 번역 방식

이 책은 AI를 활용하여 번역했으며, 저자가 번역 결과를 검토하는 방식으로 작업했습니다. 이 책이 AI 작업에 요구하는 방식 그대로, AI가 생성한 번역문은 초안이며 최종적인 판단과 책임은 저자에게 있습니다.

- 2026년 11월 10일, Claude API의 Message Batches 기능을 통해 Claude Opus 5.5 모델(claude-opus-5-5)에 총 40건의 번역 요청을 보냈습니다. 번역 대상은 본문 32개 파일과 부록 J의 6개 부분, 부록 I의 2개 부분입니다. 40건 모두 출력 토큰 한도에 따른 중단 없이 완료되었습니다.
- 번역에 앞서 문체(본문은 한다체), 세 가지 핵심 원칙의 명칭, 주요 용어의 번역 방식, 조문 번호, 사건명 및 날짜의 표기 원칙을 정했습니다.
- 주요 용어는 일관되게 번역했습니다. 예를 들어 governance, risk management and compliance는 '거버넌스, 리스크 관리 및 컴플라이언스'로, Client는 '고객사'로 번역했습니다.
- 자동화 스크립트를 이용해 모든 파일의 제목 체계, 표의 행, 링크, 상표 표기 및 맺음말이 영어 원문과 일치하는지 확인했습니다. 인용문이 포함된 422개 블록에 대해서는 원문에 기재된 숫자가 한국어 번역문에도 모두 반영되었는지 검증했습니다.
- 2026년 11월 10일, 저자가 법률 용어 목록의 권고안을 검토·승인했으며, 확정된 번역 용어를 전체 파일에 일괄 적용했습니다(v0.2.0).
- 번역된 장 제목을 바탕으로 스크립트를 이용해 목차를 생성했습니다. 이후 수작업으로 수정한 사항은 [CHANGELOG.md](CHANGELOG.md)에 하나하나 기록했습니다.
- 2026년 11월 25일, 한국어 독자의 의견을 반영하여 한국어판 제목과 부제, 그리고 이 안내문의 문체를 다듬었습니다(v0.3.0).

현재 저자의 최종 검토가 진행 중입니다. 용어 선정과 인용 관련 검토는 2026년 11월 10일 완료되었으며, 원고 전체에 대한 문장별 검토가 남아 있습니다. 검토가 완료되면 번역 상태를 갱신하고 정식 버전(v1.0.0)을 공개할 예정입니다.

## 인용

> 백선우(Son-U Michael Paik). 『최종 책임은 인간이 진다』(*Final Liability Rests with the Human*, 한국어판), v0.3.2, 초벌 번역, 저자 검토 중. GRC Solutions Korea, 2026. https://github.com/rolldabones/final-liability-rests-with-the-human-ko-wip

내용을 인용할 때는 기준 텍스트인 영어판을 인용해 주십시오. 기계가 읽을 수 있는 인용 정보는 [CITATION.cff](CITATION.cff)에 있습니다.

## 라이선스

[CC BY-NC-SA 4.0](LICENSE.md). 영어판과 같은 라이선스입니다. 상업적 이용은 [LICENSING.md](https://github.com/rolldabones/rolldabones/blob/main/LICENSING.md)를 따릅니다. 이 저장소의 내용은 법률 자문이 아니며, 이를 읽는 것만으로 변호사와 의뢰인 관계가 성립하지 않습니다.

---

## English

**Status: 초벌 번역, 저자 검토 중 (machine draft under the author's review).** This repository holds the Korean edition of *Final Liability Rests with the Human*, translated from English v1.12.0 (10 November 2026), with Chapter 15 carrying the correction of English v1.12.3 (16 November 2026) in translation, and the corrections of English v1.12.4 to v1.12.6 carried the same day as the CHANGELOG records. On 25 November 2026, after feedback from Korean readers, the Korean title became 최종 책임은 인간이 진다 (previously 최종 책임은 인간에게 있다), the subtitle was revised and the Korean README moved to the polite register (합니다체); the manuscript stays in 한다체. It is a machine draft that the author is reviewing line by line, not a finished translation. Until that review is complete, the [English edition](https://github.com/rolldabones/final-liability-rests-with-the-human-book-wip) is the text of record and governs wherever the two differ.

**What is here.** The manuscript of record, `Final_Liability_Rests_with_the_Human_KO.md` (Preface, 22 chapters, Conclusion, Epilogue and Appendices D, E, F, H, K, L and N), with 33 reading parts under `manuscript/` that correspond one for one to the English parts and rebuild the file of record byte for byte. Appendix I, the AI Audit and Due Diligence Checklist v5.3, and Appendix J, the AI GRC Master Reference v7.14 (six reading parts under `master-reference/`), are translated alongside. Appendix M, the GRC Workbook, stays in English in [grc-workbook](https://github.com/rolldabones/grc-workbook).

**How it was made.** The book was translated the way it says AI work should be governed: the model's output is a draft and a named human answers for the result. On 10 November 2026, 40 requests went to Claude Opus 5.5 (claude-opus-5-5) through the Claude API Message Batches: 32 manuscript files, six parts of Appendix J and two of Appendix I. All 40 ran to completion without reaching their output limit. The instructions fixed the register (한다체), the doctrine names (in English, with the Korean gloss at first use in each file) and the fixed terms. A script compared every file with its English source for headings, table rows, links, trademark marks and the closing line, and checked that every number in each of the 422 citation-bearing blocks appears in the Korean. The author approved the recommended term rulings on 10 November 2026, and they are applied across every file (v0.2.0). The table of contents is generated from the translated chapter headings. Every hand edit is logged in the CHANGELOG.

**What remains.** The author approved the term rulings and the 422 citation blocks on 10 November 2026; his line review of the rest of the text remains. The status label changes, and the edition is released as v1.0.0, when that review is complete.

**Cite** the English edition for its content. Nothing here is legal advice, and reading it creates no attorney-client relationship.

## Part of the ecosystem

This repository is the Korean edition of the account's doctrinal core. The canonical map of all repositories is [ECOSYSTEM.md](https://github.com/rolldabones/rolldabones/blob/main/ECOSYSTEM.md) in the profile repository. The three doctrines are used as stated in [DOCTRINE.md](https://github.com/rolldabones/rolldabones/blob/main/DOCTRINE.md); this edition translates them and adds no doctrine (ECOSYSTEM.md protocol item 6).

Nearest neighbors:
- [final-liability-rests-with-the-human-book-wip](https://github.com/rolldabones/final-liability-rests-with-the-human-book-wip): the English edition and text of record, from which this edition is translated

---

**Final Liability rests with the Human.**
