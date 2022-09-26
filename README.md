人岗匹配代码
====
本模型先将人员信息进行embedding， 然后利用cnn+capsule+bigru的网络进行训练及预测，模型最高成绩为0.271.
语言 python

环境 keras==2.3.1， tensorflow==1.15.2

data_process.py是读取json文件，并且连接文本，产生模型新的训练集测试集。
word2vec_200.py是训练200维embedding向量的代码
bilstm_cnn是模型训练及预测的代码

注意：文件夹中的新的训练集已经准备好，同时为了减少测试时间，模型已经训练好，模型文件放在./code/model/中，同时对bilstm_cnn中训练代码进行了注释，直接运行bilstm_cnn.py可以直接利用训练好的模型得到预测结果（完整训练大概需要7个小时左右）。
