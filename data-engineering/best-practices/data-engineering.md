# Data Engineering Practices
- Define and preserve schemas, types, key columns, null rules, partitions and timezones.
- Prefer idempotent, replay-safe loads; handle duplicates, late events, nulls and malformed data deliberately.
- Advance watermarks/checkpoints only after successful durable writes; bound backfills.
- For SQL, parameterize values, avoid unbounded scans and filter partitions early.
- For Spark, favor built-in functions over UDFs and avoid unnecessary collect(), cache, repartition or costly shuffles.
- In Airflow, keep DAG parsing lightweight, tasks retry-safe and dependencies explicit.
- In Kafka/streaming, document delivery semantics, offset handling, event-time assumptions and recovery behavior.
- Validate record counts, schemas, keys, incremental boundaries and failure/retry paths.
- Follow established Jenkins, Docker, EKS and environment conventions where applicable.
