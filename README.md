<div id="header" align="center">
  <img src="https://media.giphy.com/media/QDjpIL6oNCVZ4qzGs7/giphy.gif" width="400"/>

  <h1>
    Привет, я Артём
    <img src="https://media.giphy.com/media/w1OBpBd7kJqHrJnJ13/giphy.gif" width="30px"/>
  </h1>

  <img src="https://komarev.com/ghpvc/?username=udkx&style=flat-square&color=blue" alt="Profile views"/>
</div>

<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&color=7A95C9&center=true&vCenter=true&width=435&lines=Backend+Developer;Go+%C2%B7+PostgreSQL+%C2%B7+Kubernetes;%D0%9A%D0%BE%D0%B4%2C+%D1%82%D0%B5%D1%81%D1%82%D1%8B%2C+%D0%BA%D0%BE%D0%BD%D1%82%D0%B5%D0%B9%D0%BD%D0%B5%D1%80%D1%8B%2C+%D0%B4%D0%B5%D0%BF%D0%BB%D0%BE%D0%B9" alt="Typing SVG" />
</div>

---

Backend-разработчик. Go и Python, PostgreSQL, Kubernetes, CI/CD.
Пишу сервисы полного цикла: код, тесты, контейнеры, деплой.

<div>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/go/go-original-wordmark.svg" title="Go" alt="Go" width="40" height="40"/>&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" title="Python" alt="Python" width="40" height="40"/>&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postgresql/postgresql-original-wordmark.svg" title="PostgreSQL" alt="PostgreSQL" width="40" height="40"/>&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/redis/redis-original-wordmark.svg" title="Redis" alt="Redis" width="40" height="40"/>&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original-wordmark.svg" title="Docker" alt="Docker" width="40" height="40"/>&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/kubernetes/kubernetes-plain-wordmark.svg" title="Kubernetes" alt="Kubernetes" width="40" height="40"/>&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nginx/nginx-original.svg" title="Nginx" alt="Nginx" width="40" height="40"/>&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/rust/rust-original.svg" title="Rust" alt="Rust" width="40" height="40"/>&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original-wordmark.svg" title="React" alt="React" width="40" height="40"/>&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original-wordmark.svg" title="Git" alt="Git" width="40" height="40"/>
</div>

---

### Проекты

<div align="center">
  <img src="assets/100verst-stats.svg" alt="100 вёрст в цифрах: 64 тыс. строк Go, 694 теста, пропускная способность ×7, p50 2,9 мс, 98 эндпоинтов, 34 миграции, 27 тыс. строк TypeScript, 208 тестов фронтенда"/>
</div>

**100 вёрст** — B2B-платформа грузоперевозок, переписана с легаси PHP + MySQL на Go + PostgreSQL + React. Репозитории закрыты (коммерческий проект).

- Бэкенд на Go: модульный монолит, ~64 тыс. строк (треть из них — тесты: 694 теста), 98 эндпоинтов по OpenAPI-контракту, 34 миграции. Только chi, pgx и goose, остальное — стандартная библиотека.
- Деньги: неизменяемый леджер в копейках, холды, идемпотентность по ключу; гонки при зачислениях и возвратах покрыты тестами.
- Персональные данные шифруются на уровне приложения (AES-256-GCM + blind index для поиска), пароли — Argon2id, 2FA для администраторов.
- Собственный инструмент нагрузочного тестирования со сценариями с состоянием. Он нашёл Seq Scan в списке заявок; после индекса под порядок сортировки — 6 600 req/s вместо 950, p50 2,9 мс вместо 20 мс на 18 тыс. записей.
- Фронтенд: React + TypeScript, ~27 тыс. строк, типы API генерируются из OpenAPI, 208 тестов (Vitest, Playwright).

**[stalcraft-api-go](https://github.com/udkx/stalcraft-api-go)** — Go-клиент для STALCRAFT API: типизированные сервисы для всех эндпоинтов, три схемы авторизации с автообновлением OAuth-токена, клиент базы предметов. Без зависимостей вне стандартной библиотеки, 54 теста на `httptest`, CI с `-race` и golangci-lint.

**[minesweeper-ai](https://github.com/udkx/minesweeper-ai)** — сапёр и нейросеть с нуля на Python + PyTorch: движок, точный вероятностный решатель (перечисление конфигураций, сверка с полным перебором до 1e-9) и полносвёрточная сеть на 65 тыс. параметров. Сеть выигрывает 71,6 % партий на среднем уровне против 87,5 % у решателя, но впятеро быстрее, и выдаёт откалиброванные вероятности, хотя училась на жёстких метках. 25 тестов, CI.

**Проект Чернобыль** — открытый документальный архив о ликвидаторах аварии на ЧАЭС. Принцип: нет источника — нет утверждения. Next.js + Payload CMS, PostgreSQL. Репозиторий пока закрыт.

- Факт, событие хронологии или миф без ссылки на реестр источников не сохранится: это проверяет схема данных, а не интерфейс.
- Вики-режим с рецензированием: очередь предложенных правок, публикация только после одобрения, любая правка — новая неизменяемая версия, откат — тоже версия. Журнал аудита.
- Уровни доверия считаются из счётчиков одобренных, отклонённых и откатанных правок; «мелкая правка» определяется механически по изменённым полям.
- Архив источников: копия каждого из 68 документов с SHA-256 и снимком в Wayback Machine. 18 персональных страниц, схема меняется только миграциями, сквозной smoke-тест цикла «правка → одобрение → версия → откат».

**Архив особого хранения, фонд № 04** — интерактивная проза в форме найденного делопроизводства: вымышленное ведомство, опись дел, грифы, изъятые строки, кассетные расшифровки. Next.js 16, React 19, Drizzle + libSQL, Three.js. Репозиторий пока закрыт.

- Сюжет рассказывается формой документа: своя разметка (`[ИЗЪЯТО]`, `[ВОССТАНОВИТЬ]`, ссылки между делами), восстановление фрагментов сопоставлением с копией из другого дела, обратные ссылки вычисляются при чтении.
- Кабинет редактора: раздельные рабочий и опубликованный экземпляры дела, версия записи защищает от перезаписи из устаревшей вкладки (409 с сохранением текста), HMAC-подписанная сессия, проверка Origin на сервере.
- Приложения отдаются с поддержкой HTTP Range; файлы черновиков видит только редактор.
- Главный персонаж — процедурная 3D-модель на React Three Fiber: геометрия и текстуры генерируются кодом, без готовых ассетов.

**[sandustry-native](https://github.com/udkx/sandustry-native)** — нативное ядро симуляции на Rust, тик 9,9 мс против 21 мс в оригинале.

---

### Открытые проекты в цифрах

<div align="center">
  <img src="assets/open-source-stats.svg" alt="Открытые проекты в цифрах: нейросеть выигрывает 71,6 % партий в сапёр, тик симуляции 9,9 мс против 21 мс, Go SDK без внешних зависимостей"/>
</div>

---

**Контакты** — Telegram [@udkx](https://t.me/udkx) · udkx@outlook.com
