# Lecture-Note
Hexagon

그리기에 육각형이 없어서 직접 만들었습니다.  
사용방법은 아래 코드를  
`그리기도구 설정 - 사용자 정의 그리기 도구 설정 - 사용자 정의 그리기 도구 또는 컨테이너 추가`  
여기에 그대로 복사하시면 됩니다.

```
x1 = LN.getX1();
y1 = LN.getY1();
x2 = LN.getX2();
y2 = LN.getY2();

x3 = x1;
y3 = (y2 + y1)/2;

x6 = x2;
y6 = y3;

x4 = x1 + (x2-x1)/4;
y4 = y2;

x5 = x1 + 3*(x2-x1)/4;
y5 = y2;

x7 = x5;
y7 = y1;

x8 = x4;
y8 = y1;

LN.drawLine(x3, y3, x4, y4);
LN.drawLine(x4, y4, x5, y5);
LN.drawLine(x5, y5, x6, y6);
LN.drawLine(x6, y6, x7, y7);
LN.drawLine(x7, y7, x8, y8);
LN.drawLine(x8, y8, x3, y3);
```

아래는 90도 회전한 육각형입니다. (x,y 좌표를 서로 바꿈)
```
x1 = LN.getX1();
y1 = LN.getY1();
x2 = LN.getX2();
y2 = LN.getY2();

x3 = (x2 + x1)/2;
y3 = y1;

x6 = x3;
y6 = y2;

x4 = x2;
y4 = y1 + (y2-y1)/4;

x5 = x2;
y5 = y1 + 3*(y2-y1)/4;

x7 = x1;
y7 = y5;

x8 = x1;
y8 = y4;

LN.drawLine(x3, y3, x4, y4);
LN.drawLine(x4, y4, x5, y5);
LN.drawLine(x5, y5, x6, y6);
LN.drawLine(x6, y6, x7, y7);
LN.drawLine(x7, y7, x8, y8);
LN.drawLine(x8, y8, x3, y3);
```

