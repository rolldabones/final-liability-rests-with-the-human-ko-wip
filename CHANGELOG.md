# Changelog

All notable changes to this repository are documented here. Versioning follows [Semantic Versioning](https://semver.org/). The README, CITATION.cff and this file version in lockstep; prior versions are superseded, never silently overwritten. Status until the author's line review is complete: 초벌 번역, 저자 검토 중 (machine draft under the author's review).

## v0.2.1 (2026-11-10)

Patch release, 10 November 2026 (KST): the citations approved. Michael Paik approved the 422 citation-bearing blocks of the Korean text (Legal Terms and Citations v0.1, Part C) on 10 November 2026, with no correction. No change to the text. README (what remains: the line review of the rest of the text) and CITATION.cff to v0.2.1, in lockstep. Status unchanged: 초벌 번역, 저자 검토 중 (machine draft under the author's review).

## v0.2.0 (2026-11-10)

Minor release, 10 November 2026 (KST): the term rulings. Michael Paik approved every recommendation in Part A of Legal Terms and Citations v0.1 on 10 November 2026, the six consistency terms of v0.1.0 included. Applied by script (`apply_rulings.py`) to the batch output and the edition re-assembled, so v0.1.0's hand edits carry over; 183 changes, each checked against its English context. Status unchanged: 초벌 번역, 저자 검토 중 (machine draft under the author's review).

- **deployer** = 배포자: 11 occurrences of 배치자 (Chapters 13 and 19, Appendix H).
- **General Counsel** = 법무총괄: 22 occurrences of 최고법무책임자 (Chapter 12) and 법무총괄책임자 (Appendix J, Parts 1 to 3), with the following particle adjusted; every one renders "General Counsel" in the English, none "Chief Legal Officer".
- **risk appetite** = 리스크 선호도: 26 occurrences of 리스크 성향, particles adjusted; the Conclusion's heading now reads 어떤 리스크 선호도도 정당화할 수 없는 것, and the table of contents with it.
- **trustworthiness** = 신뢰가능성: 13 changes, only in blocks where the English says trustworthiness and not reliability; the adjective "trustworthy" keeps 신뢰할 수 있는.
- **operational catechism** = 운영 교리문답: 28 changes, including Chapter 5's 운영 문답서 and the bare 문답 where the English says catechism (the Conclusion, Appendix N, Appendices I and J).
- **assumption register** = 가정 등록부 (2) and **agent registry** = 에이전트 레지스트리 (8), following the appendix titles.
- **validation** = 확인: 65 changes, only in blocks where the English says validation and not verification, so the TEVV pair 검증·확인 is untouched. Exception: training, validation and test data sets keep 학습, 검증, 테스트 데이터셋, the standard rendering of that phrase. Flagged for the line review: a block that also uses 검증 for another English word (check, test) would have changed with it.
- **QMS** = 품질경영시스템: 5 occurrences of 품질관리시스템, including the US FDA Quality Management System Regulation in Chapter 20.
- **Soetsu Yanagi** = 야나기 무네요시 (2); **KRW 30 million** = 3,000만 원 (1).
- Parts regenerated; `manuscript/` and `master-reference/` confirmed with the account's `split_markdown.py --verify`, byte for byte. README (term rulings done; what remains is the line review, citations first) and CITATION.cff to v0.2.0, in lockstep.

## v0.1.0 (2026-11-10)

First release, 10 November 2026 (KST): the Korean machine draft of English v1.12.0, published for the author's line review. Decided by Michael Paik on 10 November 2026: this repository, the Informed Intent gloss 정보에 기반한 의도, a fresh translation from v1.12.0 with the approved v0.2 title page carried over, and Appendices I and J translated and shipped here.

### Source and run
- **Source.** English v1.12.0, tag `v1.12.0` at commit 0e94a8d of [final-liability-rests-with-the-human-book-wip](https://github.com/rolldabones/final-liability-rests-with-the-human-book-wip): the 32 manuscript parts after the table of contents, the six parts of `master-reference/` (Appendix J, v7.14) and `AI_Audit_Due_Diligence_Checklist_v5_3.md` (Appendix I, v5.3) split in two at its section 5. A SHA-256 of each source text is kept with the batch file.
- **Run.** Message Batch `msgbatch_01GxxbUuDg3t7pPaMY8Xkngt`, 40 requests to claude-opus-5-5 with `max_tokens` 128,000 (the model's maximum output), submitted 10 November 2026 at 14:47:57 KST and reported ended at the 14:53 poll. 40 succeeded; every request stopped on `end_turn`, none on `max_tokens`; 399,585 input and 663,230 output tokens; USD 7.43, the fall in the Console credit balance across the run.
- **Instructions.** Job E of the 10 November 2026 review build (register 한다체; doctrine names in English with the Korean gloss at first use in each file; the closing line in English; fixed terms), updated to v1.12.0. Added for this run, as assumptions awaiting the author's ruling: principal-agent = 본인-대리인 (an AI agent is always 에이전트); compliance theater = 보여주기식 컴플라이언스; Fast AI = 빠른 AI; Three Lines Model = 3선 모델; Punchlist = 펀치리스트; Unknown = 알 수 없음(Unknown).
- **Recorded error, no effect found.** The instructions for the two instruments, as submitted, named Appendix I as the Master Reference and Appendix J as the Checklist, the reverse of the English README; the correction was made three minutes after submission. The instruments' source texts carry no Appendix I or J label and neither do their translations, and every 부록 I and 부록 J in the manuscript was checked in context and refers to the right instrument. The batch's request IDs carry the swap (I- holds the Master Reference, J- the Checklist); assembly maps them to the right files, and the as-submitted request file is kept.

### Checks
- Every file against its English source by script: heading levels in order, table rows, link targets, GRCnext™ marks and the closing line all match; the Korean-to-English ratio of non-space characters lies between 0.43 and 0.59 across the 40 files, so no file is abridged (Appendix F's apparent shortfall is whitespace padding in the English tables).
- Client = 고객사 wherever the English capitalizes Client; 고객 elsewhere renders "customer".
- 422 blocks carrying a legal citation: every number in the English block checked against the Korean block. Eight flags, each read by hand and each a rendering (ranges as 제24조~제26조, KRW 30 million as 3,000만 원, EUR 15M as 1,500만 유로), not an error.
- `manuscript/` (33 parts) and `master-reference/` (six parts) confirmed with the account's `split_markdown.py --verify`: each set rebuilds its file of record byte for byte.

### Assembled, not translated
- Title page: the approved v0.2 title page (title, the English title as second line, subtitle, author and position), with the status label added.
- Table of contents: generated from the translated part and chapter headings, so it cannot disagree with them; Informed Intent glossed at its first appearance there.
- Parts named after their English counterparts, with the account's navigation sentinels and index format, so the account's verifier applies unchanged.

### Hand edits to the model output
- Chapter 4: two em dashes the model introduced (the English has none) replaced by a parenthesis and by commas.
- Appendix J: its title rendered 마스터 참조 파일 changed to 마스터 레퍼런스 파일, the form the manuscript uses.

### Open for the author's review
- Terms needing a ruling, with recommendations: deployer, General Counsel, risk appetite, trustworthiness, operational catechism, the register and registry names, verification and validation, QMS, Soetsu Yanagi, money style, and the consistency terms above. Every ruling is applied across all files in one pass and logged here.
- The line review itself, legal terms and citations first. On completion the status label changes and the edition is released as v1.0.0.

**Final Liability rests with the Human.**
