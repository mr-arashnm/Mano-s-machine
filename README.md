# Computer Architecture Implementation in Verilog (Based on Mano's Book)

This repository contains the Verilog implementation of a computer architecture as described in Mano's book on computer system architecture. The project includes various modules, testbenches, and synthesis/implementation scripts to simulate, synthesize, and implement the computer on an FPGA.

## Project Structure

- **`CPU.srcs`**: Contains the Verilog source files and testbenches.
  - `sources_1`: Verilog modules for the computer design.
  - `sim_1`: Testbenches for simulation.
- **`CPU.runs`**: Contains synthesis and implementation runs.
  - `synth_1`: Synthesis scripts and logs.
  - `impl_1`: Implementation scripts and logs.
- **`CPU.cache`**: Stores intermediate files and IP cache data.
- **`CPU.xpr`**: The Vivado project file.

## Key Modules

- **`ALU.v`**: Arithmetic Logic Unit for performing arithmetic and logical operations.
- **`BUS.v`**: Bus module for communication between components.
- **`CPU.v`**: Top-level module integrating all components of the computer.
- **`Control_Unit.v`**: Control unit for managing instruction execution.
- **`Memory.v`**: Memory module for data storage.

## Testbenches

- **`ALU_TB.v`**: Testbench for the ALU module.
- **`BUS_TB.v`**: Testbench for the BUS module.
- **`CPU_TB.v`**: Testbench for the top-level computer module.
- **`Memory_TB.v`**: Testbench for the Memory module.

## Synthesis and Implementation

- **Vivado Version**: 2022.2
- **Target Device**: `xc7z020clg400-1` (Zynq-7000)
- **Synthesis Strategy**: Vivado Synthesis Defaults
- **Implementation Strategy**: Vivado Implementation Defaults

## How to Use

1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd CPU
   ```

2. **Open in Vivado**:
   - Launch Vivado 2022.2.
   - Open the `CPU.xpr` project file.

3. **Run Simulation**:
   - Select the desired testbench from the `sim_1` file set.
   - Run the simulation to verify functionality.

4. **Synthesize and Implement**:
   - Run the `synth_1` and `impl_1` flows to generate the bitstream.

5. **Program FPGA**:
   - Use the generated bitstream to program the FPGA.

## Dependencies

- **Xilinx Vivado 2022.2**
- **Zynq-7000 FPGA**

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests to improve the project.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

Special thanks to the Xilinx community for their tools and documentation.

---
