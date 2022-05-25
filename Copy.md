<img id="Img_CSharp" src="./Images/CSharp.png" width=128 height=72>

경기게임마이스터고  <br>
학생을 위한 <br>
C# 프로그래밍 입문
=================

---

# 목차

<details>
<summary><a href="#개요"> 1장. 개요 </a></summary>
<br>

- [(C#) 프로그래밍을 익혀야 하는 이유](#프로그래밍을-익혀야-하는-이유)
- [객체지향 프로그래밍(OOP)을 왜 늦게 다루는가?](#객체지향-프로그래밍을-왜-늦게-다루는가)
- [어떻게 공부하면 좋겠습니까?](#어떻게-공부하면-좋겠습니까)

</details>


<details>
<summary><a href="#기초-문법"> 2장. 기초 문법 </a></summary>
<br>

- [주석](#주석)
- [리터럴 값](#리터럴-값)
- [타입](#타입)
- [변수와 상수](#변수와-상수)

</details>

<details>
<summary><a href="#응용-문법"> 3장. 응용 문법 </a></summary>
<br>

- [응용 문법 - 1](#응용-문법---1)
- [응용 문법 - 2](#응용-문법---2)

</details>

<details>
<summary><a href="#객체지향-프로그래밍"> 4장. 객체지향 프로그래밍(OOP) </a></summary>
<br>

- [객체지향 프로그래밍 - 1](#객체지향-프로그래밍---1)
- [객체지향 프로그래밍 - 2](#객체지향-프로그래밍---2)

</details>

<details>
<summary><a href="#응용-라이브러리"> 5장. 응용 라이브러리 </a></summary>
<br>

- [응용 라이브러리 - 1](#응용-라이브러리---1)
- [응용 라이브러리 - 2](#응용-라이브러리---2)

</details>


---

# 개요
> 본 항목에서는 책에 대한 설명과 독자를 위한 정보를 제공합니다.

C#을 공부하려하는 경기게임마이스터고 학생들을 위한 교재입니다.

Visual Studio Community 혹은 컴파일러를 사용 가능하다는 전제 하에 진행합니다.

위의 방법이 불가능 하다면 아래의 온라인 컴파일러 사이트를 이용하시길 바랍니다.

<details>
<summary><i><strong>온라인 컴파일러</strong></i></summary>
<br>

- [Programiz(Light, Dark)](https://www.programiz.com/csharp-programming/online-compiler/)
- [Rextester(Light, Dark)](https://rextester.com/)
- [Dotnetfiddle(Light)](https://dotnetfiddle.net/)
- [OnlineGdb(Light, Dark)](https://www.onlinegdb.com/online_csharp_compiler)

</details>

+ # 프로그래밍을 익혀야 하는 이유
> 프로그래밍을 왜 해야하는가?

경기게임마이스터고는 게임개발자를 양성하는 마이스터고이며, 여러분은 개발자를 목표로 공부합니다.

아트나 기획을 한다 하여도 기초 문법에 해당하는 코드는 작성할 수 있어야 합니다.

+ # 객체지향 프로그래밍을 왜 늦게 다루는가
> 객체지향 프로그래밍(OOP)은 왜 4장에서 다루는가?

객체간의 관계로 구조를 이루어 내는 객체지향 프로그래밍은 2, 3장에서 다루는 기본적인 문법을 익혀 선형적인 코딩을 충분히 익힌 후, 이해하며 천천히 도전해도 좋습니다.

+ # 어떻게 공부하면 좋겠습니까
> 어떻게 공부하면 좋은가?

<img src="./Images/Easy.png" width=5% height=5% /> &nbsp; <img src="./Images/Normal.png" width=5% height=5% /> &nbsp; <img src="./Images/Difficult.png" width=5% height=5% /> 

장마다 난이도를 나누어 두었습니다. 자신에 맞는 공부를 하고 싶다면 아래의 방식을 추천합니다.

프로그래밍 언어를 처음 접하는 분이라면 일단, <img src="./Images/Easy.png" width=5% height=5% />을 보는 것을 추천합니다.

프로그래밍 언어를 어느정도 공부하여 기초 문법을 쉽게 이해할 수 있다면 <img src="./Images/Easy.png" width=5% height=5% />을 가볍게 둘러보시고 <img src="./Images/Normal.png" width=5% height=5% />을 읽은 뒤, <img src="./Images/Difficult.png" width=5% height=5% />을 보시면 됩니다.

마지막으로 C#을 경험한 적이 있으며 되새기는 것이 목적이라면 처음부터 하나씩 짚어보며 완독 해 보시길 바랍니다.

+ # 컴파일링 테스트
> Hello World!를 출력합시다.

코드가 원활히 컴파일링 되는지 확인을 합시다.

아래의 코드를 복사하여 실행시켰을 때, 콘솔 출력으로 'Hello World!' 가 출력된다면 성공입니다.

```cs
using System;

class HelloWorld
{
    public static void Main(string[] args)
    {
        Console.Write("Hello World!");
    }
}
```

테스트에 성공했다면 다음 장으로 넘어갑시다.

---

# 기초 문법
> 프로그램을 구성하는 기초 문법에 대해 다룹니다.

+ # 주석
> 프로그램 속 메모장. 주석 처리

코드 내에서 주석을 작성하는 방법을 설명하겠습니다.

코드는 앞서 1장에서 사용한 'Hello World! 출력 코드' 를 예로서 사용합니다.

```cs
using System; // System 네임스페이스 참조

class HelloWorld
{
    public static void Main(string[] args)
    {
        Console.Write("Hello World!"); // Hello World! 출력
    }
}

/*
    실행 결과 : Hello World!
*/
```

위 코드에서 확인할 수 있듯이 '//' 는 한 줄 주석입니다. '//' 이후, 한 줄 동안은 문장이 주석 처리됩니다.

'/\* ~ \*/' 은 '/\*' 과 '\*/' 사이를 모두 주석 처리합니다.

이러한 주석은 협업을 할 때, 다른 이용자에게 코드에 대한 설명을 하기 위해 사용되거나 혹은 메모를 위해 사용될 수 있습니다.

+ # 리터럴 값
> 코딩에 사용하게 될 데이터

리터럴 값(Literal Value)은 여러분의 컴퓨터에 미리 정의되어 있는 데이터 입니다.

앞으로 이 리터럴 값을 이용하여 프로그램을 구성할 것입니다.

정수형 리터럴(integer), 실수형 리터럴(floating point), 부울형 리터럴(boolean), 문자형 리터럴(character), 문자열 리터럴(string) 로 나뉘며 이에 해당하는 데이터는 이후, 타입에 대한 설명에서 다룹니다.

+ # 자료형
> 컴퓨터가 데이터를 나누는 기준

자료형은 컴퓨터에 저장되는 데이터의 기준입니다.

- 정수형   
    ```cs
    byte   
    short   
    int   
    long   
    ```
    정수형은 -1, 0, 1등의 정수 형식입니다.

- 실수형
    ```cs
    float
    double
    decimal
    ```
    실수형은 3.14, 1.41등의 실수 형식입니다.   
    float은 'f', double은 'd', decimal은 'm'을 숫자 뒤에 붙여 형식을 지정합니다. (기본값은 double입니다)

- 부울형
    ```cs
    bool
    ```
    부울형은 true, false의 값을 가지는 형식입니다.

 - 문자형
    ```cs
    char
    ```
    문자형은 '(문자)' 형식으로 사용하는 형식입니다. 모든 유니코드를 사용할 수 있습니다.

- 문자열
    ```cs
    string
    ```   
    문자열은 "(문자열)" 형식으로 사용하는 형식입니다. 문자형과 달리 ""안에 넣을 수 있는 글자 수 제한이 없습니다.

+ # 변수와 상수
> 기초 문법 3 부제

+ # 조건문
> 조건에 따라 실행되는 문장

조건문은 프로그래밍에서 프로그램 흐름을 조건에 따라 실행시키고 싶을 때 사용합니다.

- if문   
   
    다음은 if문의 기본적인 형식입니다.
    ```cs
        if(조건)
        {
            //조건이 참일 경우 실행할 코드
        }
    ```
    if 문은 조건이 참일 경우 코드블럭 안쪽에 있는 코드를 실행하고, 조건이 거짓일 경우 코드를 실행하지 않습니다.   

    아래의 코드는 간단한 if문의 예제입니다.
    ```cs
        int a = 10;
        int b = 20;

        if(a > b)
        {
            Console.Write("Hellow if!");
        }
    ```
    위의 코드에서 a는 10으로 20인 b보다 작으므로, a > b는 거짓입니다. 따라서 "Hellow if!"는 출력되지 않습니다.

---
# 응용 문법
> 응용 문법 설명

+ # 응용 문법 - 1
> 응용 문법 1 부제

+ # 응용 문법 - 2
> 응용 문법 2 부제

---

# 객체지향 프로그래밍
> 객체지향 프로그래밍(OOP) 설명

+ # 객체지향 프로그래밍 - 1
> 객체지향 프로그래밍 1 부제

+ # 객체지향 프로그래밍 - 2
> 객체지향 프로그래밍 2 부제

---

# 응용 라이브러리
> 응용 라이브러리 설명

+ # 응용 라이브러리 - 1
> 응용 라이브러리 1 부제

+ # 응용 라이브러리 - 2
> 응용 라이브러리 2 부제

---
