Lab-1
=====


--power :: Integer -> Integer -> Integer
--power n k | k < 0 = error "power: negative argument"
--power n 0 = 1
--power n k = n * power n (k-1) 
--Assignment 1: k+1

--Assignment 2: power1 = product [2,2,2,2,2]
--"a list with k elements, all being n" t.ex n=2 k=5 --> 2^5=2*2*2*2*2
-- Solution: power n k = product (replicate k n)

power :: Integer -> Integer -> Integer
power n 0 = 1
power n k = (n * n)^div k 2 --- k == even 


--odd n*(n^k-1)
