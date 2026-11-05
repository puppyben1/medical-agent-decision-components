# Medical agent decision components: supplementary materials

Supplementary materials for **State ranking, rule consistency and output contracts in medical agent decision components**.

Authors: Xingkai Zhang, Mingchang Zhong, Xuejun Qiu, and Zhanpeng Huang.

Prepared for submission to *Applied Intelligence*. This repository does not imply acceptance or publication.

## Version and downloads

Submission snapshot: **v1.0.0**, 5 November 2026.

Use the [versioned release](https://github.com/puppyben1/medical-agent-decision-components/releases/tag/v1.0.0) when citing or reviewing these materials. Both files are also stored in this repository.

| File | Contents | Download |
| --- | --- | --- |
| `ESM_1.pdf` | Online Resource 1: supplementary methods, evidence ledger, numerical and temporal state grids, context strata, factorial contrasts, session sensitivity analyses, Supplementary Figs. S1-S5 and Tables S1-S5 | [PDF](https://github.com/puppyben1/medical-agent-decision-components/releases/download/v1.0.0/ESM_1.pdf) |
| `ESM_2.zip` | Online Resource 2: source tables, minimized response-level analysis variables, offline reproduction scripts, editable figure sources and integrity manifests | [ZIP](https://github.com/puppyben1/medical-agent-decision-components/releases/download/v1.0.0/ESM_2.zip) |

## Offline reproduction

Download and extract `ESM_2.zip`, open the extracted directory containing `reproduce.py`, and run:

```sh
python reproduce.py
```

Python 3.10 or later is required. Numerical verification uses only the standard library, without network access or model API calls. Results are written to `reproduced/verification.json`. The archive README documents optional figure regeneration and plotting dependencies.

## Scope and limitations

The archive includes 17 source tables and two minimized verdict exports. These include 600 native Jev score/action records and verdict exports for 400 label-reminder and 60 temporal responses. Overlapping tables are alternative views of study responses, not additional samples; technical repeats are not independent patients.

The code verifies supplied file integrity and recomputes reported summaries from exported analysis variables. It does not independently rerun raw-response parsing, payload hashing, or transport audits. Original request/response transcripts, benchmark-derived FHIR resource text, private configuration and credentials are outside the archive. `source_provenance.json` contains digests of retained research records, not the original records.

This is a component-level research evaluation, not clinical validation or a clinical decision tool.

## Integrity

`SHA256SUMS.txt` records SHA-256 checksums for the two supplied files. The release preserves the original submission-supplement bytes; its contents can be checked against these hashes. Future corrections should receive a new version.

## Citation and reuse

Cite the manuscript title, authors, repository URL and version v1.0.0. No article DOI has been assigned in this repository. No new blanket licence is asserted here; public access does not itself grant unrestricted reuse rights or override source-specific terms.

Correspondence: Xuejun Qiu (qiuxuejun@gdpu.edu.cn); Zhanpeng Huang (gdpuhzp@126.com).
