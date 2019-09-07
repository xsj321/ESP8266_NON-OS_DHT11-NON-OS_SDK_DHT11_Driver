# ESP8266_NON-OS_SDK_DHT11_Driver
# ESP8266_NON-OS_SDK_DHT11_驱动库
> 实现在以ESP8266_NON-OS_SDK为基础的ESP8266开发中快速读取DHT11温湿度传感器的功能:

*使用方法*：

1. 建立工程；
2. 将dht11.h文件复制到 工程目录\app\include\driver
3. 将dht11.c文件复制到 工程目录\app\driver
4. 在项目文件中应用dht11.h


----------


*主要函数*：

**DHT11_Read_Data**

**函数原型：**

    ICACHE_FLASH_ATTR uchar DHT11_Read_Data(DHT11_Data *Data,int PIN_NAME,int PIN);
> 简介：读取DHT11的数据，改变传入指针指向的Data结构体中的Humi与Temp
> 
> 参数1 Data： 储存数据的结构体
> 
> 参数2 PIN_NAME： 引脚地址 如：PERIPHS_IO_MUX_GPIO5_U
> 
> 参数3 PIN: 引脚号
> 
> 返回值: uchar(unsigned char)返回读取是否成功
> 
> 0：成功
> 
> 1：失败

