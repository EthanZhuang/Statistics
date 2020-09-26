
# NCU 統計課(Statistics)
## 20200923 敘述統計（I）Ch1
![](https://i.imgur.com/1aroXR5.png)
![](https://i.imgur.com/0pV9SAS.png)

---
Table of Content:
* 資料型態(Types of Data)
* 資料搜集方法(Collecting Data)
* 衡量的尺度(Measurement Scales for Variables)
* 次數分配表(Graphical Methodds for Describing Data)
---

Ask you five questions before you start the course.
* 何謂統計學 What is Statistics?
* 統計科學? The Science of Statistics?
* 統計學的用途? What types of Statistical Application can be used in Business?

---

### 1. 何謂統計學?
任何一個領域的**問題或爭議**，皆能透過**收集與分析數據**來找出最適合解答，並加以**制定策略**

日常應用的統計學:
1. **民意調查**: <font color = 'red'>收集</font>選民回應並預測選舉結果
2. **顧客意見**: 消費者提供資訊，以便公司分析出消費者對產品的喜好
3. **產品管理**: 出貨前，針對產品抽樣檢查，以便控管出貨或保留的決策
4. **其他**: 天氣預報、物價指數、經濟指標、交通意外事故統計等...

解決問題的流程(PPDAC):
![](https://i.imgur.com/H0eb3mx.png)

#### 例子(Example): 利用「STAR分析」，來描述故事和事件

情境(Situation):<br>
電影「魔球」，運動家球隊想要「增加營收」，增加營收則需要更多觀眾，而觀眾來看球的原因是球隊「贏球」，所以該如何「贏球」和增加營收是有很大的關係?

任務(Task):<br>
找到讓球隊增加營收的方法。分析出贏球關鍵是「得分」，得分跟「上壘率」相關。分析上壘率對於勝場數的關係是長打率(slugging percentage)的兩倍以上。

作為(Action):<br>
運動家隊開始簽上壘率高，但薪水被嚴重低估的球員，和其他球隊專簽明星球員不同。

結果(Result):<br>
運動家隊再重組後的第三年，勝率相較於三年前增加49% = (97 - 65)/ 65 * 100%，勝場數來到97場。在之後來到勝場數102場，勝率高達63%

### 2. 何謂STAR分析?

> · 情境（Situation)：Set the context for your story。經歷或是工作職務的簡單概述。<br>
> · 任務（Task)：What was required of you。撰寫工作職務中，你主要負責的工作或角色。<br>
> · 作為（Action)：What you actually did。具體寫出你特別的一兩件特別事蹟。<br>
> · 結果（Results)：How well the situation played out。簡單來說就是你達到什麼樣的成果。<br>

### 3. 統計科學(The science of Statistics)

統計科學是將大量的資料(數值、類別資料)，透過統計方法，在不確定的狀況下，淬鍊出有用的/目標的資訊(information)/知識(knowledge)的方法。統計學可被視為**產生新的認知**(理解)的方法

![](https://i.imgur.com/pWU1gnv.png)
![](https://i.imgur.com/fCcoIUw.png)

### 4. 應用領域(Application areas)
* 數理統計(Mathematical Statistics): 
以數學原理闡明統計方法理論，證明各種統計公式的來源
例: 財務工程學、管理數學、精算數學、DS、ML

* 應用統計(Applied Staistics):
將統計方法應用於科學研究、企業管理、行政措施等領域
例: 商用統計學、生物統計、經濟統計

### 5. 統計方法
統計學一般區分成兩種:
* 敘述統計(Descriptive Statistics ):
將收集來的原始資料(raw data)，進行組織、彙整、以及表格呈現，不涉及任何理論假設。<br>
簡單來說，敘述已知、分析事件的資料，掌握特徵。
![](https://i.imgur.com/fEcbsbB.png)

* 推論統計(Inferential Statistics):
將部分資料，實際樣本參數(sample)地分析結果，用於更大範圍的資料-
參數(parameter)的某些特性推論，做為策略研擬的依據。<br>
簡單來說，推論未知，由部分事件資料，推論事件的整體
![](https://i.imgur.com/KsDbY3g.png)

### 6. 母體(population)
調查者欲調查的所有個體的集合，在機率論中稱為宇集(universal set)，其所包含的元素(element)為所欲研究對象的全部個體。

母體的界定範圍又很重要，如果界定範圍發生錯誤，會導致抽樣調查有問題，後續的統計檢定、分析、推論都會產生錯誤。<br>
![](https://i.imgur.com/rn89iKF.png)

例: 廠商在推出新的咖啡前，想要了解消費者的是喝看法、喜好，則可將母體設定為「曾經喝過咖啡的社會大眾」。

#### 母體大小(population size):
* 有限母體(finite population):
若所包含的元素個數為「有限的」<br>
例: 全體國民、吸毒人數等...

* 無限母體(infinite population):
所包含的元素個數為「無限的」，或者是數量多到數不完<br>
例: 空氣中懸浮例子個數、太空的行星數量等...<br>
![](https://i.imgur.com/qStWa6Z.png)

#### 參數/母數(parameter)
用來描述母體特徵量數(characteristic of population)稱為參數/母體參數
**常用的三個參數:**
1. 母體平均數: 描述中央趨勢的特徵
2. 母體變異數: 描述離散趨勢的特徵
3. 母體比例: 描述母體比例特徵

#### 樣本(Sample): 
母體的部分集合(subset)<br>
目的為對於未知的母體參數進行統計推論(Statistical Inference) 
例如: <br>
    - 研究問題: 服用憂鬱藥的治癒率<br>
    - 樣本: 服用憂鬱藥的病人<br>
    - 樣本大小: 10000人<br>

**常用的的三個重要統計量**
1. 樣本平均數: 描述中央趨勢的特徵
2. 樣本變異數: 描述離散趨勢的特徵
4. 樣本比例: 描述樣本比例的特徵

![](https://i.imgur.com/eWZ6ecY.png)

### 7. 統計學的用途
1. 使資訊變得**有意義**<br>
例: 繪製統計圖、統計圖表或計算統計量數<br>
![](https://i.imgur.com/8D25MF5.png)

2. 處理**不確定**的問題(方法: 機率理論、貝氏決策理論)<br>
例: 物價水準的上升、下降? 新產品的成功機率? 競爭者的產能表現?

3. 分析各種變項之間的**關係**<br>
確定因素之間的因果關係和規律性，進而分析與比較

4. 預測
![](https://i.imgur.com/BZUUWen.png)

---
## 20200923 Statistics Chapter 2

---
Table of Content:
* 資料型態(Types of Data)
* 資料搜集方法(Collecting Data)
* 衡量的尺度(Measurement Scales for Variables)
* 次數分配表(Graphical Methodds for Describing Data)
---


