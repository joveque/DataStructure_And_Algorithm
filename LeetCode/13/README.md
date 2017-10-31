
# Roman to Integer

## 题目
　　Given a roman numeral, convert it to an integer.</br>
　　Input is guaranteed to be within the range from 1 to 3999.</br>
## 思路
　　罗马数字有如下符号：</br>
　　Ⅰ（1）Ⅴ（5）Ⅹ（10）L（50）C（100）D（500）M（1000）</br>
　　计数规则：</br>
　　1.若干相同数字连写表示的数是这些罗马数字的和，如III=3；</br>
　　2.小数字在大数字前面表示的数是用大数字减去小数字，如IV＝4；</br>
　　3.小数字在大数字后面表示的数是用大数字加上小数字，如VI=6;</br>
　　组合规则：</br>
　　(1)基本数字Ⅰ、X 、C 中的任何一个，自身连用构成数目，或者放在大数的右边连用构成数目，都不能超过三个；</br>
放在大数的左边只能用一个。</br>
　　(2)不能把基本数字 V 、L 、D 中的任何一个作为小数放在大数的左边采用相减的方法构成数目；放在大数的右</br>
边采用相加的方式构成数目，只能使用一个。</br>
　　(3)V 和 X 左边的小数字只能用Ⅰ。</br>
　　(4)L 和 C 左边的小数字只能用×。</br>
　　(5)D 和 M 左 边的小数字只能用 C 。</br>