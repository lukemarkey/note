# Module 02-02: Digital Logic, CPU, Memory

## The CPU & Memory

Registers:

1. Small, fast storage within the CPU
2. One input, 1-2 outputs
3. 02-64 bits wide
4. Made up of Latches and Buffers

* Latch

    1. Stores 1 bit of data
    2. Can be strung together (8-bit latch is really 8 1-bit latches)

Tri-State Buffer
3 States: Zero, One, Disconnected
Can completely disable digital logic

Registers Contain:
Memory address register - holds address in memory from which to read and write data
Memory data register - holds data or instruction words to read or write from

* Holds one memory word - 32-bit word means MDR is required to be 32 bits large

Program counter - holds address of next instruction
Instruction register - holds instruction fetched by address in program counter

* Decode phase examines contents of register to decide which operation to perform

    Register operations - stores data values temporarily and retrieves results of operations (addition, etc.)
    Instruction Cycle
    Fetch - get instruction from MAR from program counter and advance program counter
    Decode - determine operation and data
    Execute - perform operation
    Register Transfer Language
    Execute part of instruction cycle, sends contents of one or two registers through ALU
    Register operations are described with RTL

Data register - 16-32-64-128 number of data registers is typical

    Accumulator - when a computer has only one data register (calculator display)

The Datapath and Control Unit

Arithmetic-Logic Unit (ALU)
Passes to P, Z, and V
Outputs to Bus C
Inputs from Bus A and B
Diagrammed as a v-shaped parallelogram
P flag - Allow or disallow data within the operation
Z flag - inverse the data within the operation

Control Unit
Outputs to ALU
Reads data from registers
P and Z flags from ALU which are stored in a latch
Receives: 4 bits of operation code from instruction register (IR)
Generates: 4 bits of ALU control input (EnaA, InvA, EnaB, Inc) (28-bit total)
Generates: R/W and presence-detect signals for memory and registers

## Connecting With Memory

Random Access Memory (RAM)
“Random access” - any cell may be addresses as fast as any other
Dynamic RAM (DRAM) - loses contents when powered off (volatile) and refreshed thousands of times per second
Static RAM (SRAM) - expensive, faster, no refresh, volatile
SDRAM - DRAM with static buffer

Flash Memory
Non-volatile
Faster than magnetic disks, more expensive, slower than RAM
Uses: BIOS, SSD, digital cameras, thumb drives

## Buses

Definition - physical connection that makes it possible to transfer data from one location in computer system to another
Serial - one bit transmitted at a time
Signals:

    Data
    Addresses
    Control signals

Protocol - documented agreement for communication

## Instructions & Instruction Types

Elements of an Instruction
Operation code (op-code) - commands control unit and ALU what to do
Operands - address of data to be used in operation

