# Spotify Clone

Пет-проект с кастомным аудио-движоком на Web Audio API, FSD-архитектурой, production-ready стеком.

## Архитектура

FSD (Feature-Sliced Design):

- `app` — инициализация, роутинг, провайдеры
- `pages` — страницы приложения (Home, Playlist, Artist, Album)
- `widgets` — самостоятельные блоки (PlayerBar, Sidebar, TrackList)
- `features` — пользовательские сценарии (playTrack, addToQueue, toggleLike)
- `entities` — бизнес-сущности (Track, Playlist, Artist, User)
- `shared` — переиспользуемый код (UI-kit, API, utils, hooks)

## Стек

| Технология                     | Назначение               |
| ------------------------------ | ------------------------ |
| React 19 + TypeScript (strict) | UI + типобезопасность    |
| Vite + SWC                     | Сборка, мгновенный HMR   |
| Zustand                        | State management         |
| TanStack Query v5              | Data fetching, caching   |
| Web Audio API                  | Кастомный аудио-движок   |
| Tailwind CSS                   | Стилизация               |
| Vitest + Testing Library       | Unit-тесты               |
| Playwright                     | E2E-тесты                |
| Storybook                      | Документация компонентов |
| MSW                            | Mock API                 |

## Установка

```bash
git clone &lt;repo-url&gt;
cd spotify-clone
npm install
```
