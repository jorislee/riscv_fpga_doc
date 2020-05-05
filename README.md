#### 开源 FPGA 生态

1. 公司:  Lattice

   - 低端产品线: [Lattice iCE40](https://github.com/SymbiFlow/symbiflow-arch-defs/blob/master/ice40)
     - 开发软件: [Yosys](https://github.com/YosysHQ/yosys) +  [nextpnr](https://github.com/YosysHQ/nextpnr) + [icestorm](https://github.com/cliffordwolf/icestorm) , 其中  [arachne-pnr](https://github.com/YosysHQ/arachne-pnr) 混用, 是 [nextpnr](https://github.com/YosysHQ/nextpnr)  早期版本.

   - 高端产品线: [ECP5]()
     - 开发软件: [Yosys](https://github.com/YosysHQ/yosys) +  [nextpnr](https://github.com/YosysHQ/nextpnr) + [Trellis](https://github.com/SymbiFlow/prjtrellis) 

2. 公司: Xilinx

   - 支持开源产品: [Xilinx 7-series]()
     - 开发软件: [Yosys](https://github.com/YosysHQ/yosys) +  [nextpnr-xilinx](https://github.com/daveshah1/nextpnr-xilinx) + [Project X-Ray](https://github.com/SymbiFlow/prjxray) 



#### 文档整理

1. [SymbiFlow](https://symbiflow.github.io/) FPGA 开源框架, 整合编译工具链. [相关文档](https://symbiflow.readthedocs.io/en/latest/toolchain-desc/design-flow.html)
2. meta-hdl](https://github.com/nathanrossi/meta-hdl) FPGA 整合编译工具链.
3. blacksoc](https://github.com/lawrie/blacksoc) 适配 picorv32 外设组件库.
4. computer-engineering-resources](https://github.com/rajesh-s/computer-engineering-resources) 计算机工程资料索引.



#### Toolchain

| Component(组件)                                              | Function(功能)            | 开发板          | License                                                      |
| ------------------------------------------------------------ | ------------------------- | :-------------- | :----------------------------------------------------------- |
| [Yosys](https://github.com/YosysHQ/yosys)                    | Synthesis(综合)           |                 | [ISC](https://opensource.org/licenses/ISC)                   |
| [Icarus Verilog](http://iverilog.icarus.com/)                | Simulation(仿真)          |                 | [GPL-2.0](https://opensource.org/licenses/GPL-2.0)           |
| [Verilator](https://www.veripool.org/wiki/verilator)         | Simulation(仿真)          |                 | [LGPL-3.0](https://opensource.org/licenses/LGPL-3.0)         |
| [Arachne-pnr](https://github.com/YosysHQ/arachne-pnr)        | Place & Route(布局和布线) | ICE40           | [MIT](https://opensource.org/licenses/MIT)                   |
| [nextpnr](https://github.com/YosysHQ/nextpnr)                | Place & Route(布局和布线) | ICE40 &ECP5     | [ISC](https://opensource.org/licenses/ISC)                   |
| [IceStorm](https://github.com/cliffordwolf/icestorm)         | Bitstream(位流库)         | ICE40           | [ISC](https://opensource.org/licenses/ISC)                   |
| [Trellis](https://github.com/SymbiFlow/prjtrellis)           | Bitstream(位流库)         | ECP5            | [MIT](https://opensource.org/licenses/MIT)                   |
| [VTR](https://github.com/verilog-to-routing/vtr-verilog-to-routing) | ODIN II + ABC + VPR       |                 |                                                              |
| [ODIN II](code.google.com/p/odin-ii)                         | Synthesis(综合)           |                 |                                                              |
| [ABC](https://github.com/berkeley-abc/abc)                   | 优化与映射                |                 |                                                              |
| [VPR]                                                        | Place & Route(布局和布线) |                 |                                                              |
| [Gaffe-Xilinx](https://github.com/gaffe-logic/gaffe-xilinx)  | Bitstream(位流库)         | Xilinx XC7      | [Apache-2.0](http://www.apache.org/licenses)                 |
| [KinglerPAR](https://github.com/rqou/KinglerPAR)             | Place & Route(布局和布线) | 未完成          | [BSD-2-Clause](https://opensource.org/licenses/BSD-2-Clause) |
| [prjxray](https://github.com/SymbiFlow/prjxray)              | Bitstream(位流库)         | Xilinx 7-series | [ISC](https://opensource.org/licenses/ISC)                   |
| [prjxray-db](https://github.com/SymbiFlow/prjxray-db/)       | Bitstream(位流库)         | Xilinx 7-series | [ISC](https://opensource.org/licenses/ISC)                   |
| [wavedrom](https://wavedrom.com/)                            | waveform(波形或时序图)    |                 |                                                              |
| [Chibi](https://github.com/rqou/project-chibi)               | Bitstream(位流库)         | Intel MAX-V     |                                                              |
| [netlistsvg](https://github.com/nturley/netlistsvg/)         | logic diagrams(逻辑图)    |                 | [MIT](https://opensource.org/licenses/MIT)                   |



### FPGA ICE40UP5K RISC-V 可以实现列表

| Project(项目)                                                | (语言)        | 简述                                                         | License(许可证)                                              |
| ------------------------------------------------------------ | ------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| [picorv32](https://github.com/cliffordwolf/picorv32)         | Verilog       | 面积优先的实现[已测试]                                       | [ISC](https://opensource.org/licenses/ISC)                   |
| [icicle](https://github.com/grahamedgecombe/icicle)          | SystemVerilog | 5 级流水线,静态分支预测，旁路和互锁[已测试]                  | [ISC](https://opensource.org/licenses/ISC)                   |
| [VexRiscv](https://github.com/SpinalHDL/VexRiscv)            | SpinalHDL     | 可配置功能模块[已测试]                                       | [MIT](https://opensource.org/licenses/MIT)                   |
| [rudolv](https://github.com/bobbl/rudolv)                    | Verilog       | [已测试] 3199/ 5280    60%                                   | [ISC](https://opensource.org/licenses/ISC)                   |
| [magouilles](https://github.com/bioe-hubert/magouilles)      | Verilog       | 四级流水线 [已测试]] 4479/ 5280    84%                       | [MIT](https://opensource.org/licenses/MIT)                   |
| [up5k_riscv](https://github.com/emeb/up5k_riscv)             | Verilog       | 基于 picorv32 封装[已经测试]2190/ 5280    41%                | [MIT](https://opensource.org/licenses/MIT)                   |
| [yaricv32](https://github.com/google/yaricv32)               | Verilog       | google 设计[已测试] 2088 / 5280                              | [Apache-2.0](http://www.apache.org/licenses)                 |
| [SERV](https://github.com/olofk/serv)                        | Verilog       | 串行RISC-V 内核(未测试)                                      | [ISC](https://opensource.org/licenses/ISC)                   |
| [VexRiscvSoftcoreContest2018](https://github.com/SpinalHDL/VexRiscvSoftcoreContest2018) | SpinalHDL     | 基于 [VexRiscv](https://github.com/SpinalHDL/VexRiscv) 使用 iCube2 (未测试) | [Apache-2.0](http://www.apache.org/licenses)                 |
| [Sail-RV32I-common](https://github.com/physical-computation/Sail-RV32I-common) | Verilog       | 教学使用(参考)未测试                                         | [MIT](https://opensource.org/licenses/MIT)                   |
| [catena-riscv32-fpga](https://github.com/mcci-catena/catena-riscv32-fpga) | Verilog       | iCube2 (未测试)                                              | [GPL-3.0](https://opensource.org/licenses/GPL-3.0)           |
| [kronos](https://github.com/SonalPinto/kronos)               | SystemVerilog | 最大化利用 fpga, cmake (未测试))                             | [Apache-2.0](http://www.apache.org/licenses)                 |
| [midgetv](https://github.com/bnossum/midgetv)                | Verilog       | 最小资源 (使用 iCEcube2) 未测试                              | [Apache-2.0](http://www.apache.org/licenses)                 |
| [darkriscv](https://github.com/darklife/darkriscv)           | Verilog       | 三级流水线(未测试)                                           | [BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause) |
| [Riscy-SoC](https://github.com/AleksandarKostovic/Riscy-SoC) | Verilog       | 5级流水线(64 位实现), 未编译.                                | [MIT](https://opensource.org/licenses/MIT)                   |
| [glacial](https://github.com/brouhaha/glacial)               | Verilog       | 最小资源 (使用 iCEcube2) 未测试                              | [BSD-2-Clause](https://opensource.org/licenses/BSD-2-Clause)(不清晰) |
| [JiVe](https://github.com/fredrequin/JiVe)                   | Verilog       | 最小资源                                                     | [BSD-2-Clause](https://opensource.org/licenses/BSD-2-Clause) |
| [litex](https://github.com/enjoy-digital/litex)              | Python        | 基于 MiSoC                                                   | [LiteX](https://github.com/enjoy-digital/litex/blob/master/LICENSE) |
| [zipcpu](https://github.com/ZipCPU/zipcpu)                   | Verilog       | 小型 RISC CPU                                                | [GPL-3.0](https://www.gnu.org/licenses/gpl-3.0.en.html)      |



#### 其他 RISCV 实现

| Project(项目)                                          | (语言)  | 简述                                 | License(许可证)                                              |
| ------------------------------------------------------ | ------- | :----------------------------------- | :----------------------------------------------------------- |
| [leiwand rv32](https://github.com/franzflasch/leiwand_rv32)  | Verilog       | 教育类项目 5499/ 7680 仅使用 iCE40hx8                        | [GPL-3.0](https://opensource.org/licenses/GPL-3.0)           |
| [catzip](https://github.com/develone/catzip)                 | Verilog       | 小型 RISC CPU, [已经测试] 5710/ 7680    74%, iCE40hx8        | [GPL-3.0](https://www.gnu.org/licenses/gpl-3.0.en.html)      |
| [kamikaze](https://github.com/rgwan/kamikaze)          | Verilog | 精简四级流水线                       | [MIT](https://opensource.org/licenses/MIT)                   |
| [tinyriscv](https://github.com/liangkangnan/tinyriscv) | Verilog | 入门三级流水线                       | [Apache-2.0](http://www.apache.org/licenses)                 |
| [biriscv](https://github.com/ultraembedded/biriscv)    | Verilog | 超标量（双重发行）有序6或7级流水线。 | [Apache-2.0](http://www.apache.org/licenses)                 |
| [riscv](https://github.com/ultraembedded/riscv)        | Verilog | 32位RISC-V ISA CPU内核               | [BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause) |
| [dwarfRV32](https://github.com/Cloud-V/dwarfRV32)            | Verilog       | 计划待定, 未适配                                             | [GPL-3.0](https://opensource.org/licenses/GPL-3.0)           |



#### 如发现统计错误, 欢迎通过提交 issues 指正.

