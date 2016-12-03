```
"The fault, dear Brutus, is not in our stars, but in ourselves.” 
(I.ii.141) Julius Caesar in William Shakespeare’s Julius Caesar 
Cipher Text: 7sj-ighm-742q3w4t
```

# Because flag have format RC3-2016-... so shift = 16
```
cipher='7sj-ighm-742q3w4t'.upper()
alphabet='ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789'
flag=''
for i in range(0, len(cipher)) :
    if cipher[i] == '-' :
        flag = flag + '-'
    else:
        index = alphabet.index(cipher[i]) - 16
        if index < 0 :
            index = len(alphabet) + index
        flag = flag + alphabet[index]
print (flag)
```

# ```RC3-2016-ROMANGOD```
