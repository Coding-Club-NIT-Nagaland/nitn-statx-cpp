# 🧮 NITN-StatX (C++)

**NITN-StatX** is a high-performance C++ statistical and probabilistic library built by **NIT Nagaland Coding Club**.  
Designed for deterministic behavior, fast sampling, and scientific computing.

## 🚀 Features
- PDF, CDF, Quantiles for core distributions (Normal, Uniform, Exponential, Poisson)
- Hypothesis Tests (t-test, Chi-Square, Kolmogorov–Smirnov)
- Random Sampling & MCMC (Metropolis-Hastings)
- Bayesian Updating (Conjugate Priors)
- Time Series Utilities (Moving Average, ARIMA skeleton, Kalman Filter)
- Deterministic RNG with seeding support

## 🧰 Build & Install

```bash
git clone https://github.com/NITN-Coding-Club/nitn-statx-cpp.git
cd nitn-statx-cpp
mkdir build && cd build
cmake ..
make
```

To use in your project, include the headers and link against the built library (or copy headers for header-only usage if designed that way).

## 🧪 Quick Start

```cpp
#include <iostream>
#include "distributions/Normal.hpp"

int main() {
    Normal dist(0.0, 1.0);
    double p = dist.cdf(1.96);
    auto samples = dist.sample(1000);
    std::cout << "CDF at 1.96: " << p << std::endl;
    return 0;
}
```

## 📂 Project Structure

```
nitn-statx-cpp/
├── include/
│   ├── distributions/
│   ├── stats/
│   ├── sampling/
│   ├── bayesian/
│   └── timeseries/
├── src/
├── tests/
├── examples/
└── README.md
```

## 🤝 Contributing

We welcome contributions from students and developers:

1. Fork the repository  
2. Implement your feature in `include/` and `src/` as needed  
3. Add unit tests in `tests/`  
4. Run tests with `ctest` or your build system  
5. Submit a Pull Request 🚀

Follow modern C++ practices (C++17 or higher), const-correctness, and clear documentation.

## 🧑‍💻 Maintainers

* NIT Nagaland Coding Club  
* [GitHub Organization](https://github.com/NITN-Coding-Club)
