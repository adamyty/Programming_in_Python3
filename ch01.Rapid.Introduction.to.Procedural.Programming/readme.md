ch01 Rapid Introduction to Procedural Programming note & practice

note:
1. .py開頭加上#!/usr/bin/python3這樣就可以直接執行這個.py
2. python中不存在變數這種東西，他使用的是物件參照(object reference)
3. tuple () 為不可變，list [] 為可變
4. x = [1,2,3] x.append("adam") -> [1, 2, 3, 'adam']
5. python的NULL是None，例如x = None
6. a = 9 : 0<=a<=10 , 為true。python可以直接這樣做數值判斷
7. membership運算符 p = [1,2,3,"frog"] : 2 in p會得到true，"dog" not in p也會得到true
8. 邏輯(bit)運算 : and or not，boolean值 True False
9. 控制執行流程的陳述句 if boolean_exp: 後續在這個code block的code用同樣的縮排來指明。例如
if a < 10:
	print(a)
print("end") """不屬於if 這個block
10.while陳述句
while True:
	item = get_next()
	if not item:
		break
11. for ... in陳述句
for var in iterable:
	suite
12. 例外處理
try:
	try_suite
except ValueError as err:
	print(err)
以上這樣的寫法會多印出一些error msg
13. a+=b 會比a = a+b快，同理其他運算也是
14. python會替字串跟list重載，也就是字串跟清單也可以作加法
15. IO : line = input("請輸入整數")，這樣會將輸入的值assign給line
16. 函數的建立
def functionName (argument):
	suite
argument可有可無，多個引數時用;隔開

practice:
1. bigdigits.py
輸入0-9的數字，在螢幕上以"*"號排列呈現的bigdigits
bigdigits_ans.py <= 改良版，"*"號改以輸入的數字呈現

2. average1_ans.py
連續輸入數個數字，最後輸出最小數、最大數以及平均數

3. awfulpoetry1_ans.py
建立一些單字清單，例如冠詞，主詞，動詞，副詞。使用random.choice在其中各選一個出來組成一句話

4. awfulpoetry2_ans.py
承3，要能接受使用者輸入1~10的數字來決定要印出幾列句子，default為5句

5. average2_ans.py
承2，要將輸入的數列排序，這樣就能求得中位數
