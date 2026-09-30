# HSK 1-3 Datasource (v1)

Files:
- hsk1.json, hsk2.json, hsk3.json: vocabulary from the supplied XLSX, enriched where an exact/variant Hanzi match exists in the supplied BCT A PDF.
- hsk123_enriched.json: merged HSK 1-3 list.
- hsk123_missing_meanings.json: entries that still need a meaning/pinyin source.
- bct_a.json: parsed BCT A entries from the supplied PDF.

Schema per HSK entry:
{
  "id": "hsk1-0001",
  "simplified": "...",
  "traditional": "...",
  "pinyin": "... or null",
  "meaning": "... or null",
  "level": "HSK 1|HSK 2|HSK 3",
  "source": "... or null",
  "meaning_status": "from_bct|missing"
}

Important: BCT English meanings are preserved as supplied; they are not silently corrected. This is intentionally a first-pass merge so questionable meanings can be reviewed separately.
