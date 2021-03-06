汇编级机器组织
==============
##指令系统
计算机指令系统经历了从简单到复杂，再从复杂到简单的演变过程。
###CISC
复杂指令系统计算机(Complex Instruction Set Computer)  

主要特点：
* 指令格式多
* 寻址方式复杂
* 指令数量多
* 不同指令的使用频率相差很悬殊

###RISC
精简指令系统计算机(Reduced Instruction Set Computer)  

####特点:

1. 充分利用[VLSI](#vlsi)芯片的面积
   * CISC大多采用微程序控制，其控制存储器占用了CPU内大量面积
   * RISC采用组合程序控制，节约CPU空间
2. 提高计算机运算速度
   * RISC采用固定长度的指令格式，指令种类少（包括使用频率较高的简单指令以及很有用但不复杂的指令）
   * RISC大量使用寄存器，减少访存次数。提高指令的执行效率
   * RISC采用寄存器窗口重叠技术，又提高了执行速度
   * RISC采用组合逻辑控制，比CISC延迟小，缩短CPU周期
   * RISC采用的精简指令系统，适合流水工作，大多数指令在一个时钟周期内完成
3. 便于设计，可降低成本，提高可靠性
4. 有效支持高级语言程序

####简而化之
1. 指令条数少
2. 指令长度固定，指令格式和寻址种类少
3. 只有取数/存数指令访问存储器，其余指令的操作均在寄存器之间进行

>不过尽管有上述优点，但RISC绝不会完全取代CISC结构。

###指令系统的性能要求
* 指令系统的完备性
* 指令系统的有效性
* 指令系统的规整性
* 指令系统的兼容性

###指令操作的种类
- 数据传输类指令（MOV）
- 算数运算类指令
- 逻辑运算类指令
- 程序控制类指令（流程控制）
- 输入/输出类指令（IO）
- 特权指令
- 处理器控制指令

##指令格式
指令结构由两部分组成：
- 操作码
- 地址码

###地址码
根据地址码个数的不同，分为三地址指令、二地址指令、一地址指令和零地址指令
####二地址指令
*二地址指令最常见*  
依据操作数的物理位置来说，可以归结为三种类型：

|类型|全称|
|----|-----|
|SS|存储器--存储器型指令|
|RR|寄存器--寄存器型指令|
|RS|寄存器--存储器型指令|


-------------
###VLSI
超大规模集成电路
