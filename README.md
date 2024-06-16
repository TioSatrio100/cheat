# cheat
cheat for informatic exam podfak

add this code 
```vba
Sub p_1()
Dim xn As Double, xk As Double, dx As Double, n As Double

xn = Range("a")
xk = Range("b")
n = Range("n")
dx = (xk - xn) / n
For i = 1 To n
    x = xn + dx * (i + 1)
    y = f(x)
    Range("x").Cells(i) = x
    Range("y").Cells(i) = y
Next
End Sub


Function f(x) As Double
f = Sin(Log(x)) ^ 2

End Function
