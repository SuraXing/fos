## 寄存器



#### AX,BX,CX, DX

- 数据寄存器

#### SI(source index)

- Source Index

#### DI(destionation index)

- Destination Index

#### SS(stack segment)

- 栈段寄存器.

#### SP(stack pointer)

- 栈偏移地址寄存器.永远指向栈顶

#### BP(**base pointer**)

- 栈的分界线,当发生call调用时,ebp寄存器将原值压入栈中并存入当前地址作为寄存器中的值.
- 此时ebp的上面（高位地址）为函数的返回值地址以及参数，下面则为临时的栈空间。
- 当call函数结束时，mov esp,ebp ,pop ebp : 恢复栈偏移量esp, 恢复分界线bp. 

#### CS(code segment)

- 指令段寄存器,CS中存储着CPU要执行的下一条指令的段地址

#### IP(instruction pointer)

- 指令指针寄存器.IP中存储着指令的偏移地址.
- 指令地址的计算方式为: CS * 16 + IP

#### DS(data segment)

- 数据段寄存器.DS中存放着要访问内存的段地址,通过寄存器赋值DS后,可以通过[X]作为偏移量访问数据段的内存.

#### ES(extra segment)

- 通过寄存器赋值

