# nogps-maps

Офлайн-пакеты областей Украины для навигатора nogps (навигация без доверия к GPS).

Каждая область в релизе — три файла:

| файл | что внутри |
|---|---|
| `UA-xx-graph.nogpsgraph` | граф дорог для автомобиля (односторонние улицы, ограничения скорости, запреты поворотов) |
| `UA-xx-addresses.tsv.gz` | адреса: улица, дом, координаты, населённый пункт |
| `UA-xx-map.pmtiles` | векторная карта (PMTiles) |

`regions.json` — список областей с размерами и контрольными суммами (sha256).
Приложение скачивает его по адресу `https://github.com/kkav1k/nogps-maps/releases/latest/download/regions.json`.

## Источники и лицензии

- Дороги, адреса, границы областей: © участники [OpenStreetMap](https://www.openstreetmap.org/copyright),
  лицензия [ODbL 1.0](https://opendatacommons.org/licenses/odbl/). Выгрузка: [Geofabrik](https://download.geofabrik.de/europe/ukraine.html).
- Векторная карта: [Protomaps](https://protomaps.com) basemap, построена из данных OpenStreetMap (ODbL).

Пакеты производные от OpenStreetMap и распространяются на тех же условиях (ODbL).
