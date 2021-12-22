# Veri yapıları ve algoritmalar
## Projeler

### Soru 1

<details><summary>Insertion Sort</summary>

**[22,27,16,2,18,6]** -> ***Insertion Sort***

1. **Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.**

```
    [22,27,16,2,18,6] ( n )

    [2,27,16,22,18,6] ( n - 1 )

    [2,6,16,22,18,27] ( n - 2 )

    [2,6,16,18,22,27] ( n - 3 )
```

2. **Big-O gösterimini yazınız.**
```
    n + ( n - 1 ) + ( n - 2 ) + ( n - 3 ) + 1
    =
    n * ( n + 1 ) / 2
    ~~ n^2
    =>
    O(n^2)
```
3. **Time Complexity:** 

   1. **Average case: Aradığımız sayının ortada olması**
    
        ` [2,6,16,18,22,27] => 16,18 ` 

   3. **Worst case: Aradığımız sayının sonda olması** 
   
        `[2,6,16,18,22,27] => 27`

   4. **Best case: Aradığımız sayının dizinin en başında olması.**
   
        `[2,6,16,18,22,27] => 2`

4. **Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.** 
 
    `Avarage Case`

5. **[7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.**
   ``` 
   [7,3,5,8,2,9,4,15,6] ( n )

   [2,3,5,8,7,9,4,15,6] ( n - 1 )

   [2,3,4,8,7,9,5,15,6] ( n - 2 )

   [2,3,4,5,7,9,8,15,6] ( n - 3 )

   [2,3,4,5,6,9,8,15,7] ( n - 4 )

   ```
</details>



### Soru 2

<details> 
<summary>Merge Sort</summary>

**[16,21,11,8,12,22] -> Merge Sort**

1. **Merge sorta göre aşamalarını yazınız.**
   
    `[16,21,11,8,12,22]`
              
    `[16,21,11]` `[8,12,22]`
        
    `[16]` `[21,11]` `[8]` `[12-22]`
    
    `[16]` `[11,21]` `[8]` `[12-22]`
    
    `[16,11,21]` `[8,12,22]`

    `[8,11,12,16,21,22]`

2. **Big O gösterimini yazınız.**
   
    `O(logn)`
</details>

### Soru 3

<details><summary>Binary-Search-Tree</summary>

**[7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.**


```
1. Sırala [7, 5, 1, 8, 3, 6, 0, 9, 4, 2]  

2. Root bul [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

3. Root = 5 

                  5  
              /       \
             3         7
            / \       /  \
           2   4     6    8
          /                \
         1                  9
```

</details>