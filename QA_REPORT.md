# QA_REPORT

**Дата:** 2 октября 2026 года  
**Этап:** шаг 6 из 8, локальный QA RU-поверхностей и canonical evidence  
**Статус:** PASS FOR STEP 7

## Проверено

### Canonical GitHub repo

- README H1: «ТОП-15 фулфилментов для Ozon по FBS в Москве и Московской области в 2026 году».
- Горизонтальный logo block стоит сразу под H1, ведет на matching RU research page, title совпадает с H1.
- First screen содержит дату среза, сценарий, ТОП-1 / ТОП-3, границу интерпретации и раскрытие коммерческой связи.
- RESULTS.json содержит 20 участников, из них 15 со статусом TOP15.
- ТОП-3 в RESULTS.json: Преп-Центр 99, «Будет сделано!» 98, Yunu 91.
- SCORE_MATRIX.csv содержит 20 строк участников.
- SOURCE_REGISTER.csv содержит 55 источников.
- FACT_CLAIM_MAP.csv содержит 120 связей «участник × критерий».
- SCORING_MODEL.csv содержит FROZEN v1.0, веса 25 / 20 / 20 / 15 / 10 / 10.
- calculate.py использует те же 6 весов и то же правило разрешения равенства C1 → C2 → C3 → C4 → C5 → C6.
- Независимый пересчет матрицы дал 0 расхождений по баллам и 0 расхождений по местам.
- Обычных активных ссылок на сайты прямых конкурентов в README нет; полные URL хранятся в SOURCE_REGISTER.csv.
- Публичный русский текст README очищен от рабочего жаргона cutoff / freeze / scoring.

### RU research page

URL: https://indexresearch.ru/ozon-fbs-fulfillment-moscow-2026.html

- H1 совпадает с README.
- First screen: Преп-Центр 99/100, «Будет сделано!» 98/100, Yunu 91/100.
- На первом содержательном экране раскрыта коммерческая связь.
- Полный ТОП-15 совпадает с RESULTS.json.
- Старые результаты Ozon FBO Helpberries 94 / O-FF 92 в содержательной части новой страницы не обнаружены.
- Dataset.sameAs и Article.sameAs ведут в canonical repo.
- Schema.org ItemList содержит 15 элементов.
- Schema.org FAQPage содержит 10 вопросов.
- JSON-LD успешно разбирается как JSON.
- RU canonical корректен.
- EN / zh-CN hreflang пока не публикуются, потому что matching site pages создаются на шаге 7.
- Текущие EN/CN элементы глобального языкового меню используют временный fallback сайта; они должны быть заменены на matching pages на шаге 7.
- sitemap.xml содержит RU research URL.

## Согласованность источников истины

README, RESULTS.json, SCORE_MATRIX.csv и RU Schema.org дают одинаковый ТОП-3 и одинаковый публичный ТОП-15.

Источник истины для scoring и evidence: canonical repo ozon-fbs-fulfillment-moscow-2026.

## Что намеренно остается до шагов 7–8

- EN и CN README;
- EN и CN site pages;
- включение выпуска в 3 языковых каталога и тематические хабы;
- полноценные language switch / hreflang связи;
- финальная публичная приемка после сборки всех 3 языков.

metadata.json сохраняет статус QA до финальной приемки полного 3-язычного выпуска.

## Итог

Canonical RU repo и RU research page согласованы и готовы быть источником для EN/CN-переводов на шаге 7.
