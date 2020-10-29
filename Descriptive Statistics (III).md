###### tags: `Ncu Statistics`
# Ncu Statistics Week 4 - Numerical Descirptive Measures(III) 


### Problem:
![](https://i.imgur.com/XWVyE8l.png)
[這裡圖的X軸標示是不是有問題](解決)

![](https://i.imgur.com/BBqSZj5.png)
這裡應該是以u為主的主動差(central)

![](https://i.imgur.com/Y5zScMv.png)
這裡的「劃」一垂直線 >> 畫

![](https://i.imgur.com/Denylm1.png)
![](https://i.imgur.com/aG08VJM.png)
這一題在計算xi^2平方時，這裡的組中點65只有2次，而非24次。


![](https://i.imgur.com/yIA1yMv.png)
這邊分析種樹的方法只有2種，不是3種

---
### 前一章節重點:
位置量數: 衡量一組資料之「集中趨勢」或「位置特性」。(集中趨勢量數、非集中趨勢量數)<br>
差異量數: 衡量一組資料中，各個觀測值之間的 **變異(Variability)或分散(Spread)** 的程度。<br>

---

---
Table of Content
> 1. 平均數和標準差的應用(Using Mean and Standard Deviation to Describe Data)
> 2. 偏態量數，峰態量數與動差(Skewness, Kurtosis, and Moment)
> 3. 探索性資料分析(Exploratory Data Analysis)
> 4. 分組資料之各種統計量數的計算(The Numerical Measures of Grouped Data)
---

## 平均數與標準差的應用

### 1. 差異量數(Dispersion measures)
#### 絕對差異量數(Measures of absoulute dispersion)：
統計資料的「性質相同」、「單位相同」、「平均數差異不大」，皆可使用絕對差異量數比較。
EX: 全距、四分位差、平均偏差、標準差。

#### 相對差異量數(Measures of relative dispersion): 
**放在同一個基準點上面，比較不同的係數**。可以根據統計資料的「性質不同」、「單位不同」、「平均數差異很大」，則可使用相對差異量數比較。<br>
EX: 這一題可以發現**資料性質相同**，都是要比較長度，但是資料的單位不同，造成兩組資料的平均數和**標準差**差異很大，<br>
![](https://i.imgur.com/VKcYFq5.png)
![](https://i.imgur.com/fGH8XqQ.png)

若認為I組差異程度小於II組(s.d 1 < s.d 2)，也不合理。所以使用「相對差異量數」比較便可以解決問題。
而所謂的「相對差異量數」與某一**集中量數**或**其他適當數值**之比(和原資料的單位無關，通常以百分比表示)<br>

較為常見的相對差異量數，為**變異係數(Coefficient of variation, CV)**，以標準差除以平均數，去計算標準差佔平均數的百分比例。又分為母體變異係數和樣本變異係數。<br>
![](https://i.imgur.com/9ioBbGj.png)
![](https://i.imgur.com/owlws7y.png)

#### 變異係數(Coefficient of variation)(沒有單位): 
主要是用來衡量「**相對分散程度**」的量數，以標準差除以平均數，計算***標準差佔平均數的百分比例**；同時也將單消除。<br>
欲比較兩組或以上的資料之差異情況，當:
> 1. 單位不同的資料
> 2. 單位相同，但平均數差異很大的資料

則可以使用變異係數來了解資料性質

### 2. Z分數(Z-score, Standard score)
又稱**標準分數**。針對「單一資料點」計算，來衡量**某些特定資料點**在整筆資料中的相對位置；而非「整群資料」的相對位置量數。<br>
其用來表示第i項觀測值Xi與平均數(x bar)的距離**有幾倍標準差**。是以**大於或小於平均數幾倍標準差**來衡量<br>
![](https://i.imgur.com/1DkAflb.png)

EX: 比較分屬於不同資料的兩個資料之相對大小<br>
![](https://i.imgur.com/bmhB8Ys.png)
![](https://i.imgur.com/tJlUKzN.png)


### 3. 經驗法則（EMPIRICAL RULE）
主要是利用經驗法則的資料分配形狀來做觀察，觀察**以Mean為中心**，兩邊加減幾個標準差的區間，來查看會**有多少觀測值落在這些區間內**。<br>
當資料分配呈現中型或丘型形狀(bell-shaped or mound-shaped)時，亦即為「對稱分配」(median = mean = mode)<br>
![](https://i.imgur.com/boSTM5a.png)

像是:<br>
![](https://i.imgur.com/kTnOEal.png)
![](https://i.imgur.com/IRzu6jr.png)

計算過後得到的結論(S為標準差)<br> 
![](https://i.imgur.com/FV4WVK4.png)


### 4. Chebyshev定理(非Symmetry分配)
當一組資料**標準差較小**時，表示其**各數值間的差異較小**，且大多數的數值**集中在平均數**附近，計算**到底會有多少個數值落在某一區間內?**<br>
落在對稱於平均數的兩個數值之間的觀測值比例與標準差存在某些關係，稱為Chebyshev定理，而這些**不對稱的數據資料分布**，則可以使用Chebyshev來分析。<br>
![](https://i.imgur.com/P2QR4tW.png)

適用於任何的資料分配，當觀測值落於**平均數左右k個標準差**的區間內之比例，至少為:<br>
![](https://i.imgur.com/9Y7QFKm.png)
![](https://i.imgur.com/Hg9HqHT.png)

但Chebyshev定理計算出來的數值，為一個**保守的估計值**。此數值只說明**有多少比例落在此區間**，至於實際上有多少比例，則不得而知。<br>
![](https://i.imgur.com/tPhURIi.png)

#### CHEBYSHEV定理和經驗法則之比較
![](https://i.imgur.com/SONNFL9.png)

---

## 偏態量數，峰態量數與動差(Skewness, Kurtosis, and Moment)
**分配形狀量數(Measures of shape):<br>**
除了位置量數與差異量數，在描述資料分布的型態時，亦可以用分配形狀量數(measures of shape)

### 1. 偏態量數(Skewness)
一筆資料的**非對稱性(Asymmetry)於中央(Mean)附近**。用來衡量資料「**分布的形狀**」。(上一章節有提到[中位數、平均數、眾數的比較](https://hackmd.io/L6xqL0drSq6JFqIr2TKb2g?view))
1. 以中心位置成對稱形狀時稱為「對稱分配」
2. 中心位置左偏「左偏分配」
2. 中心位置又偏「右偏分配」

#### 母體偏態量數(coefficient of skewness)
![](https://i.imgur.com/3RPRHfA.png)

依據**母體的資料**，其第三級主動差M3為母體「偏態」<br>
![](https://i.imgur.com/gDtaizR.png)

### 2. 峰態係數(Kurtosis)
一筆資料在**中央(Mean)附近群距的情況(厚實程度)**，用來衡量資料分配的「**峰態高低**」。依據母體資料，其第四級主動差M4為母體「峰態」，故母體峰態量數為:<br>
![](https://i.imgur.com/I772zQH.png)

#### 峰態量數(coefficient of kurtosis)
![](https://i.imgur.com/HwcZnNV.png)

### 3. 動差(Moment)
用來表達**資料數據全體特性**的數學模型，是一種利用「冪次方」為其轉換基礎的平均數。通常會先減去一特定數，再取冪次方後，**計算全體平均數**，一般稱為以特定數為中心之動差。<br>
![](https://i.imgur.com/BBqSZj5.png)

#### 原動差(Raw moment/ Moment about zero)
**以0為主(亦即就是原資料為主)的原動差**，每筆數據資料減去0，並再根據幾級(**r**)動差而r次方。母體資料和樣本資料的計算方法相同。<br>
![](https://i.imgur.com/QKagyUJ.png)
![](https://i.imgur.com/PNCSc7o.png)

#### 主動差(Principle moment/ Central moment)
**以r為主的主動差(因為只有r(次方數)，在主動差才開始有用)**。每筆數據資料減去u(Mean)，並再根據幾級(**r**)動差而r次方。母體資料和樣本資料的計算方法相同。<br>
![](https://i.imgur.com/HmfcFiZ.png)

這裡想特別介紹**第三級母體主動差(3rd central moment)**
第三級母體主動差主要用於衡量<font color = 'r'>**偏態**</font><br>
![](https://i.imgur.com/1EJ4fT3.png)

這裡想特別介紹**第四級母體主動差(4th central moment)**
第四級母體主動差主要用於衡量<font color = 'r'>**峰態**</font><br>
![](https://i.imgur.com/Nupp5hb.png)

#### 主動差和原動差的區別
![](https://i.imgur.com/TktI9z1.png)

#### 動差證明(「原動差」轉「主動差」)
![](https://i.imgur.com/y5UM7Ia.png)

---
## 探索性資料分析(Exploratory data analysis, EDA)
統計學家將**統計圖表(visual method)** 和 **統計量數(main characteristics)** 加以結合，發展出探索性資料分析法。而總共有2種技術:
> 1. 枝葉圖(stem-and-leaf display)
> 2. 箱型圖(box plot)

### 1. 枝葉圖/莖葉圖(stem-and-leaf display or stem-plot)
是一種**描述資料特性**的統計圖，外觀和**直方圖**相當，但相較於直方圖，有提供較完整的數據資料，用來說明**資料的分布狀況**。優點是**保留原始數據資料**；缺點是**不適用於大筆的數據資料**。<br>

**枝葉圖繪圖步驟:**<br>
考慮觀測值的大小，**由小到大**按順序排列。選擇前一位數或二位數(前置數字)，**由小至大寫成一行**，並畫一垂直線。例如: 若觀測值為二位數，則前置數字取一位；若觀測值為三位數，則前置數取二位, etc.<br>

實例解析:<br>
![](https://i.imgur.com/CsCMZic.png)

我們會照著<br>
![](https://i.imgur.com/BSE6pdK.png)


### 2. 箱型圖(Box plot)
各種的**次數分配表**和**統計圖**的繪製有助於資料的整理和表示，而各種**統計量數**(平均數、標準差)的計算則**可測度資料的特性**。<br>

而箱型圖(又稱為鬍鬚盒(box-and-wisker plot))，結合了**統計圖和統計量數**(即**五個彙總量數**)，所繪製而成<br>
> 1. 最小值(Minimum)
> 2. 第一四分位數(First Quarter)
> 3. 中位數(Median)
> 4. 第三四分位數(Final Quarter)
> 5. 最大值(Maximum)

鬍鬚盒**適用**於描述**單一屬量性變數的分配**，分為盒(box)與鬚(whisker)兩個部分。<br>
#### 盒(Box)
是資料主要集中的部分，由下四分位數(Q1)、中位數(Me)、上四分位數(Q3)
等量數組成。<br>
#### 鬚(Whiskey)
資料離散的部分，由最小值(X_smallest)、最大值(X_largest)等量數來表示位置。以虛線繪製，從盒子兩端延伸至**內圍**的最小和最大值。<br>
![](https://i.imgur.com/Z5XDcYG.png)
#### 內圍值(Inner fences)
![](https://i.imgur.com/n0EFuIa.png)

#### 外圍值(Outer fences)
![](https://i.imgur.com/4i7PWgo.png)

#### 可疑離群值(Suspect Outliers)
當觀測值落在「內圍」和「外圍」**之間**，稱為**可疑離群值(Suspect Outliers)**；當觀測值落在**外圍值**之外，稱為**最高可疑離群值(Highly Suspect Outliers)**

---

## 分組資料之各種統計量數計算
### 1. 已分組資料(Grouped data)的各種統計量數計算:
資料進行分組，可能會因為資料量過於龐大，若能先加以分組，可以變於**彙總資料與統計量數**的計算。例如: 好比妳的資料有一萬筆數據，將這一份資料進行**質的分組或其他統計量數計算(平均數、標準差、變異數、峰態系數、變異係數等)**<br>

但有時在分組之後，可能**會失去一些資訊**，好比說原來觀測值在以分組的資料中再也看不出來了。而分組資料只能**視未分組資料(原始資料)** 的<font color = 'red'>**近似值**</font>

### 分組資料(Grouped data)的兩個基本假設:
1. 各組資料**均勻分布**於該組內:<br>
假設有一組 **組界(Class Boundary)為10 ~ 20**，其**次數為4(代表有4個數值在此區間內)**，表示該組的4個數直接均勻分布於10~20之間。<br>

3. 各組資料**集中於**該組的**組中點**:<br>
假定**各組中的所有數值，皆可視為等於各組組中點的數值**；如果以上面的例子來解釋，就是4個數字皆可視為15(組中點)<br>

### 統計量數於分組資料內的計算:
#### 1. 平均數(Mean)： 
![](https://i.imgur.com/v4lTN92.png)

**分組(Grouped data)與未分組資料(Raw data)** 所求得的平均數(Mean)**略有差異**，但如果組的間距越小，取的組數越多，分組平均數會越來越接近未分組平均數，但還是近似值，永遠都不會一樣。<br>

#### 2. 變異數(Variance):
![](https://i.imgur.com/72xNGI5.png)

這裡有一點很重要，因為分組資料(Grouped data)並非完整原始資料(Raw data)，所以我們還是會**減少一個自由度(degree of freedom)**，變異數的算法是採用**樣本變異數、標準差算法**，我們需要除以的是(n - 1)而非(n)。<br>

例題:<br>
![](https://i.imgur.com/0wMsUcW.png)

#### 3. 中位數(Median):
![](https://i.imgur.com/fPQZcHh.png)

重要假設: 資料皆**均勻分布於該組內**，我們現在要找下列資料集內的中位數(Suppose n = 18)，然後我們發現n = 18，在F(i-1) ~ Fi之間，此時需要的是**利用內插法**來求資料的中位數(**這只是推估值，並非真正的中位數**)<br>
![](https://i.imgur.com/dbTEiMZ.png)
![](https://i.imgur.com/OilBWgr.png)

這裡要提一下，為什麼是取F(i-1)的上組界(upper boundary) & Fi(upper boundaey)上組界? 因為我們要想這一個數值其實是在組界為(li ~ ui)內，而其實(li ~ ui) = (ui-1 ~ ui)。所以我們才會這樣取值<br>
![](https://i.imgur.com/xHQIJpe.png)

#### 4. 百分位數(percentile)
和前面的指數計算並無太大差異，求位置指標i = (k/100)* n，不論i為指數或非整數，皆保留原值。例如: i = 15.5，則利用15.5去作內插法，計算以下累積次數； i = 16，則利用15.5去作內插法，計算以下累積次數。**不需要在找16 + 17之值平均**。

#### 5. 眾數(Mode)
在次數分配表中，眾數為次數最多的那一組，該組又稱為眾數組(Mode class)。根據**均勻分配**(經驗法則)的假設，則眾數為眾數組為之**組中點**，眾數組的組中點會**隨著組距和組界**的變動而變，所以求出來的眾數只是**近似值**。<br>

資料顯示，組界為70~80的那一組，稱之為眾數組<br>
![](https://i.imgur.com/miq676J.png)

而一般常見求分組資料之眾數的方法有兩種:
> 1. 金氏法(King's Method)
> 2. 克氏法(Czuber's Method)

#### 6. 金氏法(King's Method)
計算方法:<br>
![](https://i.imgur.com/WBjqaxE.png)
![](https://i.imgur.com/c00BPDO.png)

#### 7. 克氏法(Czuber's Method)
計算方法:

![](https://i.imgur.com/ZFDtt2f.png)












