# CNNItemRec-MATLAB
使用修改后的VggNet和ResNet网络进行训练并进行分类评测
使用软件：MATLAB R2019b、PyCharm 2019.3.3 x64

其中binConvert文件夹为将二进制形式数据文件转化为图片形式的代码，因为已经下载好数据集，所以注释掉了代码中下载数据集的部分，如果未下载，可以取消掉这部分的注释进行数据集的下载。将下载好的stl10_binary文件夹粘贴进去，运行代码，会生成一个img文件夹，里面包含10个文件夹，分别为10个类，每个类中包含500张训练图片。删除生成的img文件夹
改变代码的34-38行：
# path to the binary train file with image data
DATA_PATH = './stl10_binary/test_X.bin'
# path to the binary train file with labels
LABEL_PATH = './stl10_binary/test_y.bin'
再次运行，会生成一个img文件夹，里面包含10个文件夹，分别为10个类，每个类中包含500张测试图片，手动将生成的测试集和训练集的各个文件夹改为类名字。

其中CNNItemTest为该项目，里面已经包括了处理好的数据集，不需要做数据集类型的转换。
运行方法：
1.打开MATLAB R2019b
2.在MATLAB的命令行窗口输入cd('此项目的路径')
3.在MATLAB的命令行窗口输入guide，并选择MainForm.fig，打开设计界面后点运行按钮。





