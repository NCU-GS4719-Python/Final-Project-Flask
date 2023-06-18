# 110學年度 下學期 【程式設計-Python】 期末考

## 考試須知
1. 滿分100分，每題10分，須設計函式，依據題目要求，回傳(return)正確內容。運算主機為單核心CPU，每題的最長運算時間不得超過10秒，若超過10秒視同該題沒有答對。
1. 本次考試為Open Book，你可以使用任何資源但不可詢問別人，詢問別人或找槍手代答若經檢舉成立，本考試成績為0分
1. 我們這次期末考採用Open Book Github線上程式測驗，在作答同時，可以到「自動評分儀錶板」查詢自己的即時作答成績
1. 自動評分儀錶板網址：[https://ncuedu.tw/g/e/1102/python](https://ncuedu.tw/g/e/1102/python)

## 考試題目 每題10分
1. [p00.py](./exam/p/p00.py)\
    輸入：1個，int\
    輸出：1個，`True` or `False`\
    函式功能：判斷輸入引數是否為偶數，如果是偶數則return `True`，如果不是偶數則return `False`
    
1. [p01.py](./exam/p/p01.py)\
    輸入：不固定個數int or float\
    輸出：1個，float\
    函式功能：回傳(retuen)數值最小的數字(浮點數)
    
1. [p02.py](./exam/p/p02.py)\
    輸入：2個，int\
    輸出：1個，int\
    函式功能：讓使用者輸入兩個整數引數，分別為a與b。計算並回傳(return)從a開始的偶數連加到b的總和\
    Example 1:
    ```
    輸入：a=1, b=100
    運算：2+4+6+8+...+100 = 2550
    輸出：2550
    ```
    Example 2:
    ```
    輸入：a=1, b=9
    運算：2+4+6+8
    輸出：20
    ```
    
1. [p03.py](./exam/p/p03.py)\
    輸入：1個，int\
    輸出：1個，int\
    函式功能：回傳(retuen)輸入數字的反轉值\
    Example 1:
    ```
    輸入：123
    輸出：321
    ```
    Example 2:
    ```
    輸入：-123
    輸出：-321
    ```
    Example 3:
    ```
    輸入：120
    輸出：21
    ```
    
1. [p04.py](./exam/p/p04.py)\
    輸入：1個，2-9組成之int，不限定位數\
    輸出：1個，List，內含不固定個數elements，每個element為小寫英文字母組成之string且沒有空格(space)\
    函式功能：回傳(retuen)2-9組成之int對應英文字母組合之所有可能性\
    ![](./images/200px-Telephone-keypad.png)\
    \
    Example 1:
    ```
    輸入：23
    輸出：["ad","ae","af","bd","be","bf","cd","ce","cf"]
    ```
    Example 2:
    ```
    輸入：None
    輸出：[]
    ```
    Example 3:
    ```
    輸入：2
    輸出：["a","b","c"]
    ```
    
1. [p05.py](./exam/p/p05.py)\
    輸入：2個，其中，1個引數為List `l1` 內含多個int elements，另一個引數為int `x`\
    輸出：1個，List\
    函式功能：取出 `l1` 內小於 `x` 的int elements並加以排序為 `12`，`l1`內剩餘的elements為 `l3`，輸出值為 `l2+l3`\
    自動批改條件限制:`l1`內的elements與`x`均介於0到200之間\
    ![](./images/partition.jpg)\
    \
    Example 1:
    ```
    輸入：l1 = [1,4,3,2,5,2], x = 3
    輸出：[1,2,2,4,3,5]
    ```
    Example 2:
    ```
    輸入：l1 = [2,1], x = 2
    輸出：[1,2]
    ```

1. [p06.py](./exam/p/p06.py)\
    輸入：2個，其中，1個引數為List `nums` 內含多個int elements，另一個引數為int `target`\
    輸出：1個，List，內有2個elements\
    函式功能：輸入一個整數數組 `nums` 和一個整數 `target`，輸出 `nums` 的兩個索引，使它們加起來為`target`\
    自動批改條件限制:
    * 2 <= len(nums) <= 10<sup>4</sup>
    * -10<sup>9</sup> <= nums[i] <= 10<sup>9</sup>
    * -10<sup>9</sup> <= target <= 10<sup>9</sup>
    
    \
    Example 1:
    ```
    輸入：nums = [2,7,11,15], target = 9
    輸出：[0,1]
    解釋：因為 nums[0] + nums[1] == 9，所以我們回傳 [0, 1]
    ```
    Example 2:
    ```
    輸入：nums = [3,2,4], target = 6
    輸出：[1,2]
    ```
    Example 3:
    ```
    輸入：nums = [3,3], target = 6
    輸出：[0,1]
    ```

1. [p07.py](./exam/p/p07.py) **比較版本編號**\
    輸入：2個，string，分別為`version1`與`version2`\
    輸出：1個，int\
    函式功能：比較兩個版本編號的新舊，分成三種狀況
    * 若`version1 < version2` (`version2`較新)，則回傳(retuen) `-1`
    * 若`version1 > version2` (`version1`較新)，則回傳(retuen) `1`
    * 不屬於以上狀況，則回傳(retuen) `0`
    
    自動批改條件限制：
    * `1 < len(version1) < 500`
    * `1 < len(version2) < 500`
    * `version1`與`version2`是由`0-9`與`.`組成的字串
    * 每一個revision碼均為正整數，介於 0 到 2<sup>32</sup> 之間
    
    Example 1:
    ```
    輸入：version1 = "1.01", version2 = "1.001"
    輸出：0
    解釋："01" 和 "001" 表示同一個整數 "1"
    ```
    Example 2:
    ```
    輸入：version1 = "1.0", version2 = "1.0.0"
    輸出：0
    解釋：version1 沒有指定 revision 2 ，無法比較，所以輸出0
    ```
    Example 3:
    ```
    輸入：version1 = "0.1", version2 = "1.1"
    輸出：-1
    解釋： version1 的 revision 0 是 "0", version2 的 revision 0 是 "1"，0 < 1，所以 version1 < version2
    ```

1. [p08.py](./exam/p/p08.py) **完美平方**\
    輸入：1個，int\
    輸出：1個，int\
    函式功能：給定一個整數 `n`，返回總和為 `n` 所需的最少完美平方數\
    自動批改條件限制：1 <= n <= 10<sup>2</sup>
    \
    Example 1:
    ```
    輸入：n = 12
    輸出：3
    解釋：12 = 4 + 4 + 4
    ```
    Example 2:
    ```
    輸入：n = 13
    輸出：2
    解釋：13 = 4 + 9
    ```
    

1. [p09.py](./exam/p/p09.py) **H-Index**\
    輸入：1個，List，內含多個int elements，表示文章被引用的數量\
    輸出：1個，int\
    函式功能：輸入一個 `citations` List，內含int elements，`len(citations)`為某學者發表的文章總數，每個element表示每篇文章被其他人引用的次數。H-Index是一個混合量化指標，可用於評估研究人員的學術產出數量與學術產出品質。H-Index是2005年由美國加利福尼亞大學聖地亞哥分校的物理學家喬治·希爾施提出的。H-Index的定義為：「一個人在其所有學術文章中有N篇論文分別被引用了至少N次，他的H指數就是N」。如美國耶魯大學免疫學家理察·弗來沃發表的900篇文章中，有107篇被引用了107次以上，他的H指數是107。
    自動批改條件限制：
    * n == len(citations)
    * 1 <= n <= 5000
    * 0 <= citations[i] <= 1000
    
    \
    Example 1:
    ```
    輸入：citations = [3,0,6,1,5]
    輸出：3
    解釋：citations = [3,0,6,1,5] 表示該研究人員共有 5 篇論文，每篇論文收到 3, 0, 6, 1, 5 次引用。
    由於該研究人員有 3 篇論文每篇至少被引 3 次，其餘兩篇論文每篇被引用不超過 3 次，因此他們的 H-index 
    為 3。
    ```
    Example 2:
    ```
    輸入：citations = [1,3,1]
    輸出：1
    ```
    

