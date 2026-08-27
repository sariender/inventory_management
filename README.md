# Inventory management

`analytics_retail.ipynb`: reconstructing what actually happened in a stockroom
from transaction records that do not quite add up. Stock going below zero,
receipts with no matching order, duplicate transaction ids.

A rule only means something against a stated model of how the stockroom works, so
the notebook writes those assumptions down before flagging anything.

## Running it

```sh
pip install pandas numpy plotly
jupyter notebook
```

Note: the notebook opens with `import scripts`, a local helper module that is
**not in this repository**, so it will not run end to end as cloned. The analysis
and the output are still readable in the committed cells.

Write-up: <https://endersari.com/projects/data-anomalies/>
