# 常见命令
ls: 列出当前目录下的文件和文件夹。
history: 查看命令历史记录。
useradd: 创建新用户。
chmod: 修改文件权限。
Ctrl + C: 中断当前正在执行的命令。
Ctrl + L/clear: 清屏。
cd: 切换工作目录。
mkdir：创建新目录。
rm：删除文件或目录。
cp：复制文件或目录。
mv：移动或重命名文件或目录。
hostname：显示主机名
uname：显示系统信息。
df：显示磁盘使用情况。
top：实时监控系统资源使用情况。
cat：显示文件内容。
grep：在文件中查找指定的字符串。
sed：流编辑器，用于文本替换和处理。
awk：强大的文本处理工具，可用于数据提取和分析。
# 自定义配置
个性化设置：可以通过修改终端的配置文件来实现个性化设置，如更改字体、颜色方案、提示符样式等。以 GNOME Terminal 为例，可以在其设置中选择不同的主题和字体。
环境变量配置：环境变量用于定义系统的运行环境，用户可以通过修改 ~/.bashrc 或 ~/.bash_profile 文件来配置自己的环境变量。例如，设置 PATH 环境变量，将自定义的脚本目录添加到系统的可执行路径中。

# 硬件信息
在Ubuntu系统里，可借助多种命令查看硬件信息，下面是一些常用命令：

1. CPU信息
lscpu：此命令能展示CPU的详细信息，像架构、核心数、线程数、频率等。
lscpu
cat /proc/cpuinfo：读取/proc/cpuinfo文件来获取CPU信息。
cat /proc/cpuinfo
2. 内存信息
free -h：以人类可读的格式显示系统的内存使用情况，涵盖总内存、已用内存、空闲内存等。
free -h
cat /proc/meminfo：读取/proc/meminfo文件以获取更详尽的内存信息。
cat /proc/meminfo
3. 硬盘信息
lsblk：列出所有可用块设备的信息，包含硬盘、分区等。
lsblk
df -h：以人类可读的格式显示磁盘使用情况，包括每个挂载点的总容量、已用容量、可用容量等。
df -h
sudo fdisk -l：显示硬盘的分区表信息，要使用sudo获取足够权限。
sudo fdisk -l
4. 显卡信息
lspci | grep VGA：通过lspci命令列出所有PCI设备，再用grep过滤出显卡信息。
lspci | grep VGA
lshw -C display：显示详细的显卡硬件信息，需使用sudo获取足够权限。
sudo lshw -C display
5. 系统信息
uname -a：显示系统的内核信息、主机名、发行版本等。
uname -a
lsb_release -a：显示Ubuntu的发行版本信息。
lsb_release -a
你可以在终端里输入这些命令来查看相应的硬件信息。
