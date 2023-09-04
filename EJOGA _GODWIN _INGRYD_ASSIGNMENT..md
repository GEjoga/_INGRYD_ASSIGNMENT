# ASSIGNMENT... WEEK 4


```python
'''
1. using the zipped function, merge two list into a list of tuple
2. write a program to iterate two list simultaneously. hint: list can be string and int.(print out a maping of both object)
3. write a program that uses filter to find all prime number in a range of number 
4. use a loop and any HOF (higher order function) to print every 2nd element of an iterator with its index
'''
```




    '\n1. using the zipped function, merge two list into a list of tuple\n2. write a program to iterate two list simultaneously. hint: list can be string and int.(print out a maping of both object)\n3. write a program that uses filter to find all prime number in a range of number \n4. use a loop and any HOF (higher order function) to print every 2nd element of an iterator with its index\n'




```python

# 1. using the zipped function, merge two list into a list of tuple

list1 = ["boy", "girl", "woman", "man", "child"]
list2 = ["cars", "bicycle", "dock", "train", "lorry"]

nlist = zip(list1, list2)

print(tuple(nlist))
```

    (('boy', 'cars'), ('girl', 'bicycle'), ('woman', 'dock'), ('man', 'train'), ('child', 'lorry'))
    


```python
#write a program to iterate two list simultaneously. hint: list can be string and int.(print out a maping of both object)
list3 = ["Rosemary", "Hellen", "Jonathan", "Kuti"]
list4 = [34,23,5,65]

def newlist(list3, list4):
    return list3, list4

b = map(newlist, list3, list4)

print(list(b))
```

    [('Rosemary', 34), ('Hellen', 23), ('Jonathan', 5), ('Kuti', 65)]
    


```python
# 3. write a program that uses filter to find all prime number in a range of number 

def prime(n):
    if n <=1:
        return False
    else:
        for i in range(2, n):
            if n % i == 0:
                return False
    return True

n= 100
x= filter(prime, range(n))
print(list(x))
```

    [2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47, 53, 59, 61, 67, 71, 73, 79, 83, 89, 97]
    


```python
#4. use a loop and any HOF (higher order function) to print every 2nd element of an iterator with its index
```


```python

```
