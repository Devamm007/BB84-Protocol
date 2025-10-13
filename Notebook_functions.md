# Functions

- **`bb84_protocol(n_qubits=10, noise_prob=0.0, eve_prob=0.0)`**:
  - Simulates the full BB84 protocol.
  - Generates random bits/bases for Alice and Bob.
  - Builds and runs a quantum circuit with optional noise models.
  - Performs sifting, QBER estimation, and eavesdropping detection.
  - Returns a dictionary with metrics like QBER, sifted/final key lengths, detected eavesdropping, and keys.

- **`print_bb84_results(title, metrics, eve_prob=0, print_keys=True)`**:
  - Prints simulation results in a readable format, including QBER, security status, key lengths, and optional sifted/final keys.

- **`run_scenarios(n_qubits=10, scenario='yyy')`**:
  - Runs predefined scenarios based on the `scenario` string (y/n for each):
    | Scenario          | Parameter | Description                  |
    |-------------------|-----------|------------------------------|
    | Ideal Channel     | ynn      | No noise, no Eve.            |
    | Natural Noise     | nyn      | High noise (0.1), no Eve.    |
    | Eavesdropping     | nny      | No noise, full Eve (1.0).    |
  - Example: `run_scenarios(10, 'nyy')` runs noisy and eavesdropping scenarios.

- **`collect_metrics_for_plotting(n_runs=10, n_qubits=10)`**:
  - Runs multiple simulations to average QBER and detection rates over noise/eavesdropping levels.
  - Returns data for plotting.

- **`plot_bb84_metrics_clear(results_noise, results_eve)`**:
  - Generates two side-by-side plots:
    - Left: QBER vs. Natural Noise (no Eve).
    - Right: QBER and Detection Rate vs. Eavesdropping Probability (no noise).
  - Uses Matplotlib with dual axes for clarity.
