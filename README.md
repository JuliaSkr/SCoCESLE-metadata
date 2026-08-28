# SCoCESLE Corpus — Metadata

Metadata for the **SCoCESLE** learner corpus: a collection of learner essays annotated with learner background and proficiency.

## Overview

This repository holds the **metadata spreadsheet** describing 307 learner essays, including essay prompts, learner L1, CEFR proficiency level, and demographics. It accompanies work on a "problem of computational linguistics" act (акт проблемы комплинг).

## Repository contents

| File | Description |
|---|---|
| `SCoCESLE-metadata-spreadsheet.csv` | 307 rows × 11 columns of essay metadata. |
| `SCoCESLE_metadata_spreadsheet.xls` | The same spreadsheet in legacy Excel format. |

### Schema

| Column | Meaning |
|---|---|
| `Essay ID` | Unique essay identifier (e.g. `01b.txt`) |
| `Total number of word types` | Type count |
| `Total number of word tokens` | Token count |
| `Essay type/topic` | Essay sub-type/prompt letter |
| `Essay question` | Full prompt text |
| `Course` | Course the essay was written for (e.g. `IELTS Preparation`) |
| `L1` | Learner's first language (e.g. `Colombian Spanish`) |
| `CEFR level as per course being studied` | Proficiency (e.g. `B2`) |
| `Gender` | Learner gender |
| `Year of birth` | Learner birth year |

## Quick start

```python
import pandas as pd
df = pd.read_csv("SCoCESLE-metadata-spreadsheet.csv")
print(df[["Essay ID", "L1", "CEFR level as per course being studied"]].head())
```

## License

Research use. The corpus metadata is provided for academic purposes; please contact the author before redistribution.
