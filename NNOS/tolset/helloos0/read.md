命令		命令解释
----------------
;		注释符 用于注释代码
DB		define byte 写入1个字节的指令,小写可以db. 如果写入字符串，则会自动转换为字符串对应的编码
RESB	reserve byte 预约字节，RESB 10 预约10个字节，并填充为0x00
DW		define word 写入2个字节(16bit)
DD 		ddefine double-word 写入4个字节
ORG		origin	将机器语言指令装载到内存中的哪个地址，如 ORG 0x7c00
MOV		move 对寄存器进行赋值操作
INT		interrupt 中断操作，类比一个函数，后续再补充
CMP		compare	比较
JMP		jump 程序跳转到某处
JE		jump if equal 如果等于则跳转
HLT		halt 停机指令，让CPU基本处于睡眠状态
OR		逻辑或

BIOS	basic input output system 基本输入输出系统
ROM		read only memory 只读内存



8个16位寄存器(2字节 共16字节)
AX——accumulator，累加寄存器		（AH AL）
CX——counter，计数寄存器 			 (CH CL)
DX——data，数据寄存器 				 (DH DL)
BX——base，基址寄存器 				 (BH BL)
SP——stack pointer，栈指针寄存器 
BP——base pointer，基址指针寄存器 
SI——source index，源变址寄存器 
DI——destination index，目的变址寄存器
（32位EAX, ECX, EDX, EBX, ESP, EBP, ESI, EDI）

8个8位寄存器
AL——累加寄存器低位（accumulator low） 
CL——计数寄存器低位（counter low） 
DL——数据寄存器低位（data low） 
BL——基址寄存器低位（base low） 
AH——累加寄存器高位（accumulator high） 
CH——计数寄存器高位（counter high） 
DH——数据寄存器高位（data high）
BH——基址寄存器高位（base high）

6个16位的段寄存器（2字节 共12字节）
ES——附加段寄存器（extra segment） 
CS——代码段寄存器（code segment） 
SS——栈段寄存器（stack segment）
DS——数据段寄存器（data segment） 
FS——没有名称（segment part 2） 
GS——没有名称（segment part 3）
