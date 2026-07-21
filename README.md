# HBDRPTW-F Benchmark Instances and Numerical Results

This repository contains the test instances and 10-run numerical results reported in the manuscript **“Robust Heterogeneous Bus-Assisted Drone Delivery under Transit Uncertainty and Drone Failures”** for the Heterogeneous Bus-Assisted Drone Delivery Routing Problem with Time Windows and Drone Failures (HBDRPTW-F). It includes real-world, Solomon-derived, and randomly generated instances, together with objective values obtained by JOIH-ALNSLS and the benchmark algorithms.

## Repository contents

```text
instances/
  real-world/          12 real-world instances (A1–A12)
  solomon-derived/     12 Solomon-derived instances
  random/              12 randomly generated instances (R1–R12)
  instance_manifest.csv
results/
  real-world/          10 JOIH-ALNSLS runs for each instance
  solomon-derived/     10 runs for each algorithm and instance
  random/              10 runs for each algorithm and instance
```

## Instance families

### Real-world instances

The real-world set contains 12 instances, A1–A12, with 4–15 customers. All instances use the shared station file `instances/real-world/stations.txt`.

### Solomon-derived instances

The Solomon-derived set contains 12 instances with 20 or 50 customers based on C101, C102, R101, R102, RC101, and RC102. All instances use the shared station file `instances/solomon-derived/stations.txt`.

### Random instances

The random set contains 12 instances, R1–R12, with 20–50 customers. All instances use the shared station file `instances/random/stations.txt`. The customer and station files for each instance are listed in `instances/instance_manifest.csv`.

## Algorithms included in the detailed results

The Solomon-derived and random result files contain 10 runs for each of the following algorithms:

- JOIH-ALNSLS;
- JOIH-ALNSLS-noJoint;
- JOIH-ALNSLS-noDFS;
- JOIH-ALNSLS-noPrune;
- JOIH-VNS-SA; and
- JOIH-SA.

For the real-world instances, 10 JOIH-ALNSLS runs are provided for each instance.

## Result files

Each `*_10_runs.csv` or `all_algorithms_10_runs.csv` file reports one row per run and includes the instance name, customer count, algorithm, run identifier, and objective value.

Field definitions are provided in `results/README.md`.

## Citation

If these instances or results are used in future research, please cite the associated manuscript.
