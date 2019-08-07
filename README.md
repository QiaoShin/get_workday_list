# get_workday_list

扣除一年365天（时间区间可自定义）中的节假日和周日休息日，得到工作日列表dataset，方便计算工作日与工作日之间的工作时间差。



## 思路来源

  时间A: 2019-01-05 14:30:00 （周六）
  
  时间B: 2019-01-07 15:20:00 （周一）
  
  实际时间差： 时间B - 时间A = 2 天 0 小时 50 分钟 0 秒
  
  而计算工作时间内的时间差则是： 时间B - 时间A =  8 小时 50 分钟 0 秒
  
  这个时间的计算规则是：
  
                  1. 定义一天工作八小时，8:00-12:00 13:00-17:00
                  
                  2. 周一至周六属工作日
                  
                  3. 剔除非工作日时间（周日，节假日）
                  
           所以在这里剔除一月六号是周日后 时间B-时间A应该等于：1工作日0小时50分钟0秒  
           
           而1工作日=8小时
           
           所以有如上得出的时间差。
           
   
