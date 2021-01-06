## BigInteger를 사용해야 하는 이유



| Type |                          범위                          |
| :--: | :----------------------------------------------------: |
| int  |             -2,147,483,648 ~ 2,147,483,647             |
| long | -9,223,372,036,854,775,808 ~ 9,223,372,036,854,775,807 |

int메모리는 4byte로 표현, long은 8byte로 표현할 수 있는 범위다. 범위를 벗어나면 오버플로우가 발생한다. BigInteger는 문자열 형태로 이루어져 있어 숫자의 범위가 무한하기에 어떠한 숫자든지 담을 수 있다.



## BigInteger 사용법

```
BigInteger bigInteger  = new BigIntger("10000");
```

- BigInteger를 초기화하기 위해서는 문자열을 인자 값으로 넘겨주어야 한다.

  

## BigInteger 클래스의 변수

- Zero
- ONE
- TEN



## BigInteger 계산

BigInterger는 문자열이기에 사칙연산이 안된다. 그렇기에 BigInteger 클래스의 내부에 있는 메서드를 사용해야 한다.

- 덧셈

  ```
  bigInteger.add('BigInteger자료형');
  ```

- 뺄셈

  ```
  bigInteger.subtract('BigInteger자료형');
  ```

- 곱셈

  ```
  bigInteger.multiply('BigInteger자료형');
  ```

- 나눗셈

  ```
  bigInteger.divide('BigInteger자료형');
  ```

- 나머지

  ```
  bigInteger.remainder('BigInteger자료형');
  ```

  

## BigInteger형 변환

BigInterger를 기본 타입으로 형 변환이 가능하다.

```
int num = bigInteger.intValue();
long num = bigInteger.longValue();
float num = bigInteger.floatValue();
double num = bigInteger.doubleValue();
Strubg num = bigInteger.toString();
```



## BigInteger 두 수 비교



```
BigInteger bigInteger1 = new BigInteger("100000");
BigInteger bigInteger2 = new BigInteger("1000000");
		
//두 수 비교 compareTo 맞으면 0 , 틀리면 -1
int compare = bigNumber1.compareTo(bigNumber2);
System.out.println(compare);
```

