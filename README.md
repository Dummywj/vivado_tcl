# vivado_tcl

A tcl script file that loads vivado project quickly just from neccessary source files.

Introduction in Chinese: https://zhuanlan.zhihu.com/p/12662221710 

## Usage

Create your working directory like this.

![img](https://pic2.zhimg.com/v2-ca29a59b5c20c1930b2e7745fa04122d_1440w.jpg)

Modify tcl script to fit your project.

```tcl
# Set the project name
set _xil_proj_name_ "led_test"

# Set FPGA part
set fpga_part "xcvu13p-fhgb2104-2-i"

set vivado_version "2020"

# Set Top Module
set top_module "led"
set tb_top_module "tb_led"
```

Then open vivado, and open TCL Console. First change your directory to this working directory; then run this tcl script.

```tcl
cd C:/xxx/xxx/project
source build.tcl
```

