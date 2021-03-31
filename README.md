# Baekjun_No3
백준 온라인 문제풀이 사이트의 문제를 푸는 커밋입니다. 이번 커밋은 틀린 해결방안이 있을수 있습니다.
틀린내용이 있을시 jhj091542@gmail.com으로 피드백 부탁드립니다.

<h1>구구단 2739</h1>
N을 입력받은 뒤, 구구단 N단을 출력하는 프로그램을 작성하시오. 출력 형식에 맞춰서 출력하면 된다.
첫째 줄에 N이 주어진다. N은 1보다 크거나 같고, 9보다 작거나 같다.

<pre>
<code>
a = int(input())

for i in range(1,10):
    print("%d * %d = %d" %(a , i , a*i))
</code>
</pre>

<strong>처음에는 a를 int로 입력을 받을수 있도록하였고 , 반복문에서는 1부터 10미만까지 출력을 시켰으며 , 
출력을 시킬때는 %d 즉 integer(정수형)을 출력하는 format방법을 사용하였습니다. </strong>

<h1>A + B - 3 10950</h1>
두 정수 A와 B를 입력받은 다음, A+B를 출력하는 프로그램을 작성하시오.
첫째 줄에 테스트 케이스의 개수 T가 주어진다.
각 테스트 케이스는 한 줄로 이루어져 있으며, 각 줄에 A와 B가 주어진다. (0 < A, B < 10)

<pre>
<code>
T = int(input())

for i in range(T):
    a,b = map(int, input().split())
    print(a+b)
</code>
</pre>

<strong>문제에서 T가 주어진다고 했으니 T라는 variable을 만들고 int로 input을 받게하였습니다. 
  그리고 for 반복문에서는 "T" 만큼 반복을 하라는 뜻이고 , a,b를 만들고 map을 통해 한번에 기능을 적용시켰습니다. 
  그후 int , input()으로 정수형으로 값을 받게하였구요. 
  그 다음 split()로 리스트를 각각 하나씩 나누어 주고 , 문제에서 원하는 A + B 를 출력시켰습니다.
 </strong>
 
 <h1>합 8393</h1>
 n이 주어졌을 때, 1부터 n까지 합을 구하는 프로그램을 작성하시오.
 1부터 n까지 합을 출력한다.
 
 <pre>
 <code>
 a = int(input())
sum = 0

for i in range(a + 1):
    sum = sum + i
print(sum)
</code>
</pre>

<strong> 우선 a 와 sum 이라는 variable을 만들어줍니다. 그후 a는 int로 입력값을 받아주고 , sum은 단지 0 이라는 int를 값으로 정해줍니다.
  그후에는 반복문으로 a + 1 즉 int + 1까지 반복을 해달라는 반복문을 생성한뒤에 sum = sum + i 즉 0 + (반복값) 이라는것인데요 .
  그후 sum을 출력해주시면 (반복값) + 0 을 한 결과가 출력이 됩니다.
  </strong>
  
  <h1>빠른 A + B 15552</h1>
Python을 사용하고 있다면, input 대신 sys.stdin.readline을 사용할 수 있다. 단, 이때는 맨 끝의 개행문자까지 같이 입력받기 때문에 문자열을 저장하고 싶을 경우 .rstrip()을 추가로 해 주는 것이 좋다.

<pre>
<code>
import sys
case = int(sys.stdin.readline())

for i in range(case):
    a, b = map(int,sys.stdin.readline().split())
    print(a + b)
</code>
</pre>

<strong> 우선 문제에서 말하는것은 여태까지 사용했던 input대신 속도가 더욱 빠른 sys.stdin.readline 을 사용하라는 문제였다.
  처음에 볼때는 문제가 매우 고난도 문제같았지만 가만 생각을 해보면 매우 간단하다 그냥 문제에서 답을 알려줬다고 봐야한다.
  일단 sys를 import해준후 case 라는 variable을 int로 값을 인식시켜준후 input 대신 sys.stdin.readline() 이걸 사용하면 된다.
  그후 문제에서 원하는대로 반복문인 for 을 사용한후 case까지 반복을 시켜준다.
  그러면 마지막으로 빠른 A + B 였으니 a,b를 variable로 만들고 map으로 한번에 기능을 추가시킬수 있게 한뒤
  sys.stdin.readline() 사용후 split으로 리스트를 나누어주면 된다. 그후 출력은 A + B 를 시키면 해결 완료
  </strong>
  
  <h1> N 찍기 2741</h1>
자연수 N이 주어졌을 때, 1부터 N까지 한 줄에 하나씩 출력하는 프로그램을 작성하시오. 

<pre>
<code>
 n = int(input())

for i in range(n):
    print(i + 1)
</code>
</pre>

<strong>
 자연수 N이 주어졌다고 하니 N을 int로 input받게 한뒤 시작을 하면 됩니다.
         for 반복문으로 n까지 실행이 되게 하고 N까지 실행이 된 i를 + 1 하면 해결 완료
</strong>

  
  
  
