###### tags: `Ncu Statistics`
# Ncu Statistics Week 3 - Numerical Descirptive Measures

統計量數：
老師的開場白：介紹基本的量數資料
### Problem
![](https://i.imgur.com/gEI9yU3.png)
[單一變數]

---
### Table of Content:
> * 為什麼要找尋資料趨勢? (Why we dig into the Central Tendency of Data)
> * 位置量數(集中趨勢量數location) - (Measure of Central Trendency)
> * 位置量數(非集中趨勢量數) - Measure of Non Central Location
> * 差異量數 - Measure of Variability(Dispersion, Spread)
---

### Ask you five questions before you start the course.
* 統計學常用的指標有哪些? What are common index of the STatistics
* 

---
## 1. 為什麼要找尋資料趨勢? (Why we dig into the Central Tendency of Data)
[Statistics for Data Science I: Measures of Central Tendency Using R and Python](https://medium.com/datarunner/statistics-for-data-science-i-measures-of-central-tendency-using-r-and-python-6a20c25be7fe)

* Business Development Processes
* Decision-making periods 
![](https://i.imgur.com/NXhzp1S.png)
[Measures of Central Tendency]

## 1. 統計量數(Numerical Descriptive Measures)
集中趨勢量數: 分析一組量測數據的分布，數據中心值得量數。
除了數據的集中趨勢，位置變數還可以描述資料集內不同分配位置的價值(The values in a distribution associated with position other than center)<br>

Ex: 
First quarter(25%), third quarter(75%) position 

離中趨勢量數(Measures of Variability): 又稱差異量數，離中**差異情況和離散程度**的量數，表現出Dataset內個數散布的情形。表現出數據組內個數**散布**的情形。


---
From the Medium article([Statistics for Data Science I: Measures of Central Tendency Using R and Python](https://medium.com/datarunner/statistics-for-data-science-i-measures-of-central-tendency-using-r-and-python-6a20c25be7fe)): <br>
A measure of central tendency is a **summary statistics that attempts to describe an entire dataset with a single value that represents the centre of its distribution.** Due to it delivers a comprehensive summart if the whole dataset, it si one of the most essential concept in statistics.

---

## 2. 集中趨勢函數（Measure of Central Tendency）：
又稱為**集中量數**，代表一組資料中，個觀測值有某種**共同趨勢**。因為反應Dataset內觀測值的**集中位置（Central Location）**，又稱為**位置量數**（Location measures）

### 常用的集中趨勢量數：
> 1. 平均數 Mean
> 2. 中位數 Median
> 3. 眾數 Mode

### 1. 平均數(Mean)
最重要的、對簡單、常使用的集中量數；有「簡化作用、代表作用、比較作用」，如果沒有特別指明統計量數是何種平均數，通常是指算術平均數(arithmetic mean)<br>
> * 簡化作用: 以一個數值**簡化**一組資料的全部數值
> * 代表作用: 代表一組資料的**平均水準**
> * 比較作用: 便於兩個或兩個以上**資料之間比較**
    
* 母體平均數(Population mean)/ 樣本平均數(Sample mean):
代表資料整體的平均數，假設母體/樣本共有**N個觀測值(Observed values)/樣本數為n**
![](https://i.imgur.com/PYNU2CC.png)

* 平均數的特性:
![](https://i.imgur.com/XX4a3c1.png)

* 離差(Deviation)的和為0
任一組資料中，各「觀測值」與「平均數」之差，稱之為**離差**
![](https://i.imgur.com/O1HjF3r.png)

* 合併資料，並求平均數
若有k組資料合併成一組，其**項數n**與**平均數i**分別相加相乘
![](https://i.imgur.com/7jOBGem.png)

* 極端值(Outlier or Extreme Value)
極端值通常愛處理數據資料的過程，就會被消除，以免汙染整體資料或資料分析。
![](https://i.imgur.com/URI0gvY.png)

   
### 2. 中位數(Median)
當一組資料中有極端值時，其平均數的代表性會遭受質疑，此時使用中位數(Median )是較佳量數，因為中位數不會被Outlier影響。但，中位數較缺乏敏感性，因為**只考慮**居中位置的幾個數值，基於這些理由，中位數不適合做代數運算。

* 母體中位數(Population median)/ 樣本中位數(Sample median) 
兩者計算方法相同，需要將資料**依大小順序排列**，下面為母體中位數的計算方法。
![](https://i.imgur.com/hauWuig.png)

* 中位數的特性: 資料中，各觀測值和中位數差之絕對值總和最小
![](https://i.imgur.com/EwSYW2e.png)


### 3. 眾數(Mode)
一個資料中出現最多的數值，並非唯一，但也可能沒有。而眾數特別適合用於**質的資料(類別資料)**。優點為性質簡單，不受**極端值**影響。缺點為不夠細節，所以不適合做**代數運算**，在不存在眾數的狀況下，很難了解資料；又或者是有2個以上眾數時，很難判斷哪一個為集中量數。
EX:
![](https://i.imgur.com/udWUWzR.png)
![](https://i.imgur.com/reyIlBp.png)

### 4. 集中趨勢量數比較
* 適用性比較:
![](https://i.imgur.com/PXqq3xv.png)

* 優缺點比較:
![](https://i.imgur.com/pRozUTt.png)

**三者的大小的關係**決定變數的分配型態，變數的分配型態為偏態(skewness)分為: 對稱(symmetry)，左偏(leftward skewness)，右偏(rightward skewness)
右偏(Skewed to the right):
![](https://i.imgur.com/bUpw0in.png)

Ex:
![](https://i.imgur.com/U6kw9KW.png)
![](https://i.imgur.com/3k78yvl.png)


### 5. 非集中趨勢量數 
* 百分位數(percentile)
將資料依大小順序排列，並取99個等分點(分割成100等分)，則每一分點皆為百分位數

* 百分位數的計算步驟:
![](https://i.imgur.com/D5n8tTE.png)

* 四分位數(quartile)
![](https://i.imgur.com/CoYUthd.png)

* 百分位數/中位數/四分位數/十分位數對照表:
![](https://i.imgur.com/Se0et2n.png)

## 3. 差異量數(Dispersion measures)
衡量一組資料中，各個觀測值之間的變異(variability)或分散(spread)程度。可表現出資料的「**散布程度**」及「**分布**」的型態，並可以反映出平均數的**代表性**。理想的差異量數，應將**每一個數值**對其「集中量數」支離差(差異)程度加以處理較為恰當。
![](https://i.imgur.com/R0YhwAa.png)

---
重要的差異量數:
> 1. 全距(Range)
> 2. 四分位差(Quartile deviation)
> 3. 平均偏差(Mean absolute deviation, MAD)
> 4. 變異數(Variance)
> 5. 標準差(Standard deviation)
---

### 1. 全距(Range) 
一組資料中，數值「最大」與「最小」之**差距**。優點是意義簡單明瞭，計算容易；缺點是易受**極端值**影響，無法測出中間**各個觀測值之間**的差異情形

### 2. 四分位距(Interquartile Range, IQR)
為了避免全距(Range)的極端值(Outlier)缺點，改採用資料之**第三個四分位數Q3 = 上四分位數(upper-quartile)** 與 **第一個四分位數Q1 = 下四分位數(lower-quartile)** 之間的差距，稱之為四分位距。

* 四分位差(Quartile deviation):
將四分位距(IQR = Q3 - Q1)在除以2，所得量數稱為四分位差(Quartile deviation)，亦即
![](https://i.imgur.com/wogGZJQ.png)

* 四分位距和四分位差之特性:
    1. 四分位差常和**中位數**一起運用，就是以中位數表示依次數分配之 **集中趨勢**，可再以四分位差表示其**差異**情形
    2. 四分位距計算簡單、易於了解，且不受**極端值**影響
    3. **僅考慮**一半數值，對兩端之另一半樹直接位涉及，故不能表示全部數值分散及差異情形

### 3. 平均偏差(Mean Absolute Deviation) 
「**全距**」和「**四分位差**」皆沒有考慮資料全部數值，故無法適當地描述全部資料的差異情況；而平均偏差(MAD)**是根據全部數值求得**，故可表**整組資料**之完整的差異情形，較全距與四分位距感應靈敏。缺點是，計算平均偏差時，是取**離差**的絕對值加總，而有關**絕對值**的運算意義不甚明顯；平均偏差因具有平均的意涵，故與平均數的缺點相同，易受**極端值**的影響。

* 離差(deviation)
為一組資料中，**各個數值** 與 **平均數的差**，易稱為離均差(deviation about the mean)
![](https://i.imgur.com/FVkEUbO.png)

由於**各個數值與其平均數之離差**皆**有正有負**，所以離差的總和必為0，因此**無法顯示資料分配的差異情形**。


### 4. 變異數(Variance)
以「離差」為計算基礎，取離差的平方(square)做計算。而平均偏差取絕對值和變異數取平方，皆是為了避免離差正負相消。若A、B兩組資料平均數相同，而A的變異數遠小於B組，代表A組資料的**差異程度較小**，則**平均數較具代表性。**
![](https://i.imgur.com/tkPHuYU.png)

* 母體變異數(Population variance): sigma^2
計算:
![](https://i.imgur.com/AftVDAx.png)

證明:
![](https://i.imgur.com/zY5B42N.png)
![](https://i.imgur.com/RQkfpY9.png)

EX: 
![](https://i.imgur.com/8xnD0cV.png)
![](https://i.imgur.com/HaaRPJ1.png)
![](https://i.imgur.com/HjJIZoT.png)

* 樣本變異數(Sample variance)
[On the sample standard deviation, why do we substract N by 1](https://www.quora.com/On-the-sample-standard-deviation-why-do-we-subtract-N-by-1#:~:text=To%20give%20you%20a%20mathematically,variance%20an%20'unbiased%20estimator'.&text=data%20we%20have.-,For%20a%20variance%2C,mean%2C%20not%20the%20population%20mean.)

![](https://i.imgur.com/KkXVVm5.png)
![](https://i.imgur.com/BZ2FXWD.png)

樣本變異數之分母取n-1,而非n的理由為，在樣本資料中，會用**樣本平均數**來估算母體平均數，則會失去一個自由度(degree of freedom)，故除以n-1的樣本變異數S^2才會是母體變異數sigma^2的不偏估計量(unbiased estimator)

證明想法:
![](https://i.imgur.com/Sf0Obyl.png)
![](https://i.imgur.com/omBtwJq.png)

### 5. 標準差(Standard deviation):
將「變異數取平方根」，可將單位還原與**原來資料的單位一致(Same unit)**，相同單位的比較才是有意義的。

**變異數**取離差的平方[(xi - u)^2]**有一個嚴重的缺點**，取完離差平方後，資料的「量測單位」亦需要跟著平方，此時往往變為**無意義的單位**。
EX: 原來資料是以公斤為單位，取平方後變成**平方公斤**，是無意義的。

Population Standard Deviation計算:
![](https://i.imgur.com/2TaIDoe.png)

Sample Standard Deviation計算:
![](https://i.imgur.com/1Qqd2Lp.png)

* 資料和標準差/變異數的特性:
若依資料分配的「**標準差很小**」，則表示**大部分的數值集中於平均數附近**，此時「**平均數的代表性高**」，能夠使使用者更了解到資料分配狀況；反之
，平均數的代表性低。

平均數和標準差可以為0，代表資料中的所有數值均為相同
![](https://i.imgur.com/kJbzAP0.png)
![](https://i.imgur.com/jooETCu.png)

* 資料合併問題(母體資料):
![](https://i.imgur.com/b4INQU3.png)
![](https://i.imgur.com/pfy2ydt.png)
![](https://i.imgur.com/VcHjWu5.png)

* 資料合併問題(樣本資料):
[How do I combine standard deviations of two groups? - Sample](https://math.stackexchange.com/questions/2971315/how-do-i-combine-standard-deviations-of-two-groups)
![](https://i.imgur.com/KQk0Jfi.png)
![](https://i.imgur.com/DlofxzS.png)
![](https://i.imgur.com/l3RaAhv.png)

EX: 
![](https://i.imgur.com/aszHryL.png)
![](https://i.imgur.com/mlq3TOd.png)
![](https://i.imgur.com/EtrBGDw.png)
![](https://i.imgur.com/8TcpnO8.png)

* 變異數和標準差之優缺點:
    1. **變異數**或**標準差**計算與**所有數值**有關，故其特性為「**靈敏(Sensitivity)**」；憶及，資料中若有任一數值變動，則其變異數或標準差異必隨之變動。
    1. 變異數和標準差皆與**平均數(Mean)** 有 **密切關係**，且均皆能使用「代數運算」
    2. 缺點為，易受極端值(Outlier)影響，平均數也是。


### 6. 差異量數和位置量數比較
位置量數: 衡量一組資料之「集中趨勢」或「位置特性」。(集中趨勢量數、非集中趨勢量數)

差異量數: 衡量一組資料中，各個觀測值之間的變異(Variability)或分散(Spread)的程度。
![](https://i.imgur.com/OF4ESNv.png)



# 上課的筆記: =================
Deviation: 觀測值和平均數之差， 離差和為0
平均數一定是在資料重心的位置，所以離差和必定為0
離均平方和

## 4. 差異量數： 最終的目的，看資料有無代表性
衡量資料中，各個觀測值之間的變異或分散程度，可表現出資料的「散布程度」或「分布」的型態，並可反映出平均數的代表性。
1. 全距
2. 四分位距： 只看了一半的資料，無法縱觀資料全面，但是可以看出資料的Outliers，上四分位數 - 下四分位數
3. 離差和沒用
4. 平均偏差： 將各個數值的「離差」取絕對值，然後再求其平均數
5. 變異數： 取平均的差
母體變異數推導


