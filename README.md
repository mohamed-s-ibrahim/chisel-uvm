# chisel-uvm

This repo is for the project to explore the combination and interaction of Chisel
and UVM.


# UVM Examples
In the [sv](sv) directory, a number of UVM examples are located. 
## Simple examples
 In `sv/uvm-simple-examples` a number of simple examples are located. These start with a very basic testbench with no DUT attached, and gradually transition into a complete testbench.

## Vivado UVM Examples
These examples assume that a copy of Xilinx Vivado is installed and present in the PATH. The examples are currently tested only on Linux.
* The first example is taken from [Vivado Design Suite Tutorial - Logic Simulation](https://www.xilinx.com/support/documentation/sw_manuals/xilinx2020_1/ug937-vivado-design-suite-simulation-tutorial.pdf)


# Leros ALU
In the directory `sv/leros`, the [Leros ALU](src/main/scala/leros/AluAccuChisel.scala) is tested using UVM, to showcase that Chisel and UVM can work together. This testbench is reused to also test a VHDL implementation of the ALU, to show that UVM is usable on mixed-language designs (when using a mixed-language simulator).

The VHDL implementaion is run by setting the makefile argument `TOP=top_vhd`.