1. 功能说明
    此例程展示在 RT_Thread 系统创建 SPI 设备，并读、写、擦除操作 W25Q128

2. 使用环境
    硬件环境：工程对应的开发硬件平台 
    开发板：   N32G4FRH_STB V1.1 和 N32G457QEL_EVB V1.1

3. 使用说明
    描述相关模块配置方法；例如:时钟，I/O等 
         1. SystemClock：144MHz
         2. GPIO：LED(D1)--PA8
	        SPI1: NSS--PA4、SCK--PA5、MISO--PA6、MOSI--PA7
                        日志：TX--PA9  RX--PA10，波特率：115200

    描述Demo的测试步骤和现象 
         1. 编译后下载程序复位运行
         2. 本例程在main()里面创建两个线程，test0 线程和 test1 线程，test0 线程用于控制 D1 250ms闪烁，test1线程读、写、擦除操作W25Q128，测试结果通过串口打印

4. 注意事项
    将 N32G4FRH_STB V1.1 开发板上的 SPI1 接口接在 N32G457QEL_EVB V1.1 开发板的 W25Q128 上，两个开发板需要共地

1. Function description
    This routine shows how to create an SPI device on the RT_Thread system and read, write, and erase W25Q128

2. Use environment
    Hardware environment: development hardware platform corresponding to the project 
    Development board:      N32G4FRH_STB V1.1 and N32G457QEL_EVB V1.1

3. Instructions for use
    Describe the configuration method of related modules; for example: clock, I/O, etc. 
        1. SystemClock: 144MHz
        2. GPIO: LED(D1)--PA8
	     SPI1: NSS--PA4、SCK--PA5、MISO--PA6、MOSI--PA7
                     Log: TX--PA9 RX--PA10 Baud rate: 115200

    Describe the test steps and phenomena of Demo 
        1. After compiling, download the program to reset and run;
        2. This routine creates two threads in main(), test0 thread and test1 thread, test0 thread is used to control D1 250ms flashing, test1 thread read, write, erase operation W25Q128, test results printed through the serial port

4. Matters needing attention
    Connect SPI1 interface on N32G4FRH_STB V1.1 development board to W25Q128 of N32G457QEL_EVB V1.1 development board. The two development boards need to share the ground