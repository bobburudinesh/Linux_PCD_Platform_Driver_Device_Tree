# Linux_PCD_Platform_Driver_Device_Tree
Implemented char driver for platform devices that are added from device tree. 

Added am335x-boneblack-lddcourse.dtsi at /arch/arm/boot/dts/ and included this file in master dts file(am335x-boneblack.dtsi) and compiled and generated new DTB. and used this dtb to during booting.

Note for proper functioning follow below steps:
1. Add am335x-boneblack-lddcourse.dtsi at /arch/arm/boot/dts/ 
2. Include am335x-boneblack-lddcourse.dtsi in am335x-boneblack.dts
3. generate DTB(device tree binary) using below command.
make ARCH=arm CROSS_COMPILE=arm-linux-gnueabhif- am335x-boneblack.dtb
