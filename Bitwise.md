How David tried and failed solving Bitwise (needs edit)
========================

193, 35, 9, 33, 1, 9, 3, 33, 9, 225

user_arr.append( (((ord(char) << 5) | (ord(char) >> 3)) ^ 111) & 255 )

'<<' is left bit shift

'>>' is right bit shift

'|' is bit-wise or

'^' is bit-wise xor

'&' is bit-wise and

left bit shift 5

right bit shift 3

xor 111 (01101111)

and 255 (11111111)


193 = 11000001 > 

35 = 00100001 > 

9 = 00001001 > 

33 = 00100001 > 

1 = 00000001 > 

9 = 00001001 > 

3 = 00000011 > 

33 = 00100001 > 

9 = 00001001 > 

225 = 11100001 > 

result sequence = 
