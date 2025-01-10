# Stream Mining Approaches for Data Minining
 This project implements essential stream mining algorithms, including Reservoir Sampling, Bloom Filter, and Flajolet-Martin for probabilistic counting. These algorithms are designed to efficiently process large data streams, providing methods for random sampling, set membership testing, and cardinality estimation

# Stream Mining: Reservoir Sampling, Bloom Filter, and Flajolet-Martin

This project implements key **stream mining** algorithms including **Reservoir Sampling**, **Bloom Filter**, and **Flajolet-Martin** for probabilistic counting. These algorithms are designed to process large data streams efficiently and estimate cardinality or provide membership checks.

## Overview

The project tackles three essential stream mining tasks:

1. **Reservoir Sampling**: Selects a random sample of size \( k \) from a large data stream.
2. **Bloom Filter**: Checks for set membership with a low false positive rate, using multiple hash functions.
3. **Flajolet-Martin Algorithm**: Estimates the cardinality of a stream using hash functions and trailing zeros.

### Key Tasks:
1. **Reservoir Sampling**: Efficiently sample \( k \) elements from a stream.
2. **Bloom Filter**: Implement a probabilistic data structure to test set membership.
3. **Flajolet-Martin Algorithm**: Estimate the number of distinct elements in a stream using hash functions.

## Code Structure

The project contains three Python files, each implementing a core algorithm:
1. **`reservoir_sampling.py`**: Reservoir Sampling algorithm.
2. **`bloom_filter.py`**: Bloom Filter algorithm with multiple hash functions.
3. **`flajolet_martin.py`**: Flajolet-Martin algorithm for probabilistic counting.

### Algorithms Implemented:
- **Reservoir Sampling**: Randomly samples from a stream to maintain a representative subset.
- **Bloom Filter**: Checks membership in a set with the possibility of false positives but no false negatives.
- **Flajolet-Martin**: Estimates stream cardinality based on the number of trailing zeros in hashed values.

## Output

Each algorithm produces different outputs:
- **Reservoir Sampling**: Returns a list of sampled elements.
- **Bloom Filter**: Returns whether an element is likely in the set or definitely not.
- **Flajolet-Martin**: Estimates the cardinality of the stream.

Example outputs include:
- Sampled data points for Reservoir Sampling.
- False positive rate for the Bloom Filter.
- Estimated cardinality for Flajolet-Martin.

## Results & Discussion

- **Reservoir Sampling**: Ensures that the sample is representative of the entire stream without storing the full data.
- **Bloom Filter**: Offers an efficient membership test with a trade-off between false positives and memory usage.
- **Flajolet-Martin**: Provides a highly efficient way to estimate cardinality, especially for large data streams.

## Conclusion

This project demonstrates efficient algorithms for stream mining, enabling real-time data analysis in environments with large or continuous data. Each algorithm is optimized for memory and computation, making them suitable for large-scale applications like monitoring, recommendation systems, and fraud detection.

## References

1. **Muthukrishnan, S. (2005).** Stream Mining: Algorithms and Applications.
2. **Flajolet, P., & Martin, W. (1985).** Probabilistic Counting Algorithms for Data Base Applications.
