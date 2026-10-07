# ДЗ-2. Анатомия статьи: разбор структуры по образцу

**Цель.** Разобрать на реальной принятой статье, как она устроена: из каких разделов состоит, как Introduction подводит к вкладу, где этот вклад подтверждается и как статья выполняет требования конференции. Этот разбор станет образцом для заготовки вашей собственной статьи в ДЗ-3.

> **Язык ответа: английский.** Все ответы пишите на английском, так же как будете писать саму статью. Цитаты из статьи приводите как есть.

## Что нужно сделать

### 1. Выберите статью-образец

Нужна статья **по теме, близкой к вашей** (по теме ДЗ-1), принятая на ведущую конференцию **в 2025–2026 годах**. Более ранние статьи не принимаются: требования к оформлению и обязательным разделам меняются каждый год.

Где искать:

- **ACL, EMNLP, NAACL, EACL, Findings** (NLP): ACL Anthology, https://aclanthology.org/. На странице события, например https://aclanthology.org/events/acl-2025/, видны все треки: main (long/short), Findings, demo, industry, workshops.
- **ICLR**: OpenReview, https://openreview.net/group?id=ICLR.cc/2026/Conference и https://openreview.net/group?id=ICLR.cc/2025/Conference. Бонус: там же открыты ревью и ответы авторов.
- **ICML**: PMLR, https://proceedings.mlr.press/v306/ (ICML 2026) и https://proceedings.mlr.press/v267/ (ICML 2025).
- **NeurIPS**: https://proceedings.neurips.cc/ (2025) и OpenReview https://openreview.net/group?id=NeurIPS.cc/2025/Conference. Для датасетов и бенчмарков смотрите Datasets & Benchmarks Track.
- **CVPR** (CV): CVF Open Access, https://openaccess.thecvf.com/CVPR2026 и https://openaccess.thecvf.com/CVPR2025.

Укажите название, конференцию, год, трек и ссылку. Одним предложением объясните, почему статья подходит как образец: близкая тема, тот же тип вклада.

### 2. Составьте карту структуры

Перечислите разделы основного текста. Для каждого укажите примерный объём в страницах и одной фразой его функцию. Отдельной строкой в конце таблицы укажите **Appendix**: его примерный объём и перечень материалов, которые туда вынесены.

*Пример:* ` 3 | Overview of MERA Multi | ~4 pp. | describes the benchmark itself: taxonomy, metrics, scoring, leakage protection.`

*Пример Appendix:* `Appendix A–F | ~34 pp. | Dataset cards, extended taxonomy, leakage detection method, prompts, and baseline configs.`

### 3. Выпишите Introduction по блокам

Выпишите номер абзаца, начало первого предложения абзаца в кавычках и сопоставьте его с блоком схемы из лекции:

- **Problem**: постановка задачи и её актуальность;
- **Gap**: существующие подходы и их недостатки;
- **"In this paper"**: что предлагают авторы;
- **Contributions**: перечень вклада;
- **Figure 1**: схема на первой странице.

Если какого-то блока нет или два блока слиты в один абзац, отметьте это.

*Пример:* `Para 2 | "Existing Russian-specific benchmarks, including TAPE ... focus exclusively on text-based tasks..." | Gap + "In this paper" (merged: the gap and the proposal share one paragraph).`

### 4. Проследите каждый пункт contribution

Для каждого пункта из списка contributions укажите:

- **где о нём говорится в статье**: раздел, таблица, рисунок, приложение;
- **отзеркален ли он в Conclusion**: да или нет.

Затем проверьте обратное направление (Reverse check) и напишите 1–2 предложениями: есть ли в Conclusion утверждения, которых нет среди contributions.

*Пример:* `(iii) baseline results | §4, §5, Table 6, App. F | Conclusion: NO, not mentioned.`

### 5. Сравните требования конференции со статьёй

Откройте Call for Papers этой конференции нужного года и выпишите конкретные требования:

- лимит страниц;
- обязательные разделы (Limitations, Ethics, Impact Statement, Reproducibility Statement);
- что не входит в лимит;
- нужен ли checklist.

Затем проверьте, как статья выполняет каждое требование.

*Пример:* `EACL 2026 CfP: "Limitations" section is mandatory, otherwise desk reject; not counted toward the page limit | Paper: ✓ Limitations section with 2 paragraphs (task coverage; HW/SW reproducibility).`

### 6. AI usage

В 1–2 предложениях опишите, какими AI-инструментами вы пользовались при выполнении задания и как именно они помогли (или почему не пользовались). Если пользовались, проверьте, что номера разделов и цитаты в ответе совпадают со статьёй.

## Формат сдачи и критерии оценивания

* **Формат файла:** PDF, строго **1–2 страницы A4** (сдача через систему проверки).
* **Язык ответа:** Английский. Пункты 2–5 оформляются компактными таблицами.
* **Дедлайн:** 13.10.26 г. 23:59. 

Ваш отчёт должен состоять из 6 разделов, которые оцениваются по следующим критериям:

**1. Paper Selection [0–1 балл]**
* **1 балл:** статья строго 2025–2026 гг., принята на ведущую конференцию, релевантна вашей теме, приведено внятное обоснование выбора.
* **0 баллов:** статья старше 2025 г., препринт без подтверждения публикации, статья не с ведущей конференции либо обоснование отсутствует.

**2. Structure Map [0–2 балла]**
* **2 балла:** полная таблица всех разделов статьи с объёмами в страницах и их функциями. Appendix вынесен отдельной строкой (указан его объём и что конкретно в него вынесено).
* **1 балл:** пропущен 1–2 раздела, не указан объём страниц либо забыт Appendix.
* **0 баллов:** разделы статьи не выписаны или пересказаны одной абстрактной фразой.

**3. Introduction by Blocks [0–2 балла]**
* **2 балла:** поабзацный разбор с реальными цитатами начал предложений (не пересказ). Смысловые блоки (*Problem, Gap, In this paper, Contributions, Figure 1*) определены корректно.
* **1 балл:** пропущены абзацы, вместо цитат дан пересказ либо допущены ошибки в определении блоков.
* **0 баллов:** абзацы не сопоставлены со схемой.

**4. Contribution Alignment [0–2 балла]**
* **2 балла:** все заявленные пункты вклада привязаны к разделам/таблицам статьи. Проверен Conclusion (`Yes`/`No`). Выполнен Reverse check (найдены расхождения или явно зафиксировано их отсутствие).
* **1 балл:** привязка поверхностная (нет ссылок на конкретные разделы/таблицы) либо забыт Reverse check.
* **0 баллов:** сопоставление вклада отсутствует.

**5. Conference Requirements [0–2 балла]**
* **2 балла:** требования взяты из официального CfP конференции нужного года (лимиты, обязательные разделы, чек-листы) и честно сопоставлены со статьёй.
* **1 балл:** требования выписаны в общих чертах, не привязаны к конкретному году конференции либо пропущены ключевые пункты (лимиты, чек-листы).
* **0 баллов:** требования CfP не проанализированы.

**6. AI Usage & Formatting [0–1 балл]**
* **1 балл:** соблюдён объём (1–2 стр. PDF), язык строго английский, честно описано использование AI (или его отсутствие).
* **0 баллов:** нет раздела про AI, превышен лимит объёма (>2 стр.) или отчёт сдан на русском языке.

**ИТОГО: 10 баллов**

---

## Пример выполнения

**Paper:** *Multimodal Evaluation of Russian-language Architectures* (MERA Multi), EACL 2026, Main, Long Papers. https://aclanthology.org/2026.eacl-long.94/
*Why:* a benchmark paper for Russian; this is a good model for students whose main contribution is a dataset or benchmark.

**Structure map**

| Section | Size | Function |
|---|---|---|
| 1 Introduction | ~1 p. | gap: no multimodal benchmarks for Russian → MERA Multi; 4 contributions; Figure 1 |
| 2 Related Work | ~1 p. | text-based vs multimodal benchmarks; Table 1 compares with 10 benchmarks |
| 3 Overview of MERA Multi | ~4 pp. | structure, skill taxonomy, metrics and scoring, submission, leakage protection |
| 4 Baselines | ~0.5 p. | 50+ open models + GPT-4.1; human baselines |
| 5 Results | ~1 p. | leaderboard (Table 6), 2 "Takeaway" boxes |
| Conclusion | ~0.3 p. | summary + future work |
| Limitations / Ethical Statement | ~0.7 p. | outside the page limit |
| Appendix A–F | ~34 pp. | dataset cards, taxonomy, leakage method, judge model, prompts, baselines |

*Observation:* the main text is about 8 pages, while the appendix is about 4 times longer. In practice this is the "в любой непонятной ситуации — в аппендикс" principle from the lecture.

**Introduction by blocks**

| Paragraph | Opening | Block |
|:---:|---|---|
| **Para 1** | *"Recent breakthroughs in generative AI..."* | **Problem:** Multimodal progress requires evaluation, but existing benchmarks ignore Russian. |
| **Para 2** | *"Existing Russian-specific benchmarks... focus exclusively on text-based tasks..."* | **Gap + "In this paper"** (merged: notes text-only limitations and introduces MERA Multi). |
| **Para 3** | *"More specifically, our contributions are fourfold:"* | **Contributions** (explicit list of 4 key contributions). |
| **Para 4** | *"Additionally, we provide a standardized codebase..."* | **Release Statement:** Open codebase, platform, and license. |
| **Fig. 1** | *Caption: "Overview of MERA Multi framework..."* | **Figure 1 / Teaser:** Conceptual diagram on page 1–2. |

**Contribution Alignment**

| Contribution | Where in the paper | In Conclusion? |
|---|---|---|
| (i) taxonomy & methodology | §3.2–3.3, Table 3, App. B | Yes |
| (ii) 18 novel datasets | §3.1, Table 2, App. A | Yes |
| (iii) baseline results | §4–5, Table 6, App. F | No |
| (iv) leakage analysis & watermarking | §3.4, Tables 4–5, App. C | No |

*Reverse check:* the Conclusion highlights the codebase and the submission platform, but they are not in the contribution list (only in the "Additionally" paragraph). Contributions (iii) and (iv) are not mirrored in the Conclusion. This is exactly what is worth fixing in your own paper.

**Conference requirements vs paper**

| EACL 2026 CfP requirement | Paper |
|---|---|
| Long paper: ≤ 8 pages of content (+1 page for camera-ready) | ✓ ~8 pages of main text |
| References and appendices unlimited | ✓ ~34-page appendix |
| "Limitations" mandatory, otherwise desk reject; outside the page limit | ✓ 2 paragraphs |
| Ethics section (optional) | ✓ Ethical Statement: bias out of scope, annotator pay (→ App. F.2), AI writing assistance |
| Responsible NLP checklist | ✓ published as an attachment in the Anthology |

**AI usage:** e.g., *"I used Claude to locate the CfP requirements and to draft the tables; all section numbers and quotes were checked manually against the PDF."*
