# DUST PROTOCOL — HVH Edition

Браузерный 2D top-down HvH-шутер по мотивам CS:GO / de_dust2. Один файл — `index.html`, чистый HTML5/CSS/JS (Canvas API, без внешних зависимостей). Открывается двойным кликом в любом современном браузере.

## HVH: боты тоже читеры
В HVH-режиме (включён по умолчанию) боты играют с полным набором читов, как и вы:
- **Wallhack** — всегда знают, где вы, и давят через всю карту
- **Snap-aimbot + hit chance** — мгновенный доворот с настраиваемой точностью по тирам
- **Anti-aim / desync** — модель бота стоит боком к своей реальной позиции (фейк-хитбокс)
- **Spinbot** — видимая модель бешено крутится
- **Resolver** — на каждую очередь решают, вскрыть ли вашу анти-аим
- **Double tap** — элитные боты досылают второй патрон

Побеждает тот, чей resolver и anti-aim работают лучше.

## Чит-меню (Insert) — в стиле gamesense/skeet
Тёмное перетаскиваемое окно с радужной полосой, вертикальными вкладками и групбоксами:
- **RAGE** — Aimbot (silent, FOV, hit chance, min damage, autofire, target selection), Auto wall (пробитие стен), Resolver, Double tap
- **ANTI-AIM** — yaw (backward/jitter/spin), spin speed, desync amount; фейковая модель рисуется пунктиром
- **LEGIT** — плавный aimbot (FOV/smooth), RCS, триггербот с задержкой реакции
- **VISUALS** — ESP (corner/full box, name, HP, weapon, distance, glow, resolved-хитбокс), radar hack, sound ESP, offscreen arrows, weapon drops
- **MISC** — watermark, keybind list, event log, hitmarker/hit sound/kill sound, настройка прицела
- **SKINS** — цвет/паттерн модели игрока и оружия
- **CONFIG** — 3 слота пресетов (alpha/beta/gamma) + reset; всё автосохраняется в localStorage

## Карта — de_dust2
Узнаваемая планировка: B-site, CT spawn, A-site с дефолт-плитой, mid + mid doors, catwalk/short, long A с дверями и pit, туннели с изгибом, T-spawn. Подписи зон на полу как на радаре. A* навигация ботов по тайловой сетке.

## Остальное
- 8 видов оружия + 3 гранаты, экономика и меню закупки (клавиши 1–5)
- Раундовая структура: закупка → бой → итоги → рост сложности; 3 жизни
- Пробитие стен (auto wall) со штрафом урона по прочности поверхности
- Синтезированный звук (Web Audio API), частицы, hitmarker, kill/hit sounds
- Стабильные 60 FPS, фиксированный шаг симуляции

## Управление
WASD — движение · мышь — прицел · ЛКМ — огонь · ПКМ — прицеливание · Shift — тихий шаг · Ctrl — присед · R — перезарядка · 1–4 — слоты · G — смена гранаты · E — подобрать оружие · B — закупка · **Insert — чит-меню**
