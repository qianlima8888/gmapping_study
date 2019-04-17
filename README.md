# gmapping_study
根据个人理解对gmapping代码添加注释

addscan函数为处理激光雷达数据的函数
该函数主要是调用了gridslamprocessor.cpp文件中的processScan()函数

processScan()函数会调用gridslamprocessor.hxx文件中的scanMatch()函数

scanMatch()函数会调用scanmatcher.cpp文件中的optimize()函数

optimize()函数即是对粒子的位姿进行前后左右和左转右转微调 并算出score最大的那个最为优化值

地图更新也是利用分数最大的粒子的地图
