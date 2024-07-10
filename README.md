# [Full Ver] Chapter 1. Introduction to Computer Science and Python Programming

## Table of Contents

## 1. Introduction to Computer Science and Engineering

### **[1-1] What is computer science and engineering?**

Computer Science and Engineering(이하 CSE)은 계산, 자동화 및 정보를 연구하는 학문이다. 컴퓨터 과학은 알고리즘, 계산 이론, 정보 이론, 자동화 등의 이론적 분야부터 하드웨어 및 소프트웨어의 설계와 구현 등의 실용적 분야까지 포괄한다.

CSE에 포함되는 여러가지 분야 중에 다음 분야를 보통 중요하게 다룬다. (학부 레벨에서)

1. Basic Concepts of Programming Language
2. Data Structures and Algorithms
3. Computer Architecture
4. Operating System
5. Computer Network
6. Database System
7. Software Engineering

다음 분야들은 선택적으로 공부하는 과목들이다.

- System of Digital Circuit

- Embedded System

- Introduction to Compiler Design

- Distributed System Concepts

- Linear Algebra

- Introduction to Statistics

- Numerical and GPU Computing

- Linux Kernel Development

- Scientific Computing

- Computer Graphics

- Introduction to Cryptography

- Machine Learning

- Automata

- Discrete Mathematics

- BigData Mining

CSE는 굉장히 넓은 분야를 커버하고 있고, 분야의 이름을 보면 알 수 있듯 다양한 수학/공학의 영역과 맞닿아있다. 이렇다보니 전자, 기계공학 같은 다른 공학과 다르게 학부 때는 넓은 분야를 다양하게 커버하는 느낌으로 배우게 된다. 한 가지 깊게 배우는듯한 느낌을 받는게 있다면, ***Computer System***에 대한 내용과 ***Programming***에 대한 내용이다.

(Note : Coding $\neq$ Programming $\neq$ Development)

정리하자면, CSE는 컴퓨터를 이용하여 주어진 문제를 효율적으로 계산 가능하게 하는 것에 있다. 그렇기 때문에 컴퓨터가 이해할 수 있게 문제를 정의할 수 있는 “***Computational Thinking***”의 개념과 효율적으로 컴퓨터가 계산할 수 있게 하는 “***Problem Solving***”의 영역으로 나뉘게 된다.

Computational Thinking에도 여러가지 이론이 있지만, 가장 중요한건 현실의 문제를 컴퓨터가 계산 가능한 형태로 정의하는 것이다. 그리고 잘 정의가 된 문제를 컴퓨터가 계산할 수 있게 명령을 내리는 과정이 Problem Solving이다. 이것을 잘하려면 결국 Programming을 많이 해봐야 한다.

다음은 어떤 숫자가 주어지면, 해당 숫자가 홀수인지 짝수인지를 구분하는 Python 코드이다.

```python
number = ##

if number % 2 == 0:
	print("The given number is even!")
else:
	print("The given number is odd!")

```

이 간단한 문제를 컴퓨터가 완벽하게(?) 만들어내기 위해서는 몇 가지 가정이 필요하다.

- number가 계산 가능한 숫자여야 함.
- 홀수 / 짝수를 구분하는 로직이 수학적으로 정의될 수 있어야 함.
- 컴퓨터가 “현실적으로” 계산할 수 있는 범위내에 있어야 함.

이것들을 자세하게 이해하기 위해서 2가지의 개념을 좀 더 자세하게 배워보자.

### **[1-2] Computational Thinking**

- 예시를 가지고 각 방법론을 이해해보자.

Example : “Organizing a small team-building event for your office.”

                   (회사에서 소규모 팀 빌딩 이벤트 열기)

1. **Decomposition : 전체 문제를 작은 여러가지 문제로 나누는 과정.**
    1. 이벤트에 적합한 날짜 및 시간 선택하기
    2. 팀 빌딩 활동 선택하기
    3. 장소 예약 또는 필요한 공간 및 장비 준비하기
    4. 초대장 발송 및 RSVP 추적 (RSVP; Répondez s'il vous plaît, Reply Please 라는 뜻.)
    5. 다과 및 간식 준비
2. **Pattern Recognition : 주어진 문제의 반복적으로 나타나는 패턴을 찾는 과정.**
    1. 직원들은 퇴근 후 금요일에 열리는 이벤트를 선호하는 경향이 있음.
    2. 이전의 성공적인 팀 빌딩 활동에는 방탈출과 그룹 요리 수업이 포함되어 있음.
3. **Abstraction : 문제에서 해결해야할 주요한 정보를 수치화(또는 계산 가능하게)하는 과정.**
    1. 가능한 각 활동의 구체적인 세부 사항(예: 특정 방탈출 테마)을 제외한 팀 빌딩 활동 유형
    2. 모든 개인의 선호도를 고려하기 보다는 팀원 대다수의 선호도를 선택.
4. **Algorithmic Thinking : 추천을 수행하는 과정을 step-by-step으로 만드는 과정.**
    1. 직원들에게 설문조사를 실시하여 날짜와 선호하는 활동을 선택합니다.
    2. 선택한 액티비티에 적합한 장소 또는 서비스 제공업체를 조사하고 선택합니다.
    3. 장소 또는 서비스 제공업체를 예약하고 날짜와 시간을 확인합니다.
    4. 이벤트 세부정보와 RSVP를 추적할 수 있는 방법(예: 이메일 또는 온라인 이벤트 관리 플랫폼)이 포함된 초대장을 발송합니다.
    5. 확정된 참석자 수에 따라 필요한 다과 및 간식을 구매 또는 주문합니다.
    6. 이벤트 전에 리마인더를 발송하고 모든 물류 측면이 준비되었는지 확인합니다.
    

Example : “Designing a recommendation system for an online streaming platform”

1. **Decomposition : 전체 문제를 작은 여러가지 문제로 나누는 과정.**
    1. Collecting and storing user data (e.g., watch history, preferences, and ratings)
    2. Identifying relevant features for recommendations (e.g., genre, director, actors)
    3. Developing a similarity measure between movies or users
    4. Generating personalized recommendations based on the similarity measure and user data
2. **Pattern Recognition : 주어진 문제의 반복적으로 나타나는 패턴을 찾는 과정.**
    1. Users who like action movies tend to also enjoy sci-fi movies
    2. Users who rate a specific director highly are more likely to enjoy other movies by the same director
3. **Abstraction : 문제에서 해결해야할 주요한 정보를 수치화(또는 계산 가능하게)하는 과정.**
    1. Representing movies as feature vectors (e.g., genres, keywords, director, actors) and ignoring less relevant details (e.g., release date, box office earnings
    2. Representing users by their preferences, such as liked genres, favorite actors, and preferred movie lengths, while ignoring other non-essential information (e.g., user's location, age)
4. **Algorithmic Thinking : 추천을 수행하는 과정을 step-by-step으로 만드는 과정.**
                                          (여기서는 Collaborative Filtering을 예시로 사용.)
    1. Compute the similarity between users based on their preferences or ratings of movies (e.g., using cosine similarity or Pearson correlation)
    2. Identify the most similar users (e.g., a user's "neighbors") to the target user
    3. Generate recommendations by aggregating the preferences or ratings of the target user's neighbors, weighting them by similarity, and selecting the top-rated movies that the target user has not seen
    

### [1-3] Problem Solving

자료구조나 알고리즘을 사용하여 주어진 문제에 대한 풀이법을 코드로 작성하는 과정을 말한다. 여기에는 특정 요구 사항을 해결하거나 원하는 결과를 얻기 위해 소프트웨어 또는 시스템을 설계, 구현, 테스트 및 최적화하는 작업이 포함된다.

- (일반적으로 불리는) Problem Solving(PS)는 CSE에서 정의하는 각 분야에 맞는 문제로 정의되며, 이를 해결하는 알고리즘을 설계하는 것을 말한다.
- (코딩 테스트 분야) Problem Solving(PS)는 LeetCode, CodesForce로 대표되는 코딩 문제를 해결하기 위한 분야를 이야기한다. 문제 해결을 위한 방법론들(여러가지 풀이 스킬들)이 있으며, 주어진 제한 조건을 만족하는(e.g. Memory capacity, Time limit) 코드를 작성해서 해당 문제에 대한 “정확한” 정답을 출력해야한다. 알고리즘을 설계하고 코드로 풀어내는 것을 연습하기 위해서 만들어진 분야이다.

[Two Sum - LeetCode](https://leetcode.com/problems/two-sum/)

**Example.**

- 주어진 2개의 integer list가 있을 때, 두 개의 list가 공통으로 포함하고 있는 모든 원소를 출력하는 코드를 작성하세요.

Test cases.

1) input : L1 = [1, 2, 3, 4, 5], L2 = [4, 5, 6, 7, 8]
    output : [4, 5] (순서는 상관없음)

2) input : L1 = [1, 2, 3, 1, 1, 2, 3, 4, 5, 5], L2 = [4, 3, 1, 1, 2, 5, 6, 1, 12, 5, 6, 677]
    output : [1, 2, 3, 4, 5] (순서는 상관없음)

```python
def find_common_elements(L1, L2):

	## TO-DO : 공통으로 포함된 원소를 포함하는 리스트 L을 return하라.
	pass

	return L
```

## 2. Basic Programming Concepts

### [2-1] Basic Programming Concepts

1. **Programming Language**

Programming Language(이하 PL)이란, 컴퓨터 프로그램을 작성하기 위한 언어이다. PL은 언어로써 정의되기 때문에 ***문법(syntax)***와 ***의미론(semantics)***을 가진다.

한국어, 영어, 프랑스어 등을 자연어(Natural Language)라고 구분지어 부르면 PL은 다음과 같은 특징을 가진다.

1) 사람이 목적을 가지고 언어 체계를 만든다.

2) 언어를 번역하는 프로그램에 의해 기계어(Machine Instruction)으로 번역된다. 이 때 어떤 프로그램 계열을 사용하느냐에 따라 ***Compiler 기반 언어***와 ***Interpreter 기반 언어***로 크게 구분된다.

3) 언어가 가지는 패러다임이 있다. Procedure-based Programming, Object-Oriented Programming, Functional Programming 등이 있으며 하나의 언어가 여러 패러다임을 채택할 수 있다.

4) 컴퓨터가 이해하기 좋은 ***Low-level 언어(e.g. Assembly, C)***와 사람이 이해하기 편한 ***High-level 언어(e.g. Python, JAVA, JavaScript, Go, Swift 등)***로 크게 구분된다.

<!-- ![C언어로 만들어진 “Hello World” 출력 예시 코드.](%5BFull%20Ver%5D%20Chapter%201%20Introduction%20to%20Computer%20Scie%208e4acf5ef7884827a4c85ae229c5cd48/C_Hello_World_Program.png) -->
![C_Hello_World_Program](https://github.com/vanics225/fastcampus-joy/assets/174995648/eba4a354-ba5d-4ba6-b522-c92ce6023ed1)

C언어로 만들어진 “Hello World” 출력 예시 코드.

1. **Variables**

컴퓨터 프로그램이 값을 저장하고 있는 메모리 공간을 부르는 이름이다. 이 이름을 통해서 값을 저장하고, 확인하고 다양한 연산에 사용할 수 있다. 각 프로그래밍 언어마다 변수를 정의하는 방식이 정해져있다.

변수는 코드에 의해 쓰여지는 것을 ***선언(declaration)***되었다고 한다. 선언된 변수는 개념만 존재하다가, 코드가 컴파일되거나 실행되면 메모리 상에 올라가게 된다.
(Computer Memory에 대한 자세한 설명은 Chapter 3에서 다룹니다)

![variable.png](%5BFull%20Ver%5D%20Chapter%201%20Introduction%20to%20Computer%20Scie%208e4acf5ef7884827a4c85ae229c5cd48/variable.png)

프로그래밍은 변수들을 통해서 관리되는 데이터를 원하는 방식대로 처리하는 과정이라고 볼 수 있다. 각 변수들은 프로그래밍 언어에 의해서 정의된 여러 Data Type에 따라 값을 저장하는 방식이 다르다.

1. **Data Types**

PL에서는 실제 데이터를 변수들이 저장하는 방식을 정의하고 있는데, 이를 Data Type이라고 한다. PL마다 정의하는 Data Type이 다르며, 내부 처리 방식도 다르기 때문에 처음 어떤 PL을 배우게 되면, 맨 처음에 Data Type부터 배우게 된다. 일반적으로 대부분의 PL이 채택하고 있는 Data Type들은 다음과 같다.

**1) Integer(int)** : 정수를 나타낸다. 양수, 음수 모두를 표현하며 언어마다 숫자의 표현 범위가 정해져있다.
e.g. C언어는 32bits(4B)로 정수를 표현하며, 이 경우에 $-2^{31} \leq N \leq 2^{31} - 1$ 범위를 지원한다.

**2) Floating-point(float, double)** : 소수를 나타낸다. 여기서 소수는 실수를 나타내기 위해서 사용하는 개념이며, 컴퓨터는 무한소수를 표현하지 못한다. (즉, 일부 유리수와 모든 무리수를 근사해서 나타낸다) 얼마나 자세하게 표현하느냐에 따라서 ***float(single precision), double(double precision)***으로 나타낸다.

(실수 표현에 대한 자세한 설명은 Chapter 3에서 자세히 다룹니다.)

**3) Character(char)** : 글자 하나를 나타내며 유니코드(UTF-8) 기준으로는 전세계 대부분의 언어를 지원하기 때문에, 한글도 한 글자를 표현할 수 있습니다. UTF-8 기준으로는 영어는 1B로, 한글은 3B로 표현됩니다.

**4) Boolean(bool)** : True / False를 나타내며, 1B로 표현된다. (1bit도 충분하긴 함)

**5) List** : 여러 개의 원소를 포함할 수 있는 Data Type이며, 보통 Linked List로 구현된다. 동적으로 원소를 생성 및 삭제가 가능하기 때문에 편하게 여러 개의 데이터를 하나의 변수로 다룰 때 사용한다.
(Linked List에 대한 설명은 Chapter 2에서 자세히 다룹니다)

**6) Dictionary(Maps, associative array)** : key - value의 조합으로 데이터를 저장하는 구조이다. 데이터를 효율적으로 저장하기 위한 구조이며 List와 원소를 접근하는 방식에 차이가 있다.
(Associative Array는 Chapter 2에서 자세히 다룹니다)

1. **Operators**

Operator는 주어진 변수에 대해서 연산을 처리할 수 있는 기능을 말한다. 주로 선언된 변수의 Data Type에 따라 결정되며, 어떤 연산이 수행될 수 있느냐는 Data Type과 함께 정의되어 있기 때문에 문법을 잘 익히는 것이 중요하다. 대표적인 Operator는 다음과 같다.

**1) Arithmetic Operator** : 사칙연산과 같은 산술연산자를 의미한다. **+**, **-**, **x**, **/**, **%** 등이 있다.

**2) Comparison Operator** : 두 개의 변수 사이의 크기 관계를 결정하는 비교연산자를 의미한다. **==**, **!=**, **<=**, **>=**, **<**, **>**가 있다.

**3) Logical Operator** : 어떤 두 개의 표현식의 논리 관계를 결정하는 논리연산자를 의미한다. **AND**, **OR**, **NOT**이 있다.

**4) Assignment Operator** : 변수에 값을 할당하는 할당연산자를 의미한다. 과거에는 ← 로 사용되기도 하였으나, 내부 동작 원리를 이해하고 나면 오히려 혼선을 주는 경우가 있어 현대 PL에서는 대부분 **`=`**로 사용된다.

1. **Control structures: if-else statements, loops (for, while)**

프로그램을 구현할 때 로직을 설계하기 위해서 사용하는 표현식이다.

if-else statements로 조건에 따른 판단이 가능하다.

for, while statements로 조건에 따른 반복 수행이 가능하다.

![61e15c7c389e74b5fa857860_algorithm-flow.png](%5BFull%20Ver%5D%20Chapter%201%20Introduction%20to%20Computer%20Scie%208e4acf5ef7884827a4c85ae229c5cd48/61e15c7c389e74b5fa857860_algorithm-flow.png)

위의 그림을 Flow Chart라고 하는데, 위의 Flow Chart를 Python code로 작성하면 아래와 같다.

```python
sum = 0
count = 0

while count < 6:
	n = int(input())
	sum = sum + n
	count = count + 1

print(sum)
```

조건과 반복은 프로그램의 로직을 구성하는데에 아주 중요하므로, 실제 예시들을 구현해보면서 많이 익혀보자.

1. **Functions and modules**

PL에서 function(= procedure, method, subroutine)은 코드의 재사용성을 올리고, 기능 단위 코드를 분리해서 구현할 수 있는 개념이다. Function을 잘 사용하게 되면, 깔끔하고 유지보수하기 좋은 코드를 작성할 수 있다. 보통 프로그램 개발에서는 어떤 단위로 기능 구현을 할지 디자인을 하게 되는데, 이 때 기본이 되는 단위가 Function이 된다. Function에 필요한 기본적인 개념을 아래 Python code 예제와 함께 설명한다.

![Python-Function-Syntax.png](%5BFull%20Ver%5D%20Chapter%201%20Introduction%20to%20Computer%20Scie%208e4acf5ef7884827a4c85ae229c5cd48/Python-Function-Syntax.png)

**1) Function Definition** : 정의하는 함수의 이름과 arguments의 개수와 이름, 함수 내부에 사용할 코드를 모두 정의하는 단계

**2) Parameters (or Arguments)** : 함수 내부에서 사용할 (매개)변수. interface의 역할을 하며, 함수 외부에서 데이터를 받아오고 내부에서 처리하는 대리인의 역할을 한다. Parameter를 통해서 함수는 외부와 독립적으로 구현될 수 있다.

**3) Calling** : 정의된 함수는 함수 외부에서 불러와서 사용할 수 있다. 불러올 때는 함수에 정의된 arguments에 처리할 value들을 함께 전달해야한다.

**4) Return value** : 함수의 내부 코드가 모두 실행되면 함수를 호출한 대상에게 결과값을 돌려준다. 이 때 어떤 값을 돌려줄지는 함수 내부에서 정의할 수 있다. (필요에 따라 정의하지 않아도 된다.)

**5) Scope** : 함수는 구현의 편의성을 위해서 함수 내부에서 사용한 변수들은 외부와 별개의 독립적인 변수로 관리한다. 이런 변수들을 local variable이라고 하며, local variable들은 함수 외부에서 사용 및 참조가 불가능하다.

```python
def add_numbers(a, b):
	result = a + b
	return result

added = add_numbers(3, 5)
print(added) # 8
```

PL에서 이러한 Function을 확장해서 큰 규모의 프로그램을 유지보수하기 편하게 만들 수 있도록 Module이라는 개념을 지원한다. Module(= library = package)이란 프로그램을 특정 기능과 관련된 함수, 변수, 특정 자료구조 등과 함께 묶어서 관리하는 단위를 말한다. Module을 사용하면 프로그램을 체계적으로 관리할 수 있으며, 여러 명의 개발자가 협업하여 프로그램 개발을 할 때도 전체적인 디자인을 하기가 편하다. 이러한 Module 관리를 잘하는 것이 고급 개발자의 역량이라고 볼 수 있다.

이런 Module을 구현하고 관리하기 위해서는 프로그램 개발에 필요한 기능 명세가 자세하게 되어있어야 하며, 이를 구현 가능한 단위로 나누고 각 Module들이 합쳐져서 잘 돌아갈 수 있는 디자인이 필요하다. 구현하는 단계에서 고민해야하는 개념은 다음 4가지이다.

(이에 대한 자세한 내용은 Chapter 6에서 배웁니다)

**1) Organization** : 어떤 코드들이 함께 구성되어 있어야 하는지를 결정하는 개념이다. 좋은 코드는 비슷한 기능을 하는 코드들이 함께 구현되어 있어, 유지보수를 편하게 해준다.

**2) Reusability** : Module 단위로 구현하는 가장 큰 이유는 역시 해당 Module들을 재사용하는 것에 있다. 여러 프로젝트를 수행할 때 구현해둔 Module을 그대로 가져와서 편의에 맞게 활용할 수 있어야 좋은 Module이라고 할 수 있다.

**3) Namespace** : 보통 Module 구현을 할 때, 여러 개발자가 참여하기 때문에 코드의 각 영역들을 명시적으로 나눠야 한다. 이 때 사용하는 것이 Namespace라는 명시적인 구분을 통해서 해당 코드가 어떤 코드 파일에서 정의되었는지를 알 수 있다.

**4) Importing** : 프로그래밍을 할 때, 특정 Module에 구현된 함수나 변수를 사용하기 위해서는 해당 Module을 불러와야한다. 불러오는 과정은 해당 Module의 코드들을 메모리에 load하고 현재 프로그램과 연결하는 작업이라고 볼 수 있다.

아래 Python Code 예제를 통해서 간단한 Module 구현과 사용법에 대해 짐작할 수 있다.

```python
# File: main.py

def greet():
    message = "Hello from main!"
    print(message)

# Import the 'other_module' module, which has its own namespace
import other_module

# Call the 'greet' function defined in the 'main' module
greet()  # Output: Hello from main!

# Call the 'greet' function defined in the 'other_module'
other_module.greet()  # Output: Hello from other_module!

# Access the 'message' variable defined in the 'other_module'
print(other_module.message)  # Output: Greetings from other_module!

# This would raise an error, as 'message' is defined only within the 'greet' function's local namespace
# print(message)
```

```python
# File: other_module.py

message = "Greetings from other_module!"

def greet():
    message = "Hello from other_module!"
    print(message)
```

***Python은 특히 굉장히 많은 오픈소스 기반 모듈들이 많다***. 이를 통한 확장성이 엄청나게 뛰어나고, 특히 데이터 분석 분야와 관련된 오픈소스 프로젝트들이 mainstream이기 때문에 데이터 분석 분야를 공부할 때는 Python을 공부하는것이 좋은 선택지가 된다.

### [2-2] Python Installation and Setup (30 minutes)

- Installing Python and setting up the environment
- Introduction to Integrated Development Environments (IDEs)

### [2-3] Basic Python Syntax (1 hour)

- Expressions and statements
- Comments and documentation
- Indentation and code organization
- Strings, lists, tuples, dictionaries, and sets

### [2-4] Writing and Executing Simple Python Programs (2 hours)

- Interactive mode and script mode
- Input and output operations
- Error handling and exceptions
- File I/O
- Practical examples and exercises (e.g., simple calculator, text processing)

### [2-5] Introduction to Python Libraries (1 hour)

- What are libraries and why are they important?
- Popular Python libraries (NumPy, pandas, matplotlib)
- Installing and importing libraries
- Basic usage examples of common libraries