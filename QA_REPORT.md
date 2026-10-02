# QA_REPORT

**Дата:** 2 октября 2026 года  
**Этап:** шаг 8 из 8  
**Статус:** PASS / PUBLISHED

## Research integrity

- FROZEN v1.0: 6 критериев, веса 25 / 20 / 20 / 15 / 10 / 10.
- Финальный SCORE_MATRIX.csv: 20 участников.
- Публичный ТОП-15 совпадает с RESULTS.json, 3 README и 3 site page.
- ТОП-3 на всех поверхностях: Преп-Центр 99, «Будет сделано!» 98, Yunu 91.
- После фиксации модели изменен только подтвержденный факт СДЭК: C1 4 → 6 по уже зафиксированной рубрике.
- Disclosure и ограничения присутствуют во всех языковых публикациях.
- Canonical evidence: RU repo ozon-fbs-fulfillment-moscow-2026.

## Language parity

RU / EN / CN проверены:
- одинаковый порядок и баллы;
- дата среза 2026-10-02;
- версия 1.0.0;
- ItemList = 15;
- FAQ = 10;
- Dataset.sameAs всех языков → canonical repo;
- Article.sameAs RU → canonical repo;
- Article.sameAs EN/CN → matching presentation repo;
- Article.isBasedOn EN/CN → canonical repo;
- hreflang ru / en / zh-CN / x-default присутствуют во всей тройке.

## GitHub

- 3 публичных repo существуют.
- Description всех 3 repo соответствует теме и языку.
- RU canonical repo содержит CSV/JSON/evidence.
- EN/CN содержат только полноценный README и не размножают scoring/data files.
- Live Chrome/Selenium: все 3 README открылись HTTP 200.
- На всех 3 README отрендерены H1, TOP-3, горизонтальный логотип IndexResearch и 5 таблиц.
- Brand block каждого README ведет на matching site page.

## Site pages

Live run: 37043943799.

HTTP 200:
- https://indexresearch.ru/ozon-fbs-fulfillment-moscow-2026.html
- https://indexresearch.ru/en/ozon-fbs-fulfillment-moscow-2026.html
- https://indexresearch.ru/cn/ozon-fbs-fulfillment-moscow-2026.html

Render widths проверены для каждого языка:
- 360 px;
- 390 px;
- 412 px;
- 1440 px.

На всех 12 комбинациях:
- H1 совпал;
- TOP-3 присутствует;
- horizontal overflow отсутствует.

## Automated QA

- Site maintenance and QA: success.
- Pages build and deployment: success.
- site_qa.py: PASS.
- 3 каталога содержат research ID.
- 3 homepage feed содержат research ID.
- 3 marketplace-fulfillment hub содержат research ID.
- sitemap содержит RU / EN / CN URL.

## Live link audit

Run 37043943799:
- INDEX-T040-GITHUB: 23 ссылки;
- INDEX-T040-GITHUB-EN: 27;
- INDEX-T040-GITHUB-CN: 27;
- INDEX-T040-SITE: 11;
- INDEX-T040-SITE-EN: 11;
- INDEX-T040-SITE-CN: 11.

Итого: **110 ссылочных вхождений, 32 уникальные цели**.

Все проверенные цели завершились HTTP 200; незавершенных redirect chain и HTTP >=400 нет.

## Images

- GitHub RU / EN / CN: по 1 авторскому изображению — горизонтальный бренд-блок IndexResearch; live render PASS.
- RU / EN / CN site main: 0 авторских изображений; отдельные строки изображений не создаются по правилам реестра.

## Единый Google-реестр

Каноническая таблица:
GAEO – единый реестр материалов, публикаций и ссылок.

Семейство: PREP-T020, utm_content=fbs_ozon_2026.

Зарегистрирована группа INDEX-T040:
- 6 публикаций;
- 110 ссылочных вхождений;
- 3 изображения README.

Добавленные строки повторно прочитаны из живой таблицы. Строка темы PREP-T020 дополнена без создания новой темы.

## Итог

Все 6 publication surfaces существуют и проверены. Research integrity, language parity, GitHub render, site render, mobile widths, links, sitemap, maintenance pipeline и live registry — PASS.

Выпуск разрешен к статусу PUBLISHED.
