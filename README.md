prime-number
============

import math def gcd(a,b): 	a,b=max(a,b),min(a,b) 	c=1 	while c: 		c=a%b 		a=b 		b=c 	return a	  def prime(n): 	gcdni=1 	help=int(math.sqrt(n)) 	i=2 	while i&lt;int(help)+1: 		gcdni=gcd(n,i) 		if (gcdni!=1) : 			return gcdni 		i=i+1 	return gcdni  def primitive(n,m): 	n=n+1 	list=[] 	i=0 	while i&lt;m: 		b=1 		while b==1: 			if(prime(n)==1): 				b=0 				list+=[n] 			n=n+1 		i=i+1 	return list  number=input("please enter number:") start=input("please enter srart for find:") print primitive(start,number)
