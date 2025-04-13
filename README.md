🧠 Overview


This project implements the Merge Sort algorithm using parallel processing in C++. By leveraging multithreading, the sorting process is significantly accelerated—especially for large datasets. The implementation showcases the use of thread pools and efficient synchronization mechanisms to optimize performance.



🚀 Features


Parallel Processing: Sorts using multiple CPU threads concurrently to reduce execution time.

Thread Pool: Efficiently manages threads to avoid the overhead of frequent thread creation and destruction.

Performance Benchmarking: Compares execution time between traditional Merge Sort and the parallel implementation.



⚙️ Implementation Details


The algorithm enhances traditional Merge Sort through parallelism. Key components include:

Recursive Division: Splits the dataset into smaller subarrays until a set threshold.

Parallel Sorting: Sorts subarrays in parallel using multiple threads.

Merging: Combines sorted subarrays into the final sorted array.



🧵 Thread Pool


A thread pool is used to manage and synchronize threads efficiently. This minimizes overhead and improves CPU resource utilization, leading to faster execution.

📊 Performance Comparison


Benchmark tests on a LENOVO Ideapad Gaming 3 Laptop show a clear advantage of the parallel approach:

Standard Merge Sort: ~25 seconds

Parallel Merge Sort: ~1 second

💡 That's a 25x speed boost through multithreading!

🔧 Getting Started
✅ Prerequisites
C++ Compiler (supporting C++11 or later)

CMake (optional, for build automation)

📦 Installation & Running
bash
Copy
Edit
# Clone the repository
git clone <repo-url>

# Navigate to project directory
cd parallelMergeSort/src/app

# Compile and run
g++ main.cpp -o main
./main
