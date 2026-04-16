# Roadmap index

Этот файл — вспомогательный индекс структуры roadmap после расширения ТЗ.

## Ключевые дополнения по сравнению с базовой версией
- введены дополнительные внутренние статусы: `WARMING_UP`, `WATCHLIST`, `PREVIEW`, `DEGRADED`, `BLOCKED_*`;
- tradeable `ENTER_*` для BTC v1 разрешён только на закрытии `1m` свечи;
- добавлен слой нормализации сигналов и threshold profiles;
- setup family расширена: trap / failed continuation / absorption split;
- добавлены replay/validation storage и rule versioning;
- добавлены substeps для long/short geometry.

## Новые файлы
- `3.8.md`
- `3.9.md`
- `7.9.md`
- `8.5.1.md`
- `8.6.1.md`
- `8.6.2.md`

## Обязательный порядок чтения
1. `0.md`
2. базовые этапы по порядку
3. новые дополнительные substeps там, где они появляются в дереве этапов


---

## Редакция v3: новые обязательные уточнения

В текущей редакции roadmap дополнительно закреплены:
- tradeable `ENTER_*` только на закрытии 1m;
- fixed bootstrap windows для candles / OI / funding;
- точные формулы CVD, OI acceleration, liquidation imbalance и book imbalance;
- HTF контекст = `1h + 4h` для decision v1;
- explicit setup families для trap / failed continuation / absorption;
- stale budgets;
- dedupe policy;
- carry-forward policy для minute OI;
- rule versioning и threshold profiles;
- replay / validation storage;
- no-ML rule для v1;
- read-only UX для первой версии.


## Новые файлы финальной редакции
- `6.10.md`
- `7.10.md`
- `11.7.md`

## Финальные полезные уточнения
- reconnect/backoff policy зафиксирована отдельно;
- data anomaly filter и dedupe вынесены в отдельный подэтап;
- latency SLA и quality lag отражаются в health/degraded state;
- long/short ratio добавлен как soft feature;
- benchmark baseline добавлен как отдельный validation layer.
