# NEXORA AI — Performance Evaluation

NEXORA AI treats optimization as an engineering measurement problem rather than a claim.

## Metrics

| Metric | Purpose |
|---|---|
| AI inference latency | Measures time required to produce an inference result. |
| Model loading time | Measures startup/model initialization overhead. |
| Memory consumption | Measures runtime memory requirements. |
| Throughput | Measures the amount of work completed over time. |
| Response time | Measures end-to-end user-perceived responsiveness. |
| CPU/GPU/NPU utilization | Shows hardware resource usage where measurable. |
| Power efficiency | Evaluates performance relative to energy consumption. |
| Offline responsiveness | Measures behavior without cloud connectivity. |
| Local vs cloud comparison | Quantifies differences between execution approaches. |

## Recommended Benchmark Protocol

1. Record the exact Snapdragon device and system configuration.
2. Record model name, model version, precision and runtime.
3. Use identical input workloads for comparable runs.
4. Warm up the runtime before collecting steady-state measurements.
5. Repeat each workload multiple times.
6. Report median latency and an appropriate spread such as p95 when enough samples are available.
7. Record memory and hardware utilization during the same workload.
8. Clearly distinguish measured values from theoretical specifications.

## Reproducibility

Every published benchmark should identify:

- Hardware model
- OS/build
- Model and version
- Runtime/backend
- Input size or workload
- Number of runs
- Measurement method
- Date of measurement

No benchmark result should be represented as a measured result unless it has actually been collected using the documented procedure.
