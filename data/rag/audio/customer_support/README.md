# Customer support recording

This dataset contains one English customer-support call:

| Recording | Reference text | Benchmark questions |
| --- | --- | ---: |
| `documents/en-customer-support-standard.mp3` | `reference/en-customer-support.txt` | 10 |

The reference file is an automatic Faster Whisper `small.en` transcript created locally on
2026-11-24. It has not undergone a full human listening review. Names, numbers, and unusual
phrases may contain transcription errors.

The call includes remote-access and payment-application instructions. It is retained for
research and evaluation only and should not be treated as legitimate support guidance.

Source ownership and public redistribution clearance have not been established. The
repository's code license does not grant rights to this recording or its derived text and
questions.

Only `documents/` and `benchmark.json` are uploaded by the runner. Reference text stays local.
The original 8 kHz MPEG-2.5 recording is retained in `source/` and is not uploaded.

```dotenv
AUTORAG_INPUT_DATA_KEYS=["data/rag/audio/customer_support/documents"]
AUTORAG_TEST_DATA_KEY=data/rag/audio/customer_support/benchmark.json
```
