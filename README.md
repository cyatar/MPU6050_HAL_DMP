# MPU6050_HAL_DMP
在标准库的基础上做了移植。

使用MPU6050，启用DMP计算四元数，并最终输出YAW，PITCH，ROLL。

添加了温度漂移的修正。

例程在STM32F103RCT6上运行，使用I2c2。

使用I2c1的话需要修改位于MPU6050.c中的i2cWrite和i2cRead函数。
