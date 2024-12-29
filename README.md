# FPGA-Driven Sine Wave Regeneration using ADC-DAC
## Project Description
This project focuses on the implementation of the Serial Peripheral Interface (SPI) protocol by interfacing an Analog-to-Digital Converter (ADC) and a Digital-to-Analog Converter (DAC) with an FPGA. The primary aim of the project is to regenerate a sine wave using these components, demonstrating the real-time conversion of analog signals to digital and back to analog.

The project is divided into three distinct tasks:

* VHDL Code Development for SPI Master and SPI Slave
* -  ADC to LCD via SPI
  -  SPI to DAC and multimeter
* Regeneration of Sine Wave using ADC - DAC

For more details on the problem statement, refer to the [Project Question Paper PDF](ProjectQuestionPaper.pdf).

## Features 
1. **SPI Protocol**
   - Implemented with a **10 MHz clock** using **Mode 0**:
     - Clock idle state is low.
     - Data sampled on the rising edge.
   - Data Exchange:
     - **Master** transmits **5** on **MOSI**.
     - **Slave** transmits **7** on **MISO** simultaneously.

2. **ADC Integration**
   - **MCP3008 ADC** converts **0–2V sine wave** to **10-bit digital values**.
   - Interfaced with FPGA via SPI.

3. **DAC Integration**
   - DAC was already on  **Xilinx Spartan-10 (XEN 10)** FPGA board.
   - Analog output verified using a **Digital Storage Oscilloscope (DSO)**.

## Repository Structure 
The repository is organized as follows:
| File/Folder         | Description                                                  |
|---------------------|--------------------------------------------------------------|
| 
