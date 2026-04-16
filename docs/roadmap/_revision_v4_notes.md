# Revision v4 notes

## Что добавлено в этой редакции
- Зафиксирован точный scope данных для BTC v1: `BTCUSDT` linear perpetual + `BTCUSDT` spot confirm layer.
- Зафиксированы bootstrap windows для candles, OI и funding.
- Зафиксирован двухслойный decision timing: realtime preview + tradeable enter только на закрытии `1m`.
- Добавлены точные формулы для:
  - quote-notional CVD
  - OI delta / acceleration
  - liquidation imbalance / burst
  - book imbalance
- Зафиксированы stale budgets и dedupe policy.
- Зафиксированы carry-forward правила для minute OI.
- Расширены setup families: trap / failed continuation / absorption.
- Зафиксированы RR floors и trade geometry rules.
- Добавлены replay/validation/outcome tracking requirements.
- Зафиксировано отсутствие ML/retraining в v1.
- Зафиксирован read-only UX для первой версии.

## Для чего нужен этот файл
Этот файл нужен как краткая карта отличий редакции v4 от предыдущей версии архива.
Рабочими документами остаются `0.md` и соответствующие `x.y.md`.


## Финальные уточнения сверх редакции v4
- Добавлена отдельная политика anomaly filtering / dedupe / latency tracking.
- Добавлена explicit reconnect/backoff policy для WS manager.
- Добавлен optional long/short ratio как soft sentiment feature.
- Добавлен benchmark baseline для validation-comparison.
- Зафиксировано, что эти дополнения усиливают v1, но не раздувают scope до внешних бирж, ML, K8s и прочего future backlog.
