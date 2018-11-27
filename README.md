# -
kaggle单车项目分析以及预测
## 项目需求
本次项目需要结合天气数据下的使用模式来预测共享自行车的租赁需求
## 分析过程
### 1. 数据变量说明
datetime：日期<br>
season:季节<br>
holiday:是否是节假日<br>
workdingday:是否是工作日<br>
weather: 1. 清澈，少云，多云;2. 雾+阴天，雾+碎云;3. 小雪、小雨+雷暴+散云，小雨+云;4. 暴雨+冰雹+雷暴+雾，雪+雾<br>
temp:温度<br>
atemp:体感温度<br>
humidity:相对湿度<br>
winspeed:风速<br>
casual:临时租赁数量<br>
registered:会员租赁数量<br>
count:总租赁数量<br>
### 2.数据准备
`fig, axes = plt.subplots(2, 2)
fig.set_size_inches(12,10)

sns.distplot(bike_data['temp'],ax=axes[0,0])
sns.distplot(bike_data['atemp'],ax=axes[0,1])
sns.distplot(bike_data['humidity'],ax=axes[1,0])
sns.distplot(bike_data['windspeed'],ax=axes[1,1])

axes[0,0].set(xlabel='temp',title='Distribution of temp',)
axes[0,1].set(xlabel='atemp',title='Distribution of atemp')
axes[1,0].set(xlabel='humidity',title='Distribution of humidity')
axes[1,1].set(xlabel='windspeed',title='Distribution of windspeed')`
