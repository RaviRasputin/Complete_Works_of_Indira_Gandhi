# Complete Works of Indira Gandhi (work in progress)

A year-wise research collection of speeches and writings of **Indira Gandhi** from her two periods as Prime Minister of India: **24 January 1966 – 24 March 1977** and **14 January 1980 – 31 October 1984**. It follows the layout idea of the [Selected Works of Jawaharlal Nehru](https://github.com/RaviRasputin/Selected_Works_of_JLN) corpus.

> **Not actually complete.** No complete edition of her speeches exists, and the official *Selected Speeches and Writings* (5 vols.) are selections. This repository gathers what is openly obtainable. See [Coverage](#coverage) for gaps. Parliamentary debates (Lok Sabha / Rajya Sabha) are deliberately **not** included; they are held separately.

## Layout

```
years/<YYYY>/        one folder per year (1966-1976, 1980-1984), each with a README index
years/undated/       items whose date is unknown
compilations/        published collections spanning several years (see NOTICE.md; most are not in git)
manifest.csv         one row per file: date, title, venue, language, source URL, sha256, rights status
NOTICE.md            rights and provenance statement
```

Files are named `YYYY-MM-DD_<slug>_<lang>.<ext>`. For each item there may be the original (`.pdf` / `.mp3`) and a Markdown text (`.md`) with YAML metadata.

## Text quality

- Independence Day speeches: **OCR** of scanned PIB PDFs (English and Hindi). Expect errors, especially in Hindi.
- Audio recordings: **automatic transcripts** (Whisper, `medium`); Hindi recordings also have an automatic English translation. Unverified.
- Always cite the original publication or recording, not this repository.

## Coverage

| Source | Content | Years |
|---|---|---|
| PIB | Independence Day addresses, English (no 1976) and Hindi | 1966-75, 1976 (Hi), 1980-84 |
| UN | General Assembly addresses (full plenary records) | 1968, 1983 |
| Internet Archive | Stockholm Conference speech | 1972 |
| All India Radio / HMV via Internet Archive | 8 speeches (audio) | 1969-72 |

**Known gaps:** PIB press releases (1947-2001, no bulk access), Rajya Sabha pre-1984 debates, *Selected Speeches and Writings* vols. 1, 3, 4, 5 (not freely digitised), press conferences, letters, FRUS/FBIS material.

## Scripts

`scripts/` contains the download, OCR, transcription and build scripts. Code is released under the MIT licence; see `NOTICE.md` for the content.

## Rights

See [NOTICE.md](NOTICE.md). This is an unofficial, non-commercial research collection. Rights in the underlying texts and recordings remain with their holders. Contact the maintainer to request removal of any item.
