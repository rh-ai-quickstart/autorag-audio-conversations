# Customer billing recording

This dataset contains one English customer-billing call:

| Recording | Reference text | Benchmark questions |
| --- | --- | ---: |
| `documents/en-support-billing.mp3` | `reference/en-support-billing.txt` | 10 |

The reference file is an automatic Faster Whisper `small.en` transcript created locally on
2026-11-24. It has not undergone a full human listening review. Names, numbers, currency
amounts, and unusual phrases may contain transcription errors.

The call contains speculative financial, tax, and cryptocurrency claims. It is retained for
research and evaluation only and is not financial, tax, or investment advice.

Source ownership and public redistribution clearance have not been established. The
repository's code license does not grant rights to this recording or its derived text and
questions.

Only `documents/` and `benchmark.json` are uploaded by the runner. Reference text stays local.

```dotenv
AUTORAG_INPUT_DATA_KEYS=["data/rag/audio/customer_billings/documents"]
AUTORAG_TEST_DATA_KEY=data/rag/audio/customer_billings/benchmark.json
```
