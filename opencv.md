1. 加载、修改、保存图像
    * 加载图像(cv::imread)
    * 修改图象(cv::cvtColor)
    * 保存图像(cv::imwrite)


####Mat 矩阵中data、size等属性:

data : uchar类型的指针，指向Mat数据矩阵的首地址。
dims : Mat矩阵的维度，若Mat是一个二维矩阵，则dims=2，三维则dims=3
rows : Mat矩阵的行数。
cols : Mat矩阵的列数。
size() : size是一个结构体，定义了Mat矩阵内数据的分布形式，数值上有关系式：
         image.size().width=image.cols;        
         image.size().height=image.rows;
channels()：Mat矩阵元素拥有的通道数。
            例如常见的RGB彩色图像，channels=3；
            而灰度图像只有一个灰度分量信息,channels=1。