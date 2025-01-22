## 1月22日
1. 继续学习maxmul算子但是对于V5及后续版本不理解
   
## 1月16日
1. 完成vscode连接天数并记录wiki use_vscode.md
2. 编译测试第二节课的wiki并梳理代码记录到笔记中

## 1月14日
1. 根据说明登录天数服务器 测试运行cuda及python
2. fork hpc2torch_test仓库切换到对应分支并编译通过  但是测试均为0

python3 test/gather.py --device cuda
Testing Softmax on cuda with x_shape:(3, 2) , indice_shape:(2, 2), axis:0 ,dtype:torch.float32
2025-01-14 08:34:33,434 Pytorch: 0.025467690825462342 ms, kernel: 0 ms [-100.00%]
absolute error:9.8870e-01
relative error:9.8870e+07
Testing Softmax on cuda with x_shape:(3, 2) , indice_shape:(1, 2), axis:1 ,dtype:torch.float32
2025-01-14 08:34:33,436 Pytorch: 0.020673269033432008 ms, kernel: 0 ms [-100.00%]
absolute error:9.5076e-01
relative error:9.5076e+07
Testing Softmax on cuda with x_shape:(50257, 768) , indice_shape:(16, 1024), axis:0 ,dtype:torch.float32
2025-01-14 08:34:33,452 Pytorch: 0.34048075675964357 ms, kernel: 0 ms [-100.00%]
absolute error:1.0000e+00
relative error:1.0000e+08


