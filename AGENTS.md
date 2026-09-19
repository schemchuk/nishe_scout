# AI Agent Rules — Niche Scout

Цей файл є операційною інструкцією для Kimi, Claude Code та інших AI-агентів.

## 1. Головне правило

**Не пиши production/MVP code, поки `DECISION.md` не має `DECISION: BUILD`.**

Research first. Code second.

## 2. Не вигадуй докази

Заборонено:

- вигадані reviews;
- вигадані installs;
- вигадані conversion rates;
- вигадані ranking signals;
- вигадані competitor features;
- вигадані marketplace policies.

Кожне external factual claim → URL + дата перевірки.

## 3. Пріоритет джерел

1. Офіційна документація marketplace.
2. Реальна сторінка app у marketplace.
3. Офіційні announcement/changelog.
4. Надійні вторинні джерела.
5. Reddit/G2/форум — тільки для customer voice/pain або слабшого evidence.

Якщо джерела суперечать одне одному — показати суперечність, не вибирати зручне твердження мовчки.

## 4. Порядок роботи

### Phase A — Marketplace screening

Перевірити Wix / Shopify / Atlassian / WordPress.

Потрібно встановити:

- search/discovery;
- billing model;
- review/install signals;
- new entrants;
- platform requirements;
- organic discovery evidence.

### Phase B — Select one marketplace

Після screening вибрати **один** marketplace для deep research.

Не досліджувати всі marketplace паралельно тижнями.

### Phase C — Keyword research

Досліджувати customer queries, а не просто categories.

### Phase D — Pain + switching

Шукати повторюваний pain і switching evidence.

### Phase E — Wedge

Сформулювати конкретний reason-to-install.

### Phase F — Decision

Заповнити `DECISION.md`.

## 5. Veto rules

Якщо є явний FAIL по одному з основних gates — не компенсувати його іншими плюсами.

Особливо:

- Solo Gate = veto.
- Marketplace commercial fit = veto.
- Organic discovery evidence = veto для цієї моделі.
- Wedge = veto.

## 6. Не створювати document factory

Не створювати багато дублюючих markdown-файлів.

Основний research — `RESEARCH.md`.

Основне рішення — `DECISION.md`.

Новий файл створювати тільки коли він має окреме операційне призначення.

## 7. Заборонені аргументи

Не писати:

- «ринок величезний, тому шанс є»;
- «конкурентів багато, але це добре»;
- «поставимо низьку ціну»;
- «додамо AI»;
- «після MVP займемося acquisition»;
- «отримаємо перші 50 users somehow».

Кожен такий висновок має бути замінений доказом або гіпотезою з test method.

## 8. Що робити при відсутності даних

Писати:

`UNKNOWN — NEEDS EVIDENCE`

а не заповнювати прогалину припущенням.

## 9. Стиль рішення

Фінал research має бути коротким:

`BUILD / REJECT / NEEDS EVIDENCE`

із 3–7 найсильнішими доказами.
