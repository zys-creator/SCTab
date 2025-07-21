# SCTab: A Benchmark Test Set for Table Structure Recognition

**SCTab** is a large-scale test dataset designed for evaluating table structure recognition (TSR) models, especially in complex scenarios involving spanning cells, irregular layouts, and real-world scanned documents.

## 📦 Dataset Overview

- **Total samples**: 10,000
- **File format**: JSON Lines (`.jsonl`)
- **Image format**: PNG
- **Use case**: Evaluation of table parsing / structure recognition models

Each entry corresponds to one table image with detailed structural annotations.

### ✅ JSONL Format Example

Each line in the `.jsonl` file contains:

```json
{
  "name": "000_00000151.png",
  "text": ["Abstract", "TOTAL", "con-", "of", "sale", "paid", "in", "Analyses", ...],
  "box": [[17, 25, 76, 44], [99, 11, 143, 30], ...],
  "html": ["<table>", "<tr>", "<td rowspan=\"2\">", "</td>", ...]
}
