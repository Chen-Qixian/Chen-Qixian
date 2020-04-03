## 拓扑映射算法实现

### 北京航空航天大学 陈麒先

#### 概述

利用拓扑映射算法进行通信性能优化的主要原理是将存在大量数据通信的进程划分至相同进程组，进而将其布置在数据传输能力强的计算节点中。因此，并行应用的通信局部性特征成为了拓扑映射优化的重要考虑因素。本仓库选取LPMS、QTLS、MPIPP、TreeMatch、APHiD 以及TopoMapping这六种表现优异的典型算法进行深入研究，依据其原理编程实现了这些算法。

#### 说明

- LPMS、QTLS、APHiD 以及TopoMapping算法均由本人采用C++编程实现，运行之前，请修改file-io.h文件中输入文件路径（注意是绝对路径）。编译并运行main.cpp并在output中查看运行结果。

- MPIPP、TreeMatch为论文原作者开源实现。执行以下命令即可得到运行结果。注意需要Hwloc环境依赖。

  ```bash
  $ ./configure
  $ make install
  $ make
  ```

  

