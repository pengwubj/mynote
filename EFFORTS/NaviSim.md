# Unknown Things

1. BICG benchmarks from PolyBench
2. MGPUSim
3. Performance discrepancies
4. Akita simulation engine
5. DRAMSim3
6. HBM
7. GDDR
8. Daisen GPU visualization framework
9. photolithography technology
10. Barriers in work-groups in GPUs.
11. What are work-items, work-groups, wavefront?
    > WaveFront: Group of threads that are executed simultaneously using SIMD
12. Lock-step execution
13. Thread divergence
    > -  is a phenomenon that occurs in parallel computing when different threads in a warp take different paths through the code.
    >   -  happens when a thread encounters a conditional statement and the condition evaluates to different values for different threads.
14. What is a Kenel in GPUs?
15. Multi2Sim
16. GPGPUSim
---
# Architectures
## Compute Unit on a GPU 
- responsible for instruction execution and data processing
-  1 Scheduler
  can fetch and issue instructions for up to 40 wavefronts.
  40 wavefront handling
	- decode 5 instruction
	  and issue to 5 execution units
		- 1 branch unit 
		- 1 scalar unit(executes instruction manipulating data shared by work-items in a wavefront)
		- 1 LDS(Local Data Share)
		- 1 vector memory unit 
		- 4 SIMD unit 
- 1 SIMD unit 
	- responsible for executing vectorized floating-point instruction for 10 out 40 wavefronts
	- contains 16 single-precision ALUs
	- => 64-work-item wavefront takes 4 cycles to finish

---
# Tasks

- [ ] Go through the RDNA Whitepaper.
