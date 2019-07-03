# MODULE 02-03 MODERN COMPUTER SYSTEMS

## SECTION 01 INSTRUCTION SET ARCHITECTURES

**Complex Instruction Set Computers (CISC):**

* Different kinds
* Different formats
* Different lengths
* Different operation codes

**Procedure Call** - Sets out of instruction to input of next instruction

## SECTION 02 MEMORY ENHANCEMENTS

**CPU**

Faster than memory (2GHz CPU vs. 70ns DRAM)

**Memory**

Cache memory, set addresses to subsections, parallel fetch

Memory Cache:

* 90% hit and 50% improved execution speed
* Locality and small region size important

## SECTION 03 EMERGING TRENDS

Multi-core chips- 2+ CPUs in a single integrated circuit package

Cluster computing - 100+ computers working together

Instruction pipelining - assembly line technique for overlapping fetch-execute cycles

Hardware programming - speed vs physical space requirements

## SECTION 04 COMPUTER ORGANIZATION

Mainframe organization - PC organization with channel support for workstations

## SECTION 05 IMPROVING PERFORMANCE

Improving performance:

* Faster clock speeds
* Faster buses and circuits
* Wider instruction and data paths
* More and faster memory
* Faster disks

Multiprocessing - PC has 2+ CPUs for faster and parallel processing

* Tightly coupled CPUs share memory and I-O as manager-worker or symmetic (SMP)
* SMP more reliable but vulnerable to parallel instruction run errors

* Loosely coupled CPUs are clustered, each system has own CPU, memory, and I-O facility
	* Shared-nothing model - no sharing of resources, pass messages to partition work

Multiprogramming - 2+ programs running on PC at same time

Cluters:

* Externally seen as single computing unit
* Load balancing evens out workload
* Blade components - computers mounted on motherboard plugged into rack connectors

Massively parallel processor architecture (MPP):

* Good at problems with subtasks
* Cloud (grid) computing - supercomputer performance through distributed network PCs

Parallel computers - 100000+ CPUs with small local memory and shared global memory

