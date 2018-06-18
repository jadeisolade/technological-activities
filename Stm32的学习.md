GPIO_WriteBit    对某一个IO管脚输出高低电平  
GPIO_Write对某一位、端口输出高低电平（比如F位，有八个引脚）  
一般Bit代表某一个管脚，无则代表一个端口。
管教输出速度最大100M。  
首先要定义各种类型的结构体变量。  
初始化结构体是指针型的，所以注意加地址（&GPIO_InitStructure  和C语言结构体类型指针结合起来）  
可以一次对多个管脚进行初始化，前提必须是它们的配置模式需一样。比如： GPIO_InitStructure.GPIO_Pin=GPIO_Pin_9|GPIO_Pin_10; 利用或运算。  



