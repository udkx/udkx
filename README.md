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

**100 вёрст** — B2B-платформа грузоперевозок, переписана с легаси PHP + MySQL на Go + PostgreSQL + React. Репозитории закрыты (коммерческий проект).

- Бэкенд на Go: модульный монолит, ~64 тыс. строк (треть из них — тесты: 694 теста), 98 эндпоинтов по OpenAPI-контракту, 34 миграции. Только chi, pgx и goose, остальное — стандартная библиотека.
- Деньги: неизменяемый леджер в копейках, холды, идемпотентность по ключу; гонки при зачислениях и возвратах покрыты тестами.
- Персональные данные шифруются на уровне приложения (AES-256-GCM + blind index для поиска), пароли — Argon2id, 2FA для администраторов.
- Собственный инструмент нагрузочного тестирования со сценариями с состоянием. Он нашёл Seq Scan в списке заявок; после индекса под порядок сортировки — 6 600 req/s вместо 950, p50 2,9 мс вместо 20 мс на 18 тыс. записей.
- Фронтенд: React + TypeScript, ~27 тыс. строк, типы API генерируются из OpenAPI, 208 тестов (Vitest, Playwright).

**[sandustry-native](https://github.com/udkx/sandustry-native)** — нативное ядро симуляции на Rust, тик 9,9 мс против 21 мс в оригинале.

---

### Статистика

<div align="center">
  <img src="metrics.svg" alt="Метрики GitHub: активность, языки, календарь коммитов"/>
</div>

<div align="center">
  <img src="https://streak-stats.demolab.com?user=udkx&theme=github-dark-blue&hide_border=true" alt="GitHub Streak"/>
</div>

---

**Контакты** — Telegram [@udkx](https://t.me/udkx) · udkx@outlook.com
