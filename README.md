# Cpp-Primer
Answer of the practice
1.18
答案在1.17中已给出
1.19
习题1.10已实现该功能
1.20及之后的习题因为Sales_item.h文件出错不能使用，因此暂时未写入。
2.1
int、long、long long与short的区分
short长度为2，适用范围为-2^7~2^7-1
int长度为4，适用范围为-2^31~2^31-1
long与int相似
long long 长度为8，适用范围为-2^63~2^63-1
无符号类型与带符号类型的区别
无符号类型从0开始，到该类型能保存的最大数目。
如 unsigned short 从0开始到255
带符号类型则是以0为中间点，正数负数各占一半左右(正数要少一个，因为0的存在)
如short从-128到127
float与double的区别
同为保存浮点数，double比float精度要高，而且二者运算速度相差无几，甚至在某些情况下double比float运算速度还快，因此C++ primer中推荐使用double而不是float
2.2
利率因为肯定小于0，而且可能在小数点后有较多位数，因此选择double类型是较为合适的，本金一般为整十整百甚至整千的数目，因此选择int类型较好，而付款则是经过利率和本金的运算，因此用double表示会更好一点。
2.3
32 2^32-32
32 -32 0 0
2.5
(a)char、wchar_t、string、wchar_t*
(b)int、unsigned int、long、unsigned long、int、int
(c)double、float、long
(d)int、unsigned int、double、double
2.6
有区别。以0开头的数字是八进制数字，定义上面一组变量时无问题，定义下面一组时，因为09是没有意义的八进制数字，因此编译器会提示出错。
2.7
