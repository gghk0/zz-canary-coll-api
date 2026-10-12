# ZZ Canary Coll API

Collection-parser canary fixture for Agent Context ingestion testing (team 46199161).

- Spec: [`openapi.yaml`](./openapi.yaml)
- Collections: [`postman/collections/`](./postman/collections) — one benign ("ZZCOLLCTRL_*"),
  one carrying inert breaker strings in collection/item/variable names ("ZZCOLLBREAK_*").

All breaker characters are inert text; they matter only if the ingestion writer
concatenates these strings into a query.
