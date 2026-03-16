# SONA8 NER Config (spaCy)

```ini
[components.sona8_ner]
factory = "ner"
positive_label_weight = 1.2
negative_label_weight = 0.8
labels = ["ORG", "PERSON", "PRODUCT", "FEATURE", "METRIC"]
```

Training TODO:
1. Generate silver data from recent product calls
2. Fine-tune `en_core_web_trf` on ~4k annotated sentences
3. Add rule-based matcher for KPI phrases
4. Export as package for downstream analytics