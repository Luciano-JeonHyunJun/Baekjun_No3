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

<h1>기찍 N 2742</h1>
자연수 N이 주어졌을 때, N부터 1까지 한 줄에 하나씩 출력하는 프로그램을 작성하시오.
첫째 줄부터 N번째 줄 까지 차례대로 출력한다.

<pre>
<code>
n = int(input())

for i in range(n , 0 ,-1):
    print(i)
</code>
</pre>

<strong>마찬가지로 n이라는 variable을 int로 값을 input받도록 합니다. 
    그후 range에 초기값인 n을 넣어주고, Argument에 0과 -1을 넣어준다면 숫자는 n에서 -1미만까지 즉 1까지 출력이 됩니다.
</strong>
  
<h1>A+B - 7 11021</h1>
두 정수 A와 B를 입력받은 다음, A+B를 출력하는 프로그램을 작성하시오.
첫째 줄에 테스트 케이스의 개수 T가 주어진다.
각 테스트 케이스는 한 줄로 이루어져 있으며, 각 줄에 A와 B가 주어진다. (0 < A, B < 10)
각 테스트 케이스마다 "Case #x: "를 출력한 다음, A+B를 출력한다. 테스트 케이스 번호는 1부터 시작한다.

<pre>
<code>
t = int(input())
i = 0

for i in range(t):
    i += 1
    a,b = map(int,input().split())
    print("Case #%s: %s"% (i, a + b))
    
</code>
</pre>

<strong> 우선 제 코드에선 i는 0으로 variable을 만들었습니다 t를 주어진다고 하니 t를 int로 input받구요.
    그런다음 for 반복문으로 t까지 반복을 합니다. t는 int니깐 반복이 되겟죠 .
    그후에는  i += 1 인데 '+='은 <a href="https://corytips.tistory.com/162">할당연산자</a>입니다.
    += 의 뜻은 "왼쪽 변수에 오른쪽값을 더하고 그 결과를 왼쪽 변수에 할당한다"
    즉 i += 1은 현재 i가 반복된 값으로 되었으니 , 쉽게 보면 " i + 1" 을 말하는것입니다.
    그러면 이제 a,b를 나누기만하면 되는데요. 따로 나눠도 되지만 코드는 깔끔한것이 좋으니
    a,b를 동시에 쓰고 map으로 동시에 인식받게한후 split로 리스트를 나누겟습니다.
    마지막 출력코드는 format방법으로 한거구요 %s는 string을 의미합니다! 그러면 첫번째 %s 에는 i가 대입되고
    두번째에는 a+b값이 대입이 되겠네요!
</strong>

<h1>A+B - 8 11022</h1>
첫째 줄에 테스트 케이스의 개수 T가 주어진다.
각 테스트 케이스는 한 줄로 이루어져 있으며, 각 줄에 A와 B가 주어진다. (0 < A, B < 10)
각 테스트 케이스마다 "Case #x: A + B = C" 형식으로 출력한다. x는 테스트 케이스 번호이고 1부터 시작하며, C는 A+B이다.

<pre>
<code>
case = int(input())

for i in range(case):
    a,b = map(int,input().split())
    print("Case #%s: %s + %s = %s"% (i + 1, a, b ,a + b))
</code>
</pre>

<strong>저도 이문제를 보고난후 조금 충격을 받았는데요. 분명 숫자 하나 차이인줄 알았는데 아니였습니다.
    우선 case라고 variable을 만들고 int로 input을 받게합니다. 그후에는 for반복문으로 int인 case까지 반복을 시키고
    a,b를 int를와 input으로 값을 받고 split으로 리스트를 나눠줍니다.
     이제 이 문제에서 제일 핵심인 출력문인데요. 첫번째 %s에는 i가 들어갑니다 i는 case까지 반복한뒤 +1을한 값입니다.
    그리고 두번째 %s는 a 세번째는 b가 출력이 되구요 마지막에는 ""을 안했으니 str그대로가 아닌 결과값이 format이 됩니다.
</strong>

<h1>별 찍기 2438</h1>
첫째 줄에 N(1 ≤ N ≤ 100)이 주어진다.
첫째 줄부터 N번째 줄까지 차례대로 별을 출력한다.

<pre>
<code>
n = int(input())

for i in range(1,n+1): #1부터 n까지
    print('*'* i)
<code>
</pre>

<strong>우선 n은 int로 input받습니다. 그다음에 for 반복문을 보면 1부터  n + 1 까지 반복을 하는데요.
        이제 출력을 하는코드인데 문제를 풀면서 느꼇지만 for i in range() 까지는 이제 쉬운데 print코드를 짜는게 이렇게 어려운건지 처음 알았습니다.
        우선 str이라고 알려주는 '' 따옴표를 씁니다 왜냐면 문제에서 예제를 보니 별을 출력하는건데 그냥 *을 쓰면 이건 string형태의 *이 아닌 곱하기로 인식을 합니다.
        그러면 이제 * 옆에 있는것도 *인데 이건 따옴표가 없는것을 봐선 곱하기를 말하는거같네요. 그러면 별 x 반복값인 i가 되는것입니다.
</strong>

<h1>별 찍기 - 2 2439</h1>
첫째 줄에는 별 1개, 둘째 줄에는 별 2개, N번째 줄에는 별 N개를 찍는 문제
하지만, 오른쪽을 기준으로 정렬한 별(예제 참고)을 출력하시오.

<pre>
<code>
num = int(input())

for i in range(1, num+1):
    print(" " * (num - i) + "*" * i)
</code>
</pre>

<strong>우선 num 이라는 variable을 만들고 int로 input받는것은 이제 기본적으로 한다고 생각하시면 편합니다.
        그후 이제 저번문제들과 똑같은 for 반복문을 사용하는데요. 이번에는 1부터 num(int형태) + 1 까지 반복한 값을 i로 저장한다고 합니다.
        이제 print코드인데요. print코드는 int(input())으로 써놓은것을 5로 바꿔서 설명드리겟습니다.
</strong>

<pre>
<code>
num = 5

for i in range(1, 5+1):
    print(" " * (5 - i) + "*" * i)
</code>
</pre>

<strong>코드를 풀이해보자면 일단 5+1까지 반복이니 6까지 반복으로 생각하시면 되겟습니다. 그러면 1부터 6미만까지 즉 5까지 출력이 되는것이구요.
        print코드를 보자면 우선 공백 x 5 - i + 별 x i 입니다 . 그러면 처음에는 i는 반복값이니 5-5가 되면 0 인데요. 
        그후에 별을 i는 반복값이니 5입니다 그러면 별 모양을 5개 출력하면 되는것입니다 . 
</strong>

<h1>X보다 작은 수 10871</h1>
정수 N개로 이루어진 수열 A와 정수 X가 주어진다. 이때, A에서 X보다 작은 수를 모두 출력하는 프로그램을 작성하시오.
첫째 줄에 N과 X가 주어진다. (1 ≤ N, X ≤ 10,000)
둘째 줄에 수열 A를 이루는 정수 N개가 주어진다. 주어지는 정수는 모두 1보다 크거나 같고, 10,000보다 작거나 같은 정수이다.
X보다 작은 수를 입력받은 순서대로 공백으로 구분해 출력한다. X보다 작은 수는 적어도 하나 존재한다.

<pre>
<code>
a, b = map(int, input().split())

c = list(map(int, input().split()))

for i in c:
    if i < b:
        print(i, end=" ")
</code>
</pre>

<strong>첫번째코드는 a,b를 map으로 동시에 int와 input을 받아주고 split으로 나눠줍니다.
        그리고 이제는 c라는 variable을 만든후 list를 만들어서 아까와 같이 해줍니다.
        이번 문제에서는 if 조건문을 활용해야하는데요 . 처음에는 for 반복문으로 c까지 반복을 해달라고 코드를 작성합니다.
        그후에는 if 조건문을 활용해서 "만약 i(반복값)이 b보다 작다면 " 이라는 조건을 만들어줍니다.
        마지막으로 조건이 맞을시 print로 반복값을 출력해주고 , end = "" 로 코드를 마무리 합니다.
</strong>

# Baekjun_No3(ENG.Ver)
This is a commit that solves the problem of the Baekjun online problem solving site. This commit may have an incorrect solution.
If you have any incorrect information, please give feedback to jhj091542@gmail.com.

<Please note that all translations have been made using Google Translator.

<h1>Multiplication table 2739</h1>
After receiving N, write a program that outputs the multiplication table N. Just print it according to the output format.
N is given in the first line. N is greater than or equal to 1 and less than or equal to 9.

<pre>
<code>
a = int(input())

for i in range(1,10):
    print("%d * %d = %d" %(a, i, a*i))
</code>
</pre>

<strong>At first, a was allowed to be input as an int, and in the loop, output from 1 to less than 10 was made,
When outputting, I used the format method that outputs %d, that is, integer (integer type). </strong>

<h1>A + B-3 10950</h1>
Write a program that takes two integers A and B and then outputs A+B.
In the first line, the number of test cases T is given.
Each test case consists of one line, with A and B given on each line. (0 <A, B <10)

<pre>
<code>
T = int(input())

for i in range(T):
    a,b = map(int, input().split())
    print(a+b)
</code>
</pre>

In the <strong>problem, we said that T was given, so we created a variable called T and received an input as an int.
  And in the for loop, it means to repeat as many as "T", and create a,b and apply the function at once through map.
  After that, int and input() were used to receive values ​​in integer type.
  Then split() the list one by one, and prints the desired A + B in the problem.
 </strong>
 
 <h1>Total 8393</h1>
 Given n, write a program that finds the sum from 1 to n.
 Print the sum from 1 to n.
 
 <pre>
 <code>
 a = int(input())
sum = 0

for i in range(a + 1):
    sum = sum + i
print(sum)
</code>
</pre>

<strong> First, create a variable called a and sum. Then a takes the input as an int, and sum just sets an int equal to 0.
  After that, after creating a loop to repeat a + 1, that is, int + 1, it is sum = sum + i, that is, 0 + (repeated value).
  After that, if you print the sum, the result of (repeated value) + 0 will be printed.
  </strong>
  
  <h1>Fast A+B 15552</h1>
If you are using Python, you can use sys.stdin.readline instead of input. However, in this case, it is recommended to add .rstrip() if you want to save the string because the newline character at the end is also input.

<pre>
<code>
import sys
case = int(sys.stdin.readline())

for i in range(case):
    a, b = map(int,sys.stdin.readline().split())
    print(a + b)
</code>
</pre>

<strong> The first thing I was talking about in the problem was to use the faster sys.stdin.readline instead of the input we used so far.
  At first, the problem seemed to be a very difficult problem, but if you think about it, it is very simple.
  Once sys is imported, the variable called case is recognized as an int, and then sys.stdin.readline() is used instead of input.
  After that, it repeats until the case after using the loop for as desired in the problem.
  Then finally, it was fast A + B, so after making a and b into variables and adding functions with map at once
  After using sys.stdin.readline(), split the list by splitting. After that, output A + B to complete the solution.
  </strong>
  
  <h1> Take N 2741</h1>
Given a natural number N, write a program that prints 1 to N, one per line.

<pre>
<code>
 n = int(input())

for i in range(n):
    print(i + 1)
</code>
</pre>

<strong>
 It is assumed that a natural number N is given, so you can start after receiving N as an int.
         If the for loop is executed up to n and i + 1 executed up to N is completed, the solution is completed.
</strong>

<h1>Gigi N 2742</h1>
Given a natural number N, write a program that prints N to 1, one per line.
Prints sequentially from line 1 to line N.

<pre>
<code>
n = int(input())

for i in range(n, 0 ,-1):
    print(i)
</code>
</pre>

<strong>Likewise, a variable called n is inputted as an int.
    After that, if you put the initial value n in the range and 0 and -1 in the Argument, the number will be output from n to less than -1, that is, 1.
</strong>
  
<h1>A+B-7 11021</h1>
Write a program that takes two integers A and B and then outputs A+B.
In the first line, the number of test cases T is given.
Each test case consists of one line, with A and B given on each line. (0 <A, B <10)
For each test case, print "Case #x:" and then print A+B. Test case numbers start at 1.

<pre>
<code>
t = int(input())
i = 0

for i in range(t):
    i += 1
    a,b = map(int,input().split())
    print("Case #%s: %s"% (i, a + b))
    
</code>
</pre>

<strong> First of all, in my code, i is made a variable with 0. Since t is given, it receives t as an int.
    Then, it repeats up to t with a for loop. Since t is an int, it will be repeated.
    After that, i += 1, but'+=' is <a href="https://corytips.tistory.com/162">assignment operator</a>.
    += means "add the right value to the left variable and assign the result to the left variable"
    In other words, i += 1 means "i + 1" if you look at it easily because i is a repeated value.
    Then we just need to divide a and b. It can be divided separately, but the code is good.
    We write a and b at the same time, let them be recognized as maps at the same time, and then split the list with split.
    The last output code was done in the format method, and %s means string! Then i is assigned to the first %s
    In the second, a+b value will be substituted!
</strong>

<h1>A+B-8 11022</h1>
In the first line, the number of test cases T is given.
Each test case consists of one line, with A and B given on each line. (0 <A, B <10)
For each test case, output in "Case #x: A + B = C" format. x is the test case number, starting from 1, and C is A+B.

<pre>
<code>
case = int(input())

for i in range(case):
    a,b = map(int,input().split())
    print("Case #%s: %s + %s = %s"% (i + 1, a, b ,a + b))
</code>
</pre>

<strong>I was also a little shocked after seeing this problem. I thought it was one number difference, but it wasn't.
    First, a variable called case is created and input is received as an int. After that, repeat the case with int with a for loop.
    Takes a,b as an int and an input and splits the list by split
     Now, this is the most important output statement in this problem. The first %s contains i. i is the value of +1 after repeating up to the case.
    And in the second %s, a and in the third, b is output. At the end, we didn't do "", so str is not the same, but the result value is the format.
</strong>

<h1>Taking stars 2438</h1>
The first line is given N(1 ≤ N ≤ 100).
Stars are printed in order from the first line to the Nth line.

<pre>
<code>
n = int(input())

for i in range(1,n+1): #1 to n
    print('*'* i)
<code>
</pre>

<strong>First, n is input as an int. Then, if you look at the for loop, it repeats from 1 to n + 1.
        It's the code that prints now, but I felt it while solving the problem, but for i in range() is now easy, but for the first time I knew if writing the print code was so difficult.
        First of all, I use quotation marks saying ``str'' because in the example in the problem, it prints a star, but if you use *, it is recognized as multiplication, not * in string form.
        Then, the * next to * is also *, but it seems to mean multiply because there are no quotation marks. Then it becomes i, which is a star x repetition value.
</strong>

<h1>Taking a star-2 2439</h1>
1 star on the first line, 2 stars on the second line, and N stars on the Nth line
However, print the stars sorted by the right (see example).

<pre>
<code>
num = int(input())

for i in range(1, num+1):
    print(" "* (num-i) + "*" * i)
</code>
</pre>

<strong>First of all, it is comfortable to think that creating a variable called num and receiving input as an int is now basically done.
        After that, we now use the same for loop as in the previous problems. This time, it is said that the repeated value from 1 to num (int type) + 1 is stored as i.
        Now this is the print code. The print code will be explained by changing what was written as int(input()) to 5.
</strong>

<pre>
<code>
num = 5

for i in range(1, 5+1):
    print(" "* (5-i) + "*" * i)
</code>
</pre>

If you try to solve the <strong>code, it is repeated until 5+1, so you can think of it as repeating up to 6. Then, from 1 to less than 6, that is, 5 is output.
        Looking at the print code, first of all, it is space x 5-i + star x i. Then i is a repetition value at first, so when it reaches 5-5, it is 0.
        After that, i is the repeat value, so it is 5, then you can print 5 stars.
</strong>

<h1>Number less than X 10871</h1>
A sequence of N integers A and an integer X are given. At this time, write a program that prints all numbers less than X in A.
In the first line, N and X are given. (1 ≤ N, X ≤ 10,000)
In the second line, N integers that make up the sequence A are given. All integers given are integers greater than or equal to 1 and less than or equal to 10,000.
Numbers less than X are separated by spaces in the order in which they were input, and output. There is at least one number less than X.

<pre>
<code>
a, b = map(int, input().split())

c = list(map(int, input().split()))

for i in c:
    if i <b:
        print(i, end=" ")
</code>
</pre>

<strong>The first code receives int and input at the same time as a map and divides a and b into split.
        And now, after creating a variable called c, create a list and do the same as before.
        In this problem, we need to use the if conditional. At first, I write the code to iterate up to c with a for loop.
        After that, an if conditional is used to create a condition of "If i (repeated value) is less than b".
        Finally, if the condition is met, the repeat value is printed with print, and the code is finished with end = "".
</strong>


 
  
        
