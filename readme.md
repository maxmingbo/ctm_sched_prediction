
调度系统进度预测内部比赛,第二名获奖方案；
![image](https://github.com/maxmingbo/ctm_sched_prediction/blob/master/8submit/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20190114201639.jpg)
比赛预测多天整个数据仓库20多万/天个跑批作业完成时间的比赛。


队伍：DataCode的解决方案

代码贡献者:Zmax


__环境：__

windows下：

python3.6

pandas 0.21.0

scikit-learn 0.19.0

xgboost 0.6+20171121

lightgbm



__程序文件:(数字序号编就是程序运行的大致顺序）__

CTM:
    
    1data_analysis
    
    2data_split  ---产生数据文件data_src
    
    3processing  ---data_processed
    
    4union     ---data_train
    
    5model
    
    6feature_importance
    
    7blending
    
    8submit   ---data_submit
    

  文件夹代码具体作业：
    
    1data_analysis：简单的数据查看，数据分析
    2data_split  ：把数据按图实例化日期分割成单独的文件
    3processing  ：每个表进行特征加工处理
    4union     : 把每个表的特征连接起来成一个大表
    5model     : 各种预测算法
    6feature_importance :计算特征重要性及简单的模型调优
    7blending    :    模型融合
    8submit     :    产生最终的提交结果

__数据结果文件：（按数据文件产生顺序）__

CTM:
    
    data_src        --存放按天(order_day)的最原始数据
    data_processed    ---存放初步加工的数据特征
    data_train      --- 存放给模型训练的数据
    result_submit    --- 提交的最终结果




