# 1.交易量
# 2.price

价格在周期内的低点， 周期：1天，1周，1月。


2.《寻找买入点》功能
      日内买入会找布林带在日内可以找到最大颗粒度的布林带下轨， 底部结构，底部放量等位置，macd等等 这个日内位置应该要更具更大的结构的动能预测
      同样的趋势 可以以macd 量 看涨图形结构找买入点

# 3.pattern：

      bullish_list = ['bullish_flag','double_bottom','inverse_head_shoulders','bullish_pennant','triple_bottom','falling_wedge']
      not_sure_list = ['triangle', 'rectangle']


# 4.指标：
### 4.1 MACD

      在结合交易量数据和MACD指标寻找TSLA股票的买入点时，我们可以通过以下方式分析：

      1. 交易量和MACD的信号分析
### MACD金叉信号：当MACD线（快线）向上穿越Signal线（慢线）时，通常表示买入信号。这一信号表示短期趋势强于长期趋势，可能预示价格上涨。
      放量确认：仅靠MACD金叉可能产生误导，因此需要结合交易量进行确认。如果在MACD金叉的同时，交易量出现明显放大，且买入量大于卖出量，说明多方力量较强，有可能支撑价格进一步上涨。
      2. 判断买入量和卖出量的变化
      买入量大于卖出量：当买入量显著高于卖出量时，表明市场上买方力量更强，价格有可能被进一步推高。
      交易量持续增加：如果MACD金叉出现后的几分钟内，买入量持续增加，显示出多头势力的不断加强，这种情况下MACD信号可信度较高，是适合的买入时机。
      3. 实施策略
      结合上述信号的综合考虑，在一天的交易中找出买入点可以分为以下步骤：

      确认MACD金叉：观察MACD线是否有效向上穿越Signal线，这是初步的买入信号。
      观察放量情况：金叉后确认是否有较大的成交量，尤其是买入量高于卖出量。此时，放量增大则说明市场对价格上涨有较高的认可度。
      确认背离情况：若MACD和价格走势出现背离（如价格回调但MACD在上升），可以认为这是多方蓄力的信号，往往会出现短期上涨机会。
      实例分析：
      假设我们在某个时间段看到以下情况：

      时间点1：MACD线接近Signal线，形成金叉的趋势。
      时间点2：金叉形成，且交易量开始放大，买入量大于卖出量，MACD的柱状图开始转为正值。
      时间点3：金叉后5分钟内，交易量继续增加，且价格向上突破。
      在时间点2-3之间，买入信号已经基本确认，这是较为合适的买入点。此时MACD和放量的结合说明多头情绪高涨，买入后短期内的上涨概率较高。

      风险控制
      即便MACD和交易量结合形成了买入信号，也应保持谨慎。可以设定止损点，以防市场突发因素导致信号失效。

### 4.2.MACD

  ![image](https://github.com/user-attachments/assets/b332c0d3-d712-469f-aed8-79a681aaaf40) 
  ![image](https://github.com/user-attachments/assets/8e22244d-d276-4919-9d04-cd632c1f7b37)
  ![image](https://github.com/user-attachments/assets/04f3c33e-af3c-4096-8a4f-efd29e84cc25)
  ![image](https://github.com/user-attachments/assets/9547d458-22cf-4fe9-815c-40adff6710e7)
      
      双线MACD（26,12,9）:
      T越近的、price越接近的 影响越大EMA（Exponential Moving Average），比MA变动迅速。
      快线DIF = 12EMA - 26EMA （两根均线差离值，差离值越大，说明价格上涨速度越快）
            DIF（T-1） < 0 ，DIF （T） > 0 （12EMA上穿26EMA，快线DIF上穿零轴,处于多头趋势）

            DIF（T-1） > 0 ，DIF （T） < 0 （快线DIF下穿零轴,处于空头趋势）

            
      慢线DEA = 9EMA(DIF) （以周期9计算 DIF 的EMA）
      能量柱 = n*(快线DIF-慢线DEA)  （n=1,2.  1倍或2倍的快线与慢线之间的差离值）

      金叉：快线DIF上穿慢线DEA： (T-1) 快线DIF < 慢线DEA, (T) 快线DIF > 慢线DEA (出现多头信号)
      
      死叉：快线DIF下穿慢线DEA： (T-1) 快线DIF > 慢线DEA, (T) 快线DIF < 慢线DEA (出现空头信号)

   ![image](https://github.com/user-attachments/assets/904e2ee1-bf26-44ce-9d80-8ee5717627b0)
   ![image](https://github.com/user-attachments/assets/427eedd9-5a30-4596-82ad-ae961b45ff4d)

  
背离：
      某支股票价格上涨速度变慢，快线DIF （= 12EMA - 26EMA） 【两根均线差离值，差离值越小，说明价格上涨速度越慢】由大变小。


      单线MACD(26,12,1):
      快线DIF = 12EMA - 26EMA （两根均线差离值）
      
#### 4.3 KDJ

      在结合交易量数据和KDJ指标寻找TSLA股票的买入点时，我们可以通过以下策略分析来判断适合的买入时机：

      1. KDJ的金叉信号与超卖状态
      KDJ金叉：当K线向上穿过D线时，通常被视为买入信号，说明短期内买方力量开始增强，股价可能迎来反弹。
      超卖区域：K、D、J值在20以下，尤其是J值接近0时，通常代表股票处于超卖状态，市场可能有回升的潜力。
      2. 交易量的支持
      买入量大于卖出量：在KDJ出现金叉的同时，如果买入量显著高于卖出量，说明市场上买方力量充足，资金持续流入可能推动股价上涨。
      放量信号：在KDJ金叉的同时，若交易量也有所放大（尤其是买入量增加），意味着市场对于短期反弹的认可程度较高，金叉信号的可信度增加。
      3. 实施策略
      在一天的交易中，我们可以按以下步骤寻找合适的买入点：

      观察超卖状态：首先观察KDJ指标是否处于超卖状态（K、D、J在20以下），并密切关注是否即将形成金叉。这表明股价可能处于相对低位，有反弹潜力。

      等待KDJ金叉形成：当K线向上穿过D线形成金叉时，表明买入信号已经初步确认。

      确认交易量增加：在KDJ金叉形成的同时，确认买入量是否显著大于卖出量，或者交易量是否有明显的放大迹象。若有，则说明市场的短期反弹可能具备足够的资金支撑。

      实例分析：
      假设在某个时间段内观察到以下情况：

      时间点1：K、D、J值都在20以下，处于超卖状态。K线开始接近D线，有金叉迹象。
      时间点2：K线成功向上穿过D线，形成金叉，同时买入量显著高于卖出量，显示多头力量开始增强。
      时间点3：金叉后，成交量继续放大，尤其是买入量的持续增加，股价随之上行。
      在时间点2-3之间，买入信号已得到确认，这是较为合适的买入点。此时不仅有KDJ的金叉信号，还得到了交易量的支撑，表明多头势力进一步增强。

### 4.3. Stochastic/KDJ Indicator 

![image](https://github.com/user-attachments/assets/c228e410-a5b6-49b4-9569-1ca071ebc6c2)
![image](https://github.com/user-attachments/assets/4f291509-3b3f-4f90-8e83-3f982148083f)
![image](https://github.com/user-attachments/assets/21904e63-1e97-4933-ab65-56cdc4dd019d)
![image](https://github.com/user-attachments/assets/3b612c01-7a3b-4616-bdeb-b2f93eaba1bd)
      
            快线DIF
            慢线DEA
            20轴
            80轴
            KD参数（9，3，3）
            
            RSV = (close_price[T] - lowest_price[T-8, T])*100/(highest_price[T-8, T] - lowest_price[T-8, T])  
                   [当前收盘价格距离最低价格的上涨幅度，涨幅] / [最高值与最低值之间的差值，振幅]
                   if 当前收盘价格==最高价， 涨幅==振幅， RSV = 1*100/1 = 100；
                   if 当前收盘价格==最低价， 涨幅==0， RSV = 0
      
                   金叉：上穿20轴（多头信号）
                   死叉：下穿80轴（空头信号）
                   
            K = (2/3)*(lastday_K[T-1]) + (1/3)*(todat_RSV[T])  [RSV的加权移动平均]
            
            D = (2/3)*(lastday_D[T-1]) + (1/3)*(todat_K[T])   [K的加权移动平均]
      
      特点：变化快，灵敏
      ![image](https://github.com/user-attachments/assets/df51016a-37f0-4665-b880-283b11be6a37)
      
      MACD趋势+KD信号：
            MACD能量柱-->是否处于多头趋势【DIF（T-1） < 0 ，DIF （T） > 0 （12EMA上穿26EMA，快线DIF上穿零轴,处于多头趋势）】
            KD金叉：上穿20轴（多头信号，入场信号）


### 4.4.BOLL

![image](https://github.com/user-attachments/assets/7803de24-d1fa-4929-b2d1-8164de9f6ecb)
![image](https://github.com/user-attachments/assets/98ee1a17-a8a8-4d77-bf4e-f762d9c88eb3)

      Bollinger Bands 布林带：上轨、中轨、下轨， 参数：20.
      [中轨] MA = sum(close_price [T-19, T] )/20  [20天收盘价求和/20]
      MD:
          方差 = sum((close_price[T-19, T] - MA)**2) / 20
          标准差MD = 平方根方差  [收盘价的离散程度]
          
      中轨 = MA
      上轨 = MA + 2MD
      下轨 = MA - 2MD

![image](https://github.com/user-attachments/assets/8c02ffbe-8d5c-4659-bd04-6746bcad4080)
![image](https://github.com/user-attachments/assets/033fe74e-1cab-45b4-b92f-f70218040735)
      
      BOLL 开口的判断：向上开口--> 多头信号，入场信号。
      BOLL 开口的判断：向下开口--> 空头信号，出场信号。
      超买：price(T-1) > 上轨，price(T) < 上轨（再回到布林带）。 ----> 做空信号。
      超卖：price(T-1) < 下轨，price(T) > 下轨（再回到布林带）。 ----> 做多信号。

      价格 ---决定--> BOLL -----不能决定---> 价格


      正态分布：对自然数据统计中有正态分布的特点。




# 5.SMA(simple moving average) 

![image](https://github.com/user-attachments/assets/63f21291-908d-4421-82aa-14e64428cf9e)
![image](https://github.com/user-attachments/assets/934ea5ca-9cb2-4444-b282-a9f32ead6c2f)
      
      金叉：price(T-1) < SMA，price(T0) > SMA 
       对于单根(均值)SMA：当价格上穿SMA，形成金叉（多头信号）。

      多个均线：
      金叉：周期小的SMA，上穿周期大的SMA，形成金叉（多头信号）。
       
       特点：直观、滞后
       challenge：不同参数的SMA 会有不同的特点，短线慢线的时间周期越大，金叉死叉的信号会更滞后（更晚），但会更稳定。
             对于不同的“标的”和不同的“趋势”，不同周期的MA会有不同的作用。
             时间周期较大的SMA，在长周期大幅度上涨的 标的/趋势 中，金叉买入死叉卖出，会获得更多利润。


# 4.5.RSI（Relative Strength Index）及其相关指标 RSI-based Moving Average (MA) 的详细解释：

1. RSI（相对强弱指数）
      RSI 是一种振荡类技术指标，用于衡量价格变动的速度和幅度，以帮助识别股票是否处于超买或超卖状态。RSI 通过一段时间（通常为 14 个周期）的价格涨跌来计算，并将结果标准化到 0 到 100 之间。它通常用于判断市场趋势和逆转的可能性。
      
      
      RSI 的基本公式是：
      RSI = 100 − 100/(1 + 平均上涨幅度/平均下跌幅度)
      
      其中：
      平均上涨幅度 是在选定周期（例如 14 天）内所有价格上涨的平均值。
      平均下跌幅度 是在同一周期内所有价格下跌的平均值。
      RSI 的值一般解读为：
      
      RSI > 70：表明股票处于超买状态，可能有回调压力。
      RSI < 30：表明股票处于超卖状态，可能存在反弹潜力。
      在实际操作中，当 RSI 从低于 30 回升到 30 以上时，可以视为买入信号；当 RSI 从高于 70 回落到 70 以下时，可以视为卖出信号。

      RSI 的作用
      超买/超卖信号：帮助量化交易员识别市场的极端状态，判断趋势是否可能逆转。
      趋势强弱判断：RSI 还可用作趋势强弱的衡量工具，例如在 50 水平之上时代表趋势偏强，反之亦然。
   
3. RSI-based Moving Average (RSI-based MA)
   
      RSI-based Moving Average 是基于 RSI 的移动平均值，进一步平滑 RSI 指标，以减少短期波动的影响，使信号更加稳定。通过在 RSI 的基础上添加移动平均线，交易员可以更好地识别 RSI 指标的趋势和关键点位。
      
      RSI-based MA 的实现方式
      RSI-based MA 的常见方法是计算 RSI 的简单移动平均线（SMA）或指数移动平均线（EMA），以便减少 RSI 的噪音：
      
      RSI-based MA=SMA(RSI,period)或EMA(RSI,period)
      其中：
      SMA 是 RSI 的简单移动平均值。
      EMA 是 RSI 的指数移动平均值，通常对最新的 RSI 值给予更高的权重。
      RSI-based MA 的用途
      趋势确认：RSI-based MA 可以帮助确认 RSI 的走势。例如，当 RSI 维持在其移动平均线上方时，表示多头强势；当 RSI 在其移动平均线下方时，表示空头强势。
      平滑信号：相比于原始的 RSI 值，RSI-based MA 平滑了短期波动，可以有效过滤掉一些假信号，让量化交易员更专注于长期趋势。
      信号交叉：一些量化策略会使用 RSI 和 RSI-based MA 的交叉作为交易信号。当 RSI 上穿 RSI-based MA 时，这是一个潜在的买入信号；反之，当 RSI 下穿 RSI-based MA 时，这是一个潜在的卖出信号。
      RSI 和 RSI-based MA 在量化交易中的应用
      在量化交易中，RSI 和 RSI-based MA 通常用来生成买卖信号、预测市场逆转，甚至配合其他指标来制定更加复杂的交易策略。例如：
      
      超买超卖策略：当 RSI > 70 时进入空头，当 RSI < 30 时进入多头，结合 RSI-based MA 可以进一步确认信号。
      
      趋势反转策略：当 RSI 从低于 30 上升到 30 以上并且 RSI 突破 RSI-based MA 时，买入信号更为可靠；反之亦然。
      
      双重滤波策略：通过 RSI 和 RSI-based MA 之间的交叉过滤信号，避免在波动较大的市场中因短期假信号而频繁交易。

总结
      RSI 提供了价格变动的强弱信息，是判断超买和超卖的重要工具。
      RSI-based MA 则是平滑 RSI 的波动，过滤噪声，帮助确认 RSI 的信号。
      结合 RSI 和 RSI-based MA，量化交易员能够更好地捕捉趋势，识别市场极端情况，从而优化交易策略。

例子：下图为RSI【紫色线条】和 RSI-based MA【黄色线条】的例子，RSI-based MA上穿30轴会有明显的滞后。

![image](https://github.com/user-attachments/assets/eb8af994-aec1-46f6-9094-e64593108c27)

下图中有两个波动的RSI上穿30线的例子，可发现最后一个RSI上穿30线时为最佳买入点。(大鱼被动晕眩，1/3，2/，33/3)

![image](https://github.com/user-attachments/assets/986d1136-5977-4dcd-b311-ae26416c348b)


### 4.6 On Balance Volume OBV

      if price_close(T) > price_close(T-1):
            OBV(T) = OBV(T-1) + volume(T)
      if price_close(T) < price_close(T-1):
            OBV(T) = OBV(T-1) -volume(T)
      else: #price_close(T)=price_close(T-1)
            OBV(T) = OBV(T-1)

      
      股价上涨，OBV增加，股价下跌，OBV下跌

![image](https://github.com/user-attachments/assets/3e808eb0-8ca3-48b3-b684-7969aac86811)

      OBV金叉
      买入信号：OBV(T-1) < MA(T-1), OBV(T) >= MA(T)
            或：OBV(T-1) < EMA(T-1), OBV(T) >= EMA(T)
            或：OBV(T-1) < SMA(T-1), OBV(T) >= SMA(T)
![image](https://github.com/user-attachments/assets/988865f2-c846-4d81-8365-d4fe2a7be159)

      OBV死叉
      卖出信号：OBV(T-1) > MA(T-1), OBV(T) <= MA(T)
            或：OBV(T-1) > EMA(T-1), OBV(T) <= EMA(T)
            或：OBV(T-1) > SMA(T-1), OBV(T) <= SMA(T)
![image](https://github.com/user-attachments/assets/de937900-bebf-4200-949a-9729382add04)

      短时间内反复交叉，不需要操作。
![image](https://github.com/user-attachments/assets/c040304c-f776-4451-8584-259906e63dd7)

      缺点：信号有延迟

（背离信号1）购买力的信号：股价上涨（或者跌完再涨），OBV上涨幅度不高；或者股价创新高，OBV没有继续增加（没之前点高）。预示着股价上涨力量不足（可能会快速暴跌）。

![image](https://github.com/user-attachments/assets/335a2ad1-374e-4703-9a25-29e9aa0f1440)
![image](https://github.com/user-attachments/assets/befa08e9-dbd7-4ae5-8501-8ac121880345)

（背离信号2）购买力的信号：股价持续下降，OBV不下降，说明在底部蓄力；预示未来会上涨。
![image](https://github.com/user-attachments/assets/21532a47-7779-4da1-a649-44ffad72b1a1)
![image](https://github.com/user-attachments/assets/85338df7-2ac5-45da-9723-976b8cc31b89)

![image](https://github.com/user-attachments/assets/abc3b07d-b608-4748-b33f-c35fd3d56c3d)
![image](https://github.com/user-attachments/assets/e1dc92b7-2a74-4d24-bbf6-b774f6877f45)

      
# 11.candle

      锤⼦线（Hammer）和倒锤⼦线（Inverted Hammer）
      蜻蜓⼗字星（Dragonfly Doji）
      看涨吞噬(Bullish Engulfing)
      启明星（Morning Star）
      启明⼗字星（Morning Doji Star）
      ⽩三兵（Three White Soldiers）
