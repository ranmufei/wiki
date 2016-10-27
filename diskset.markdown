# 再生龙制作的镜像 复制到 大硬盘后 扩容目标盘

>  再生龙 制作的系统 拷贝大于自己的硬盘上后 并不会自动扩容磁盘空间，这样就浪费了大容量硬盘空间。故必须手动的对大容量硬盘剩余的空间 进行分区 加载进系统中来。



#### 需要两个工具

- GParted  linux 系统分区工具 （http://heanet.dl.sourceforge.net/project/gparted/gparted-live-stable/0.26.1-5/gparted-live-0.26.1-5-i686.iso）

- 吧 GParted 烧录到U盘 启动工具  `LinuxLive USB Creator 2.9.4.exe` (http://download.tuxfamily.org/lilicreator/stable/LinuxLive%20USB%20Creator%202.9.4.exe)

- 以及 一个U盘


>>  通过 LinuxLive USB Creator 吧下载的 gparted 烧录到 u 盘 即可  。。  待吧系统拷贝成功后  ，关机 使用U盘启动 GParted 进行操作即可。。 有图形界面 ！