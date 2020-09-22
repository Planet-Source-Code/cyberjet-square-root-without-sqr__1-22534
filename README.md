<div align="center">

## Square root without sqr


</div>

### Description

The code is simply shows you how to evaluate square root without using sqr function. It may not really be usefull but if you interested it'll be of some value to you.By the way, i was surprised when after search for simmilar function only found examples of using Sqr(x)
 
### More Info
 
integer

In order to have this code working you need to create two text boxes "text1" and "text2" names are default and a command button named "command1" enter value you want to square root in text1 and you'll get result in text 2

square root of integer


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Cyberjet](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/cyberjet.md)
**Level**          |Beginner
**User Rating**    |5.0 (15 globes from 3 users)
**Compatibility**  |VB 4\.0 \(32\-bit\), VB 5\.0, VB 6\.0
**Category**       |[Math/ Dates](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/math-dates__1-37.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/cyberjet-square-root-without-sqr__1-22534/archive/master.zip)





### Source Code

```
Function sqroot(number As Integer) As Single
res = number / 2
Do
summed = (number - res * res) / (2 * res)
res = res + summed
Loop Until summed > -0.0001 And summed < 0.0001
Text2.Text = res
End Function
Private Sub Command1_Click()
sqroot (Int(Text1.Text))
End Sub
```

