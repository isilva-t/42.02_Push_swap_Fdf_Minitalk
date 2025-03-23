# Push_swap

![Push_swap Program Flow Diagram](./docs/prog_map.jpg)

## About
A sorting algorithm project that uses two stacks and a limited set of operations to sort integers with minimal moves.

## The Algorithm
- For small stacks (2-5 numbers): Optimized hard-coded solutions
- For larger stacks: Radix sort with binary representation
  - Convert numbers to 32-bit binary strings
  - Sort by processing one bit at a time, moving numbers between stacks

## Available Instructions
```
sa, sb, ss  - Swap the top elements
pa, pb      - Push elements between stacks
ra, rb, rr  - Rotate (shift up all elements)
rra, rrb, rrr - Reverse rotate (shift down)
```

## Usage
```
./push_swap 4 67 3 87 23
```

To validate:
```
ARG="4 67 3 87 23"; ./push_swap $ARG | ./checker_OS $ARG
```

## Learning Focus
- Practical understanding of linked lists
- Algorithm optimization
