# Lab 1: Thirty-One Day Month

VHDL template for ECE 281 [Lab 1](https://usafa-ece.github.io/ece281-book/lab/lab1.html)

Targeted toward Digilent Basys3 in Vivado 2024.

Tested on Windows 10.

## Usage

Clone and cd into the directory.

You should see a `.xpr` file. Open it with Vivado!

## GitHub Actions Testbench

The workflow uses the [setup-ghdl-ci](https://github.com/ghdl/setup-ghdl-ci) GitHub action
to run a *nightly* build of [GHDL](https://ghdl.github.io/ghdl/).

First, the workflow uses GHDL to **analyze** all `.vhd` files in `src/`.

Then it **elaborates** `thirtyOneDayMonth_tb` entity.

Finally, the workflow **runs** the simulation. If successful then it will quietly exit with a `0` code.
If any of the `assert` statements fail then GHDL will cease the simulation and exit with non-zero code; this will also cause the workflow to fail.
Assert statements of other severity levels will be reported, but not fail the workflow.

Documentation Statement: Capt Brian Yarbrough helped me with the breadboard implementation of the 
integrated part of the lab by explaining that I can convert the 8:1 to 4:1 mux by grounding the later 
half of the data inputs and replicating the boolean equation made in the pre lab by mapping the left 
inputs to high voltage and ground, and that the original truth tables doesn't have to be implemented. 
C3C Dexter James helped me with the my VHDL code by explaining that 
in the test bench I need to use hex instead of binary to assign the test cases to the truth table.
I used https://surf-vhdl.com/how-to-implement-digital-mux-in-vhdl/ to see other ways to implement the 
mux in the VHDL and to troubleshoot my syntx that was failing on 8th iteration. Turned out my logic
statements in architecture were misaligned, which did not prompt the syntax error, but made the
simulation fail