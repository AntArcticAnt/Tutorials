# Ease of Movement（EMV）
* [Ease of Movement（EMV）](http://stockcharts.com/school/doku.php?id=chart_school:technical_indicators:ease_of_movement_emv)

## Introduction
* Developed by Richard Arms, Ease of Movement (EMV) is a volume-based oscillator that fluctuates above and below the zero line. As its name implies, it is designed to measure the “ease” of price movement. Arms created Equivolume charts to visually display price ranges and volume. Ease of Movement takes Equivolume to the next level by quantifying the price/volume relationship and showing the results as an oscillator. In general, prices are advancing with relative ease when the oscillator is in positive territory. Conversely, prices are declining with relative ease when the oscillator is in negative territory.

* 由理查德昂斯，EMV是一个以成交量为基础的振荡器，波动在零线以上和之下。顾名思义，它的设计是为了衡量价格变动的“舒适度”。昂斯创造了等量图表，以直观地显示价格范围和数量。通过量化价格/成交量的关系，并将结果显示为一个振荡器，易移动将等量提升到下一个水平。一般来说，当振子处于正向区域时，价格相对容易上涨。相反，当振荡器处于负区间时，价格相对容易下降。

## SharpCharts Calculation
* There are three parts to the EMV formula: distance moved, volume and the high-low range. First, the distance moved is calculated by comparing the current period's midpoint with the prior period's midpoint, which is the high plus the low divided by two. Distance moved is positive when the current midpoint is above the prior midpoint and negative when the current midpoint is below the prior midpoint. Distance moved is shown as the numerator in the formula below.

* EMV公式分为三个部分：距离移动、成交量和最高价-最低价范围.。首先，通过比较当前周期的中点和前期的中点，即最高价加最低价除以2，计算出移动距离。当当前中点高于前中点时，移动距离为正；当当前中点低于前中点时，移动距离为负。移动距离在下面的公式中显示为分子。

> Distance Moved = ((H + L)/2 - (Prior H + Prior L)/2)<br>Box Ratio = ((V/100,000,000)/(H - L))<br>1-Period EMV = ((H + L)/2 - (Prior H + Prior L)/2) / ((V/100,000,000)/(H - L))<br>14-Period Ease of Movement = 14-Period simple moving average of 1-period EMV<br>

* The other two parts form the Box ratio, which uses volume and the high-low range. Equivolume charts are based on volume and the high-low range as well. The Box ratio is the denominator of EMV. Note that volume is divided by 100,000,000 to keep it relevant with the other numbers.

* 另外两个部分组成了盒比，它使用体积和高-低范围.。等量图是基于卷和高-低范围以及。箱比是EMV的分母。注意，卷除以100，000，000，以保持它与其他数字相关。