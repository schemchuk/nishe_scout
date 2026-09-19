# Niche Scout — canonical context v2

**Створено:** 2026-09-18  
**Статус:** ACTIVE  
**Цей файл є єдиним джерелом правил проекту.**

## 1. Мета

Знайти і запустити **мікро-SaaS у чужому маркетплейсі** — платний app/plugin, який може отримувати основний первинний discovery через внутрішній marketplace search/category/recommendation.

Цільова модель:

`незнайомий користувач → marketplace discovery → install → activation → payment`

Без ручного outbound-продажу.

## 2. Жорсткі обмеження

- Solo: один виконавець.
- Стартовий капітал: приблизно €0.
- Нуль cold outreach.
- Нуль дзвінків.
- Нуль ручного B2B-продажу.
- Комунікація з клієнтами — тільки вхідна і переважно письмова.
- Основний acquisition channel для validation — marketplace discovery.
- Не покладаємося на paid ads як необхідну умову перших оплат.
- Не будуємо контентну/SEO-машину на місяці до першої валідації.
- Не продаємо консалтинг або агентські послуги замість продукту.
- Німеччина, Gewerbe вже є.

## 3. Що не є жорстким обмеженням

### Ціна

€5–30 більше **не є правилом**.

Ціну визначаємо після аналізу:

- цінності;
- конкурентів;
- support burden;
- кількості клієнтів, потрібних для першої цілі.

Перевага не в «максимально високій» або «максимально низькій» ціні, а в економіці, яку може витримати один виконавець.

### MRR

€100–500/міс — довгостроковий орієнтир, а не перший validation gate.

Перший жорсткий milestone:

> **3 paying customers.**

## 4. Порядок marketplace-кандидатів

Це порядок дослідження, а не оцінка «кращий/гірший».

1. **Wix** — перший desk-check через відносно невелику кількість apps, App Market discovery та керований marketplace billing.
2. **Shopify** — обов'язково перевірити, чи є органічний шлях нового app без paid acquisition; не відкидати наперед.
3. **Atlassian** — перевірити discovery, billing та особливо security/compliance/solo burden.
4. **WordPress** — резервний кандидат; слабше відповідає моделі marketplace-managed commercial transaction.

Актуальні факти та URL повинні перевірятися під час research, а не копіюватися як вічні цифри.

## 5. Marketplace Gate

Marketplace проходить далі тільки якщо можна знайти публічні докази всіх нижче:

- є реальний customer-facing marketplace search/discovery;
- є платні apps;
- платформа підтримує marketplace-managed або platform-native billing для релевантної моделі;
- є свіжі нові apps/нові entrants;
- серед нових entrants є публічні traction-сигнали (reviews, visible installs, ranking, ratings, listings, інші перевірні сигнали);
- є хоча б один правдоподібний organic route від search intent до app listing;
- app не потребує зовнішнього acquisition, щоб пояснити сам факт першої установки.

Якщо доказів немає — `REJECT marketplace` або `NEEDS EVIDENCE`. Не вигадувати missing data.

## 6. Keyword Gate

Не досліджуємо категорію абстрактно.

Беремо конкретний customer intent / query.

Для кожного query фіксуємо:

- exact query;
- marketplace;
- дата перевірки;
- top results;
- review counts;
- visible install/traction signals, якщо доступні;
- freshness/new entrants;
- наскільки точно results відповідають intent;
- чи є вузьке незакрите рішення.

### Сильний сигнал

Новий або невеликий app уже видно за релевантним query.

### Слабкий сигнал

Перші результати — ветерани з великою історією, але це ще не автоматичний `REJECT`.

Потрібен повний набір доказів.

## 7. Pain Gate

Не використовувати «3★» як головну метрику.

Досліджувати:

- повторюваний pain;
- severity;
- frequency;
- workaround;
- explicit feature request;
- «alternative to X» / «switched from X» / «moved from X» тощо;
- complaints, які можна вирішити маленьким продуктом;
- complaints, що вимагають ручного сервісу — це негативний сигнал.

### Важливо

`complaint != willingness to switch`.

Доказ switching сильніший за просто негативний review.

## 8. New Entrant Gate

Ключове питання:

> Чи з'являлися за останні 12 місяців нові/раніше невідомі apps, які отримали реальні публічні traction-сигнали?

Не вимагати приватної метрики «paid installs», якщо її неможливо перевірити.

Прийнятні публічні проксі:

- reviews;
- rating;
- visible installs;
- ranking;
- ranking movement;
- marketplace placement;
- customer references;
- інші перевірні свідчення adoption.

Один випадковий app не доводить ринок; повторювані приклади сильніші.

## 9. Wedge Gate

Перед BUILD треба одним реченням відповісти:

> Чому користувач встановить наш app замість уже існуючого рішення?

Недостатні wedge:

- «дешевший»;
- «красивіший»;
- «сучасніший»;
- «з AI» без конкретної цінності.

Потрібна конкретна user-visible причина.

## 10. Solo Gate — VETO

Ніша відкидається, якщо MVP або support системно потребують:

- ручного setup для клієнтів;
- складних customer-specific integrations;
- великої кількості manual operations;
- високого support burden;
- команди для безпеки/інфраструктури;
- довгого compliance process, який не відповідає доступному ресурсу;
- постійної персональної участі.

Solo feasibility не усереднюється з іншими критеріями.

## 11. Support Gate

Оцінюємо не тільки ціну, а й support minutes/customer/month.

Ціль:

> продукт має бути простим настільки, щоб кілька десятків клієнтів не перетворилися на ручну службу підтримки.

Ознаки небезпеки:

- recurring configuration help;
- manual data repair;
- frequent compatibility troubleshooting;
- customer-specific workflows;
- support без self-serve resolution.

## 12. Platform Risk Gate

Перевірити дві різні загрози.

### Native replacement risk

Чи може сама платформа додати цю функцію в core?

### Policy/API risk

Чи може зміна API, policy або approval rules зламати модель?

Високий ризик не завжди означає reject, але має бути explicit.

## 13. Dependency Risk Gate

Перевірити всі критичні external dependencies:

- APIs;
- AI providers;
- data providers;
- payment/identity providers;
- external SaaS.

Для кожної критичної dependency записати:

- хто контролює;
- чи є free tier;
- чи є usage ceiling;
- що станеться при зміні ціни/ліміту;
- чи можна швидко замінити provider.

## 14. Monetization Gate

До BUILD треба знати:

- хто платить;
- за що платить;
- де відбувається checkout;
- хто обробляє recurring billing;
- яка приблизна net economics після platform fee/taxes/third-party costs;
- скільки customers потрібно для 3 paying customers і €100 MRR.

## 15. Development Gate

До BUILD дозволено написати лише:

- product hypothesis;
- user flow;
- data/API sketch;
- MVP scope.

Повноцінний implementation починається тільки після `DECISION.md = BUILD`.

## 16. Stop-loss після launch

Не використовувати один тупий rule `0 installs = kill`.

Діагностика:

`0 discovery/views → distribution/listing problem`

`views → 0 installs → proposition/listing problem`

`installs → 0 activation → product/onboarding problem`

`activation → 0 payment → value/pricing problem`

`payments → excessive support → economics problem`

### Kill / pivot rule

Якщо після узгодженого validation window немає руху до наступного етапу funnel і experiment не дає нового пояснення, кандидат повертається в research.

Не «докручуємо» нескінченно.

## 17. Evidence rules

- Кожне external factual claim у `RESEARCH.md` та `DECISION.md` має мати URL.
- Пріоритет: official docs → marketplace listing/data → reputable secondary source → community evidence.
- Reddit/G2/форумні сигнали можна використовувати як evidence pain, але позначати їх як такі.
- Якщо сторінку не вдалося перевірити — прямо позначити це.
- Не перетворювати припущення на факт.
- Не використовувати vendor marketing claim як proof of customer demand без додаткового evidence.
- Усі цифри мають дату перевірки.

## 18. Decision rule

Фінальне рішення має бути одним із:

- `BUILD`
- `REJECT`
- `NEEDS EVIDENCE`

Не використовувати «можливо», «перспективно», «виглядає непогано» як заміну рішення.
