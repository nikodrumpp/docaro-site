# Задача для иллюстратора — Docaro Landing Page

## Контекст

**Продукт:** Docaro — цифровая сервисная книжка с AI-сканированием чеков  
**Сайт:** docaro.botneversleeps.com  
**Репозиторий сайта:** github.com/nikodrumpp/docaro-site  

---

## Visual Language — обязательно изучить перед началом

В репозитории уже есть 5 готовых SVG иллюстраций. Все новые иллюстрации **обязаны** выдержать тот же стиль.

**Готовые файлы для референса:**
```
assets/icons/auth_hero_dark.svg
assets/icons/ai_scan_dark.svg
assets/icons/smart_reminders_dark.svg
assets/icons/unlimited_records_dark.svg
assets/icons/pdf_export_dark.svg
```

**Ключевые параметры стиля:**

| Параметр | Значение |
|---|---|
| Фон | `#0D0D10` / `#111827` radialGradient, `rx="72"` |
| Акцент синий | `#4B9EFF` / `#0A84FF` |
| Акцент зелёный | `#34D399` |
| Акцент фиолетовый | `#A78BFA` |
| Акцент жёлтый | `#F59E0B` |
| Карточки | `fill="#17171D"`, border `stroke-opacity` 0.42–0.62 |
| Текст в карточках | `#F5F5F7` (primary), `#8E8E93` (secondary) |
| Glow-фильтры | feGaussianBlur stdDeviation 3–5, feMerge |
| viewBox | `0 0 400 400` |
| Формат | `.svg`, тёмная тема |
| Corners background rect | `rx="72"` |

**Обязательные элементы в каждой иллюстрации:**
- Ambient ellipse (очень тонкий glow по центру, opacity 0.03–0.05)
- Neural nodes (3–6 точек с соединительными линиями, opacity 0.09–0.17) в углах
- Subtle grid lines (stroke-opacity 0.022)

---

## Что нужно создать

### Группа A — Иконки Problem секции (3 шт)

Маленькие иконки, `52×52px` отображение внутри карточки на тёмном фоне `#14141F`.  
Фактический SVG `viewBox="0 0 80 80"` — простые, лаконичные, моноцветные с одним акцентным цветом.

---

**`problem_receipt_dark.svg`**
- Что изображает: мятый / скомканный бумажный чек
- Смысл: receipts pile up and disappear
- Акцент: `#F59E0B` (amber — тревога, потеря)
- Детали: чек слегка смят, загнут угол, несколько строк текста-плашек, возможно тень
- Путь: `assets/icons/problem_receipt_dark.svg`

---

**`problem_calendar_dark.svg`**
- Что изображает: календарь с красным крестом или пропущенной датой
- Смысл: missed service date
- Акцент: `#EF4444` (red — ошибка, пропуск)
- Детали: календарная сетка, одна ячейка выделена крестом или красным кружком
- Путь: `assets/icons/problem_calendar_dark.svg`

---

**`problem_question_dark.svg`**
- Что изображает: знак вопроса над силуэтом автомобиля
- Смысл: can’t prove service history when selling
- Акцент: `#8E8E93` (grey — неопределённость, незнание)
- Детали: упрощённый силуэт машины снизу, большой `?` сверху
- Путь: `assets/icons/problem_question_dark.svg`

---

### Группа B — Feature карточки (2 шт)

Иллюстрации для feature-карточек. Размер отображения `100% width`, `aspect-ratio: 4/3`.  
Стиль: сцена, как в `smart_reminders_dark.svg` и `ai_scan_dark.svg` — с data-карточками, glow, particles.  
`viewBox="0 0 400 300"`

---

**`feature_history_dark.svg`**
- Что изображает: список сервисных записей / лог обслуживания
- Смысл: Full Service History — all records in one place
- Акцент: `#4B9EFF` (blue)
- Детали: несколько вертикально расположенных карточек-записей с иконками категорий (масло, шины, тормоза), датами, суммами. Последняя запись — самая яркая (newest)
- Путь: `assets/icons/feature_history_dark.svg`

---

**`feature_multicar_dark.svg`**
- Что изображает: несколько транспортных средств (авто + мотоцикл, или 2 авто)
- Смысл: Multiple Vehicles — car, motorcycle, truck, boat in one account
- Акцент: `#34D399` (green) + `#4B9EFF` (blue) для двух объектов
- Детали: два силуэта транспорта, у каждого своя бейдж-карточка с именем/типом, объединены общим интерфейсом
- Путь: `assets/icons/feature_multicar_dark.svg`

---

### Группа C — Why Docaro карточки (2 шт)

Маленькие иконки `56×56px` отображение. `viewBox="0 0 80 80"`.  
Стиль проще, чем A: чёткий смысловой символ без лишней детализации.

---

**`why_transfer_dark.svg`**
- Что изображает: две фигуры людей, между ними стрелка передачи
- Смысл: History Transfer — sell your car, pass the history
- Акцент: `#4B9EFF` (blue)
- Детали: упрощённые силуэты двух людей (левый — продавец, правый — покупатель), между ними горизонтальная стрелка вправо, возможно маленький файл/документ на стрелке
- Путь: `assets/icons/why_transfer_dark.svg`

---

**`why_privacy_dark.svg`**
- Что изображает: щит с замком
- Смысл: Your data stays yours — no third-party access
- Акцент: `#34D399` (green — безопасность, доверие)
- Детали: щит, внутри замок, возможно тонкое свечение вокруг
- Путь: `assets/icons/why_privacy_dark.svg`

---

### Группа D — Крупный визуал (1 шт)

**`final_cta_dark.svg`**
- Что изображает: силуэт автомобиля или телефон с открытым приложением
- Смысл: финальный призыв — эмоциональная точка страницы
- Размер отображения: `440×140px` (широкий горизонтальный баннер)
- `viewBox="0 0 880 280"` (или пропорционально)
- Акцент: `#4B9EFF` + `#34D399`, premium feel
- Детали: силуэт машины с подсветкой снизу (ground glow) и парой data-карточек рядом, или лаконичная горизонтальная композиция — телефон + луч/scan-линия
- Путь: `assets/icons/final_cta_dark.svg`

---

## Куда класть файлы

Все файлы — в одну папку:
```
github.com/nikodrumpp/docaro-site / assets/icons /
```

Именование строгое: только латиница, snake_case, суффикс `_dark.svg`.

---

## Как файлы подключены в HTML

После добавления файлов — разработчик (или этот агент) обновит `index.html`, заменив плейсхолдеры на:
```html
<img src="assets/icons/[filename].svg" alt="..." loading="lazy"/>
```

Дополнительных действий от иллюстратора не требуется — только положить файлы в папку.

---

## Приоритет выполнения

1. **Группа C** (why_transfer, why_privacy) — маленькие, быстро
2. **Группа A** (problem ×3) — маленькие иконки
3. **Группа B** (feature_history, feature_multicar) — сложнее, требуют сцены
4. **Группа D** (final_cta) — финальный крупный визуал

---

## Summary — итого нужно создать

| Файл | Группа | Размер отображения | Сложность |
|---|---|---|---|
| `problem_receipt_dark.svg` | A | 52×52 | ●○○ |
| `problem_calendar_dark.svg` | A | 52×52 | ●○○ |
| `problem_question_dark.svg` | A | 52×52 | ●○○ |
| `feature_history_dark.svg` | B | 400×300 | ●●● |
| `feature_multicar_dark.svg` | B | 400×300 | ●●○ |
| `why_transfer_dark.svg` | C | 56×56 | ●○○ |
| `why_privacy_dark.svg` | C | 56×56 | ●○○ |
| `final_cta_dark.svg` | D | 880×280 | ●●● |

**Итого: 8 файлов**
