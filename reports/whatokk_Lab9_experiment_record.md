# Lab9 Experiment Record

- Experiment: Distributed Object Storage & Fault Tolerance Testing
- Repository: https://github.com/whatokk/lab9-distributed-object-storage
- Successful Actions run: https://github.com/whatokk/lab9-distributed-object-storage/actions/runs/27364710248
- Execution environment: GitHub Actions Ubuntu runner
- Storage simulation: MinIO with four mounted directories data1, data2, data3, data4
- Bucket: my-cloud-storage
- Test object: bigfile.bin, 20 MiB
- Fault simulation: stopped cluster, deleted and recreated data3, restarted cluster
- Result: object remained accessible; original and recovered files had identical SHA256 hash
- Generated at: 2026-06-12 01:25:22 +08:00

## Key Results

MinIO distributed storage split object data and metadata across all four storage directories. After data3 was removed and recreated, the object `bigfile.bin` was still listed and readable. The SHA256 hashes of `bigfile.bin` and `recovered-bigfile.bin` matched exactly, verifying fault tolerance through erasure coding and distributed redundancy.
