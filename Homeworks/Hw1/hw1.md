# 编译原理作业1
**张博厚 PB22071354**

## 2.3

### 2.3.(b)
由0,1构成的, 任意两个0均不相邻,且不以0结尾的数字串.

### 2.3.(c)
0,1构成的,以000/001/010/011结尾的数字串.

## 2.4

### 2.4.(a)
令$otherchar = (b | c | d | f | g | h | j | k | l | m | n | p | q | r | s | t | v | w | x | y | z)$\
则待求串为: $(otherchar)^* a (otherchar)^* e (otherchar)^* i (otherchar)^* o(otherchar)^* u(otherchar)^*$

### 2.4.(c)

$chars = a | b |...| z$

所求串为$/*\ chars^*\ ( \ /\ |\ (*^*\ chars\ chars^*))^*\ *^*\ */$

### 2.4.(e)
先考虑相邻字母均不同的串:
$$S_9: 9$$
$$S_{8-9}: (8\ |\ S_9\ 8)(S_9\ 8)^*(S_9\ |\ \epsilon)\ |\ S_9$$
$$...$$
$$S_0: (0\ |\ S_{1-9}\ 0)(S_{1-9}\ 0)^*(S_{1-9}\ |\ \epsilon) |\ S_{1-9}$$

则最多有一处字母相邻的串为: $S_0S_0$
