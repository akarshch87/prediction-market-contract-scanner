# Kalshi Market Integrity Scanner

A Python scanner that monitors public market metadata for potential contract inconsistencies and places candidates in a local review queue. Each finding includes evidence for a human to inspect.

The scanner uses six checks, keeps market snapshots in SQLite, and rechecks contract changes without rerunning validation for ordinary quote updates. A versioned fingerprint also makes it possible to revalidate saved markets after the checks change.

A reproducible study runs the full review queue on 1,200 fictional contracts from 12 scenarios. It reports precision, recall, and missed cases. The sample is synthetic and does not establish real market accuracy.

Download and extract `kalshi-scanner-source.zip` for the source, setup instructions, tests, and study. The project reads public data and does not place orders or submit reports.
