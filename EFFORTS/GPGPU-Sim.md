# Notes

- GPGPU-Sim was created by <mark style="background: #FFF3A3A6;">Tor Aamodt's</mark> research group at the University of British Columbia.
- GPGPU-Sim models the features of a modern graphics processor that are relevant to non-graphics applications.
- Creating benchmarks for the original GPGPU-Sim simulator was a very time consuming process and the validity of code generation for CPU run on a GPU was questioned by some.
	- These issues motivated the development an interface for directly running CUDA applications to leverage the growing number of applications being developed to use CUDA.
- subsequently added support for OpenCL and removed all SimpleScalar code.
- The interconnection network is simulated using the <mark style="background: #08BFFF99;">booksim</mark> simulator developed by Bill Dally's research group at Stanford.

## GPUWatcch

- GPUWattch (introduced in GPGPU-Sim 3.2.0) was developed by researchers at the <mark style="background: #FFF3A3A6;">University of British Columbia</mark>, the University of Texas at Austin, and the University of Wisconsin-Madison.
- GPUWattch leverages <mark style="background: #08BFFF99;">McPAT</mark>, which was developed by <mark style="background: #FFF3A3A6;">Sheng Li et al.</mark> at the University of Notre Dame, Hewlett-Packard Labs, Seoul National University, and the University of California, San Diego.
