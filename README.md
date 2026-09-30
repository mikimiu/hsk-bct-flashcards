# HSK Vocabulary Flashcards

Mobile-first PWA for daily review of the vocabulary from the uploaded HSK XLSX and BCT(A) PDF.

## Included
- HSK 1, HSK 2, HSK 3 sections from the uploaded XLSX.
- Simplified / Traditional / Both display filter for HSK.
- BCT A section from the uploaded PDF, with exact Hanzi duplicates removed when the same Hanzi exists in HSK 1–3.
- Local progress in `localStorage`.
- Due / unseen / mastered / missed filters.
- Basic spaced review intervals.
- PWA files so it can be installed from Chrome after deployment.

## Data note
The uploaded XLSX contains Simplified and Traditional columns but does not contain pinyin or English meanings. The app therefore enriches HSK cards on first load from the public `jelleverheyen/hsk-vocabulary` dictionary dataset. After loading, the enriched data is cached in the browser.

The BCT PDF itself supplies pinyin, Chinese, and English; those values are included locally.

## Deploy to GitHub Pages
1. Create a GitHub repository.
2. Upload everything in this folder.
3. In the repository: Settings → Pages → Deploy from branch → `main` / root.
4. Open the resulting Pages URL in Chrome on your phone.
5. Chrome can then offer **Add to Home screen / Install app**.

You can also deploy the folder to any static hosting provider.

## Sources
- User-provided HSK XLSX: vocabulary/character lists.
- User-provided BCT(A) PDF: 600 numbered BCT(A) entries.
- HSK enrichment dataset: https://github.com/jelleverheyen/hsk-vocabulary
