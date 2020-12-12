命令		命令解释
----------------
;		注释符 用于注释代码
DB		define byte 写入1个字节的指令,小写可以db. 如果写入字符串，则会自动转换为字符串对应的编码
RESB	reserve byte 预约字节，RESB 10 预约10个字节，并填充为0x00
DW		define word 写入2个字节(16bit)
DD 		ddefine double-word 写入4个字节