# Tensorflow Wheels

Tensorflow wheels built for **AMD Phenom(tm) II X6 1045T Processor** CPUs or equivalent instruction sets:

fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush mmx fxsr sse sse2 ht syscall nx mmxext fxsr_opt pdpe1gb rdtscp lm 3dnowext 3dnow constant_tsc rep_good nopl nonstop_tsc cpuid extd_apicid aperfmperf pni monitor cx16 popcnt lahf_lm cmp_legacy svm extapic cr8_legacy abm sse4a misalignsse 3dnowprefetch osvw ibs skinit wdt cpb hw_pstate vmmcall npt lbrv svm_lock nrip_save pausefilter

NVIDIA Driver 418.87.00 

| TF | HW |Python | CUDA | cuDNN | Support | OS | Download |
|:------:|:------:|:------:|:----:|:-------:|:-----:|:------------:|:------:|
| 2.0 |GPU|   3.7  |10.1| 7.6 | w/out AVX,AVX2 | Ubuntu 18.04 x86_64 |[**Download**](https://app.box.com/s/p571878q6hvgnkcwau6lbce9sdvsejr0)|
| 1.15 |GPU|   3.7  |10.1| 7.6 | w/out AVX,AVX2 | Ubuntu 18.04 x86_64 |[**Download**](https://app.box.com/s/spuank3te8y19uffoi7jk7y0jyvk75pm)|


$ sudo bazel build -c opt --config=cuda --copt=-mno-avx --copt=-mno-avx2 --local_ram_resources=12288 --local_cpu_resources=5 --local_cpu_resources=5 //tensorflow/tools/pip_package:build_pip_package

## Install the package
$ pip install tensorflow-1.15.0-cp37-cp37m-linux_x86_64.whl

  or
  
$ pip install tensorflow-2.0.0-cp37-cp37m-linux_x86_64.whl
