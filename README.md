# Memory Allocator Simulator

An interactive Python-based memory allocation simulator that demonstrates concepts like memory management, external fragmentation, and memory compaction.

## Overview

This simulator provides a practical demonstration of how operating systems manage memory allocation for processes. It implements the First-Fit allocation strategy and shows how memory fragmentation occurs and how compaction helps solve this issue.

## Features

- Allocate memory to processes using First-Fit algorithm
- Release memory when processes terminate
- Visualize memory layout showing allocated and unused blocks
- Detect external fragmentation issues
- Perform memory compaction to consolidate free space
- Interactive command-line interface

## Concepts Demonstrated

- **Memory Allocation**: The process of assigning memory blocks to processes
- **First-Fit Algorithm**: Allocates the first memory block that is large enough
- **External Fragmentation**: When free memory exists in non-contiguous blocks, making it unusable for large processes
- **Memory Compaction**: The process of moving allocated memory blocks to consolidate free space

## How to Use

1. Run the program: `python memory_allocator.py`
2. Enter the number of initial processes to create
3. For each process, specify its size in KB
4. Use the menu to:
   - Add new processes
   - Release existing processes
   - View the current memory status
   - Perform memory compaction
   - Exit the program

## Example Scenario

1. Create several processes of different sizes
2. Release a process in the middle
3. Try to add a new process that's larger than any single free block
4. Observe the external fragmentation error
5. Perform memory compaction
6. Retry adding the new process and observe success

## Code Structure

- `MemoryAllocator` class: Handles the core memory management functionality
- `interactive_allocator()` function: Provides the user interface
- Memory representation: List of tuples containing (status, start_address, end_address)

## Requirements

- Python 3.x
- No external libraries required

## Educational Use

This simulator is perfect for computer science students learning about:
- Operating systems concepts
- Memory management techniques
- Process allocation strategies
- Memory fragmentation issues

## Future Enhancements

- Graphical user interface to visualize memory blocks
- Support for Best-Fit and Worst-Fit allocation algorithms
- Process priority handling
- Simulated virtual memory with paging


