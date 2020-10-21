################################################################################

1. How to Build
    - get Toolchain
        From android git server, codesourcery and etc ..
         - arm-eabi-4.9

    - make output folder
        EX)OUTPUT_DIR=out
        $ mkdir out

    - edit Makefile
        edit "CROSS_COMPILE" to right toolchain path(You downloaded).
          EX)  CROSS_COMPILE= $(android platform directory you download)/android/prebuilt/linux-x86/gcc/linux-x86/arm/arm-eabi-4.9/bin/arm-eabi-
          Ex)  CROSS_COMPILE=/usr/local/toolchain/arm-eabi-4.9/bin/arm-eabi-          // check the location of toolchain

2.Build command
        ./build_kernel.sh

3. Output files
    - Kernel : out/arch/arm/boot/Image
    - module : out/drivers/*/*.ko

4. How to Clean    
        Change to OUTPUT_DIR folder
        EX) $(pwd)/out
        $ make clean

##################################################################################
