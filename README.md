# School Table

**Русский** · [English](README.en.md)

[![CI](https://github.com/EDeev/school_table/actions/workflows/ci.yml/badge.svg)](https://github.com/EDeev/school_table/actions/workflows/ci.yml)
[![Release](https://img.shields.io/github/v/release/EDeev/school_table)](https://github.com/EDeev/school_table/releases)

Десктопный дневник школьника на PyQt5: расписание на неделю и заметки с датами, которые сами
появляются под нужным днём.

**Статус:** учебный проект (Яндекс Лицей, 2021), завершён

![Вкладка «Расписание»](docs/screenshots/timetable.png)

**Стек:** Python 3 · PyQt5 · SQLite

## Возможности

- Сетка на шесть учебных дней, до восьми уроков в день
- Список предметов: добавить, переименовать, удалить (предмет пропадает и из расписания), очистить урок
- Подсветка выбранного предмета во всей неделе
- Заметки с датой и временем: под расписанием показываются по дню недели, на вкладке «Заметки» —
  общим списком за всё время, ближайший месяц или неделю
- Правка заметки и отметка «сделано» (выполненная заметка удаляется)
- Всё хранится локально в `table.db`

## Запуск

Готовая сборка для Windows — в [релизах](https://github.com/EDeev/school_table/releases): `SchoolTable.exe` — просто
запустите (при первом запуске рядом появятся пустая база `table.db` и иконка), или `SchoolTable-windows.zip` — то же
с базой и иконкой в архиве.

Из исходников:

```bash
git clone https://github.com/EDeev/school_table.git && cd school_table
pip install -r requirements.txt
python main.py
```

## Как выглядит

![Вкладка «Заметки»](docs/screenshots/notes.png)

## Структура

```
main.py     приложение: интерфейс (сгенерирован из rasp.ui) и вся логика
rasp.ui     макет окна для Qt Designer
table.db    пустая база: предметы, расписание по дням, заметки
image.ico   иконка
```

## Лицензия

Учебный проект (Яндекс Лицей, 2021). Код открыт для изучения, отдельной лицензии нет.

## Автор

**Деев Егор Викторович** — [GitHub](https://github.com/EDeev) · [Telegram](https://t.me/DeevEgor) · [egor@deev.space](mailto:egor@deev.space)

---

<div align="center">
  <sub>⭐ Если проект оказался полезным, поставьте звёздочку на GitHub!</sub>
  <p><sub>Сделано с ❤️ — <a href="https://deev.space">deev.space</a></sub></p>
</div>
