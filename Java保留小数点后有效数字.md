## 题目描述

现在有 500 毫升的肥宅快乐水，要均分给 3 名同学，每位同学可以分到多少毫升？请输出一个数字作为输出。保留 6 位有效数字，且不使用科学计数法

## 输出样例

166.667

## 代码

```java
import java.math.BigDecimal;
import java.math.MathContext;
public class Main {
public static void main(String[] args) {
    // TODO Auto-generated method stub
    double a=500,b=3;
    BigDecimal m = new BigDecimal(String.valueOf(a/b)); 
    BigDecimal divisor = BigDecimal.ONE;  
    MathContext mc = new MathContext(6); 
    System.out.println(m.divide(divisor, mc));
  }
}
```
