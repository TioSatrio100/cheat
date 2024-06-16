# cheat
cheat for informatic exam podfak

## To make this one
![Screenshot 2024-06-17 020625](https://github.com/TioSatrio100/cheat/assets/88955341/8d537ee9-6201-4942-b61b-a5f8fd67d531)

## add this code 
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
```

## To make this one
![Screenshot 2024-06-17 021340](https://github.com/TioSatrio100/cheat/assets/88955341/b96a7bd3-caa8-4a4b-bfb1-502415218a2a)

## add this code
```vba
Sub p_1()
Dim xn As Double, xk As Double, dx As Double, n As Double, h As Double


xn = Range("a")
xk = Range("b")
n = Range("n")
h = Range("h")

dx = (xk - xn) / n
For i = 1 To n
    x = xn + dx * (i + 1)
    y = f(x)
    Range("x").Cells(i) = x
    Range("y").Cells(i) = y
    Range("df_").Cells(i) = df(x, h)
Next
End Sub


Function f(x) As Double
f = Sin(Log(x)) ^ 2

End Function


Function df(x, h) As Double
df = (f(x + h) - f(x)) / h

End Function
```
## To make this one 
![Screenshot 2024-06-17 023515](https://github.com/TioSatrio100/cheat/assets/88955341/7576181c-5345-4f91-aa29-84af16615587)

## add this code 
```vba
Sub mat()
Dim xn As Double, xk As Double, dx As Double, x As Double
Dim yn As Double, yk As Double, dy As Double, y As Double
Dim A() As Double

xn = Range("xn")
xk = Range("xk")
n = Range("n")
yn = Range("yn")
yk = Range("yk")
m = Range("m")
dx = (xk - xn) / n
dy = (yk - yn) / m
ReDim A(1 To m, 1 To n)
For i = 1 To m
    y = yn + dy * (i - 1)
    For j = 1 To n
        x = xn + dx * (j - 1)
        A(i, j) = zz(x, y)
        Range("zz_").Cells(i, j) = A(i, j)
 Next
 Next
 
End Sub

 Function zz(x, y) As Double
 zz = Sin(x) * Cos(y) ^ 2
 
 
 End Function
```
