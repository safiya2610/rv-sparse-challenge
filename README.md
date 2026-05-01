# RV-Sparse Coding Challenge

## Overview
This project implements sparse matrix-vector multiplication using the Compressed Sparse Row (CSR) format.

The implementation converts a dense row-major matrix into CSR representation and computes y = A * x efficiently using only non-zero elements.

## Key Features
- Zero dynamic memory allocation inside the function
- Efficient CSR construction
- Optimized sparse matrix-vector multiplication
- Handles varying matrix sizes and densities

## Approach
1. Scan matrix row-wise
2. Store non-zero values in `values`
3. Store column indices in `col_indices`
4. Maintain row boundaries using `row_ptrs`
5. Compute result using CSR traversal

## Complexity
- Time Complexity: O(rows × cols)
- Space Complexity: O(nnz)

## Result
All randomized test cases passed with zero numerical error.

## Output
<img width="929" height="933" alt="Screenshot (2602)" src="https://github.com/user-attachments/assets/2228cba7-17d6-4107-ba7e-7be08cc69553" />

<img width="948" height="923" alt="Screenshot (2604)" src="https://github.com/user-attachments/assets/806216cb-8e96-4414-8f37-12d8e86ded59" />
