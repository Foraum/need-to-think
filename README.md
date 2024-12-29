# FPGA-Driven Sine Wave Regeneration using ADC-DAC
## **Project Description**
This project demonstrates the design and implementation of a system capable of regenerating an analog sine wave using an FPGA and peripheral devices like ADC and DAC. The system employs the Serial Peripheral Interface (SPI) protocol to facilitate communication between the FPGA and external components.

The project is divided into three distinct tasks:

* VHDL Code Development for SPI Master and SPI Slave
* -  ADC to LCD via SPI
  -  SPI to DAC and multimeter
* Regeneration of Sine Wave using ADC - DAC

For more details on the problem statement, refer to the [Project Question Paper PDF](ProjectQuestionPaper.pdf).

## **Key Components**

| **Technology/Component**    | **Details**                                                                                          | **Quantitative Features**                                      |
|------------------------------|------------------------------------------------------------------------------------------------------|---------------------------------------------------------------|
| **SPI (Serial Peripheral Interface)** | A synchronous, full-duplex protocol for short-distance communication.                           | - Signals: MOSI, MISO, SCLK, CS<br>- Clock Frequency: 1 MHz<br>- Configuration: Mode 0 (CPOL = 0, CPHA = 0) |
| **ADC (Analog-to-Digital Converter)**  | Component: MCP3008<br>Converts analog signals into 10-bit digital values.                       | - Resolution: 10 bits<br>- Input Voltage Range: 0–3.3V<br>- Sampling Rate: 200 kSPS |
| **DAC (Digital-to-Analog Converter)**  | Component: MCP4921<br>Converts 10-bit digital data back to analog form.                        | - Resolution: 10 bits<br>- Output Voltage Range: 0–3.3V<br>- Reference Voltage: 3.3V |
| **FPGA (Field-Programmable Gate Array)** | FPGA Board: XEN 10<br>Handles SPI Master implementation and ADC/DAC communication.       | - SPI Clock Frequency: 1 MHz<br>- Registers for Data Storage: 10-bit width |
| **LCD Display**              | Displays intermediate values, such as voltage calculated from ADC data.                             | - Display Units: Voltage (scaled using 3.3/1024) |

## Task Workflow 
### Task 1 
Implement SPI communication between Master and Slave.
Files:
- [SPI Master VHDL Code](
- [SPI Slave VHDL Code]
- [Toplevel VHDL Code]
- [Testbench VHDL Code] 

