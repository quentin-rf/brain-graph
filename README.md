# Brain Signals Graph

## Background Information

An electroencephalogram (EEG) is a test used to measure electrical activity of the brain,
specifically voltage fluctuations that occur when neurons communicate with each other via
electrical impulses. EEG signals are classified into different brain wave types based on
their frequency bands. The brain waves are divided into five main types: Delta, Theta,
Alpha, Beta and Gamma. Each frequency represents a different brain wave type which can be
seen in the table below.

| Brain Wave Type | Frequency Range (Hz) | Represents                          |
| --------------- | -------------------- | ----------------------------------- |
| Delta           | 0.5 - 4              | Deep sleep, unconsciousness         |
| Theta           | 4 - 8                | Light sleep, relaxation, creativity |
| Alpha           | 8 - 13               | Calm, relaxed, but alert            |
| Beta            | 13 - 30              | Active thinking, focus, high alert  |
| Gamma           | 30 - 100             | High-level information processing   |

A given EEG signal is associated with a reading at a given timestamp. An example signal is as follows:

```json
{
  "timestamp": "2023-10-01T12:00:00Z",
  "delta": 2.5,
  "theta": 5.0,
  "alpha": 10.0,
  "beta": 20.0,
  "gamma": 40.0
}
```

## Problem Statement

Model EEG signal data as a graph data structure to facilitate analysis and visualization of
the dataset. The graph should be able to represent various relationships between the EEG signals, such as but not limited to how EEG signals change over time, how different brain regions interact at the same moment, EEG signals with the same brainwave type and brain signals that are highly similar. Use path traversal algorithms to simulate how signals propagate through the brain.
