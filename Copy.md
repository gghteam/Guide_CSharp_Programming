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
    정수형은 `-1`, `0`, `1`등의 정수 형식입니다.

- 실수형
    ```cs
    float
    double
    decimal
    ```
    실수형은 `3.14`, `1.41`등의 실수 형식입니다.   
    float은 'f', double은 'd', decimal은 'm'을 숫자 뒤에 붙여 형식을 지정합니다. (기본값은 double입니다)

- 부울형
    ```cs
    bool
    ```
    부울형은 `true`, `false`의 값을 가지는 형식입니다.

 - 문자형
    ```cs
    char
    ```
    문자형은 `'(문자)'` 형식으로 사용하는 형식입니다. 모든 유니코드를 사용할 수 있습니다.

- 문자열
    ```cs
    string
    ```   
    문자열은 `"(문자열)"` 형식으로 사용하는 형식입니다. 문자형과 달리 ""안에 넣을 수 있는 글자 수 제한이 없습니다.

+ # 변수와 상수
> 기초 문법 3 부제

+ # 조건문
    > 조건에 따라 실행되는 문장

    조건문은 프로그래밍에서 프로그램 흐름을 조건에 따라 실행시키고 싶을 때 사용합니다.
    + ## if문   
   
        먼저 조건문의 가장 기초가 되는 if문 부터 알아봅시다.   
        >if문은 쉽게 생각해서 `만약` 이라는 키워드를 코드에서 사용하는 것입니다.

        다음은 if문의 기본적인 형식입니다.
        ```cs
        if(조건식)
        {
            //만약 조건식이 참일 경우 실행할 코드
        }
        ```
        if 문은 만약 조건식이 `참`일 경우 코드블럭 안쪽에 있는 코드를 실행하고, `거짓`일 경우 코드를 실행하지 않습니다.   

        아래의 코드는 간단한 if문의 예제입니다.
        ```cs
        int a = 10;
        int b = 20;

        if(a < b) //a가 b보다 작으므로 참
        {
            Console.Write("Hellow if!"); //조건식이 참이기 때문에 실행되는 코드
        }
        ```
        <details>  
            <summary>출력 결과</summary>  

            Hellow if!
        </details>  
        앞으로도 출력 결과를 가려놓을테니, 열어보기 전에 어떤 출력값이 나올지 생각해봅시다.

        위의 코드는 만약 a가 b보다 작다면 코드블럭 안쪽에 있는 코드를 실행하도록 작성한 코드입니다.   

        a에는 `10`이 들어있고 b에는 `20`이 들어있습니다.   
        따라서 a는 b보다 작으므로 위의 조건식은 `참`이 되고 콘솔에는 `"Hellow if!"`가 출력되게 됩니다.   

        if문에 대해서 감을 잡으셨다면 else문으로 넘어가 봅시다.

    + ## else문   

        else문은 if문과 함께 사용되는 코드입니다.
        >if가 만약 이라면 else는 아니라면 이라고 생각하셔도 좋습니다.

        먼저 else문을 사용하는 방법부터 알아봅시다.
        ```cs
        if(조건식)
        {
            //만약 조건식이 참일 경우 실행할 코드
        }
        else
        {
            //위의 조건식이 참이 아니라면 실행할 코드
        }
        ```
        else문은 위의 조건식이 `참이 아니라면` 실행되는 코드입니다.   
        주의할 점은, else문을 쓸 때는 `반드시` if문을 코드블럭 위쪽에 함께 써야한다는 것입니다.   

        else문에 대해 어느정도 감이 잡히셨다면 아래의 예제를 살펴보겠습니다.
        ```cs
        int a = 10;
        int b = 20;

        if(a > b) //a가 b보다 작으므로 거짓
        {
            Console.Write("Hellow if!"); //a가 b보다 작기 때문에 실행되지 않는 코드
        }
        else
        {
            Console.Write("Hellow else!"); //위의 조건식이 참이 아니기 때문에 실행되는 코드
        }
        ```
        <details>  
            <summary>출력 결과</summary>  

            Hellow else!
        </details>  
        위의 예제에서는 a가 b보다 작으므로 조건식은 참이 아닌 `거짓`이 됩니다.   
        따라서 if문 안쪽에 있는 `"Hellow if!"`는 출력되지 않고, else문 안쪽에 있는 `"Hellow else!"`가 출력되게 됩니다.   

        다음은 else if문에 대해서 알아봅시다.

    + ## else if문

        else if문 또한 if문과 함께 사용되는 코드입니다.
        >else if는 아니라면과 만약을 결합한 ~이 아니고, 만약 ~라면 이라고 이해하시면 됩니다.   

        else if문은 아래의 형식처럼 사용합니다.
        ```cs
        if(조건식)
        {
            //만약 조건식이 참일 경우 실행할 코드
        }
        else if(조건식)
        {
            //위의 조건식이 거짓이고 조건식이 참일 경우 실행할 코드
        }
        else
        {
            //위의 조건식이 참이 아니라면 실행할 코드
        }
        ```
        else if문은 `위의 조건식` 이 거짓이고, `조건식` 이 참일 경우 실행되는 코드입니다.
        >현재 코드에서는 if문 안에 있는 조건식이 위의 조건식 이고, else if문 안에 있는 조건식이 조건식 입니다.   

        else if문을 사용할 때 if문은 `반드시 사용`해야 하지만, else문은 `사용하지 않아도` 됩니다.   

        else if문은 말로 설명하는 것보다 예제를 보는게 훨씬 더 이해하기 쉽습니다.
        ```cs
        int a = 10;
        int b = 20;

        if(a == b) //a가 b와 같지 않으므로 거짓
        {
            Console.Write("Hellow if!"); //a와 b가 다르기 때문에 실행되지 않는 코드
        }
        else if(a < b) //a가 b보다 작으므로 참
        {
            Console.Write("Hellow else if!"); //위의 조건식이 거짓이고 조건식이 참이기 때문에 실행되는 코드
        }
        else
        {
            Console.Write("Hellow else!"); //위의 조건식이 참이기 때문에 실행되지 않는 코드
        }
        ```
        <details>  
            <summary>출력 결과</summary>  

            Hello else if!
        </details>  
        위의 예제에서 if문에 있는 조건식이 거짓이기 때문에, if문 아래에 있는 else if문의 조건을 한번 더 검사하게 됩니다.  
        else if문에 있는 조건식이 참이기 때문에 else if문 안에 있는 코드가 실행되고, else문 안에 있는 코드는 실행되지 않습니다.  

    + ## switch문

        switch문은 여태까지 배웠던 if문에서 파생된 조건문들과는 성격이 조금 다릅니다.  

        switch문은 주로 여러개의 조건식의 결과를 검사할 때 사용됩니다.  
        >switch문은 조건식의 결과와 여러개의 값을 비교하면서 코드를 실행한다고 생각하면 됩니다.  

        아래의 코드는 switch문의 기본 형식입니다.
        ```cs
        switch(조건식)
        {
            case 비교할 값1:
                //실행할 코드 1
                break;
            case 비교할 값2:
                //실행할 코드 2
                break;
            case 비교할 값3:
                //실행할 코드 3
                break;
            default:
                //아무것도 아닐 때 실행할 코드
                break;
        }
        ```
        switch문은 `조건식의 결과`를 각각의 `case의 값`과 비교하여 `조건식의 결과`와 `case의 값`이 같으면 `break`를 만날 때 까지 적혀있는 코드를 실행합니다.  
        >break 키워드는 지금으로써는 switch문을 종료하기 위해서 사용한다고 생각하셔도 좋습니다.  
        >break 키워드를 사용하지 않으면 switch문을 빠져나갈 수 없기에 오류가 발생합니다.
          
        만약 case의 값이 `모두 조건식의 결과와 일치하지 않는다면`, default 키워드 밑에 적혀있는 `코드를 실행`합니다.  
        >default 키워드를 사용하지 않고 case만 사용해도 switch문은 정상적으로 작동`합니다.  
        ```cs
        int a = 10;
        int b = 20;

        switch(b - a)
        {
            case 0:
                Console.Write("0");
                break;
            case 10:
                Console.Write("10");
                break;
            case 20:
                Console.Write("20");
                break;
            default:
                Console.Write("Default");
                break;
        }
        ```
        <details>  
            <summary>출력 결과</summary>  

            10
        </details>  
        위의 예제에서는 조건식에 `b - a`를 넣었기 때문에 조건식은 `10`이 됩니다.  
          
        첫번째 case는 `0`이기 때문에 `10`과 같지 않습니다. 따라서 결과는 `거짓`이기 때문에 `다음 case`를 검사하게 됩니다.  
        두번째 case는 `10`으로 조건식인 `10`과 같습니다. 그러므로 밑에 있는 `코드가 실행`되어 콘솔에 `10`이 출력됩니다.  
        두번째 case에서 코드를 실행하고 `break`키워드를 만났기 때문에 `switch문을 빠져나와` 세번째 case는 `검사하지 않습니다`.  
          
        다음 장 부터는 반복문을 살펴보도록 하겠습니다.
+ # 반복문
    >복사 붙여넣기에 지친 당신에게

    반복문은 말 그대로 같은 코드를 여러번 반복시켜주는 역할을 합니다.  

    + ## while문

        while문은 반복문 중 가장 간단한 반복문 입니다.  
        ```cs
        while(조건식)
        {
            //실행할 코드
        }

        //실행할 코드
        ```
        위의 예제는 while문의 기본 형식입니다.  
        while문은 정말 단순하게 조건식이 참인 동안 코드블럭 안에 있는 코드를 반복해서 실행합니다.  
        조건식이 거짓이 되면 while문을 빠져나와 다음 코드를 실행하게 됩니다.  
          
        아래의 예제는 a가 5보다 작을동안 a의 값을 콘솔에 출력하는 예제입니다.
        ```cs
        int a = 0;

        while(a < 5)
        {
            Console.Write(a);
            a++;
        }

        Console.Write("Exit");
        ```
        <details>  
            <summary>출력 결과</summary>  

            01234Exit
        </details>  
        while문에 있는 조건식은 0이 5보다 작으니 참이고, 조건식이 참이기 때문에 while문 안으로 진입합니다.  
          
        처음 while문 안에 있는 코드가 실행되면 a에는 0이 들어가있습니다.  
        따라서 콘솔에 0이 출력된 후 a의 값이 1이 증가합니다.  
          
        코드블럭 안에 있는 코드가 모두 실행된 뒤에는 다시한번 조건식을 검사하게 됩니다.  
        다시한번 조건식이 참이기 때문에 while문 안으로 진입합니다.  
          
        두번째로 while문안에 있는 코드가 실행될 때는 첫번째 실행에서 a값을 1증가시켰기 때문에 a에 1이 들어가있습니다.  
        그러므로 콘솔에 1이 출력되고 이후 a값이 또다시 1증가합니다.

        위의 과정을 반복하며 a가 5보다 작지 않으면(같거나 크면) while문을 나오게 됩니다.  
    + ## for문
        위의 while문 예제에서 a값을 증가시키면서 조건식을 거짓으로 만들어 반복문을 벗어났습니다.  
        for문은 이러한 반복을 조금 더 편하게 해주는 반복문입니다.

        for문의 기본형식은 아래와 같습니다.
        ```cs
        for(자료형 변수명 = 초기화값; 조건식; 증감식)
        {
            //실행할 코드
        }
        ```
        이렇게 보면 이해가 쉽지 않으니 아래의 예제를 보면 좋을 것 같습니다.
        ```cs
        for(int i = 0; i < 5; i++)
        {
            Console.Write(i);
        }

        Console.Write("Exit");
        ```
        <details>  
            <summary>출력 결과</summary>  

            01234Exit
        </details>  
        눈치채신분들도 있겠지만 위의 예제는 while문의 마지막 예제를 for문으로 작성한 코드입니다.  
        
        for문을 차근차근 살펴보도록 하겠습니다.  
        
        처음에 int형식의 i 값을 0으로 초기화 하였습니다.  
        이후 반복을 돌 때마다 조건식인 i < 5의 참 거짓 여부를 확인하면서, 증감식인 i++를 실행해줍니다.  
        루프를 한번씩 돌때마다 i값이 1씩 증가했으니 5번의 반복을 들게되면 i의 값은 5로 i < 5가 거짓이 됩니다.  
        그러므로 총 5번 반복이 되고 for문을 빠져나와 마지막에는 "Exit"가 출력되게 됩니다.  
          
        그렇다면 아래 예제의 출력값은 어떻게 될까요?  
        바로 출력값을 열어보기보단 충분한 생각을 해본 후 열어보는걸 추천합니다.  
        ```cs
        for(int i = 0; i < 5; i++)
        {
            Console.Write(1);
        }

        Console.Write(1);
        ```
        <details>  
            <summary>출력 결과</summary>  

            111111
        </details>  
        위의 예제에서는 반복을 돌 때마다 변수인 i값이 아닌 리터럴 값인 1을 출력했습니다.
        따라서 for문이 5번 실행되어 1이 5번 찍힌 후 for문 밖에 있는 문장때문에 1이 한번 더 찍힙니다.  
        그래서 출력값에 1이 6번 찍히는 것입니다.  

        다음은 반복문에서 주로 사용하는 키워드에 대해서 알아보도록 합시다.  
    + ## break, continue, goto
        break, continue, goto키워드 모두 반복문을 제어할 때 사용하는 키워드입니다.

        하나하나 차근차근 알아가 보도록 하겠습니다.
        
        + ### break
            break는 언제든지 반복문을 중단시킬 수 있는 키워드 입니다.  
            switch문에서 break 키워드를 만나면 switch문을 종료한다고 설명했었습니다.  
            반복문에서도 마찬가지로 반복을 돌다가 break 키워드를 만나면 반복문을 빠져나오게 됩니다.  
            
            이해를 돕기위해 예제 하나를 보겠습니다.
            ```cs
            for(int i = 0; i < 5; i++)
            {
                if(i == 2)
                {
                    break;
                }

                Console.Write(i);
            }

            Console.Write("Exit");
            ```
            <details>  
                <summary>출력 결과</summary>  

                01Exit
            </details>  

            위의 예제는 i가 2일때 반복을 종료하고 "Exit"을 출력하는 코드입니다.    
            원래는 i가 5보다 작을때까지 반복을 돌아야 하지만, if문에서 i가 2일때 break를 해주었기 때문에 0, 1까지만 출력하고 반복을 종료하는 것입니다.

            break 다음에는 비슷하지만 얼핏 다른 continue 키워드에 대해서 알아봅시다.

        + ### continue
            break가 반복문을 즉시 종료시키는 키워드라면 continue는 continue 키워드 아래의 문장을 실행하지 않고, 다음 반복으로 넘어가는 키워드 입니다.  
              
            마찬가지로 예제를 보도록 하겠습니다.
            ```cs
            for(int i = 1; i < 5; i++)
            {
                if(i % 2 == 0)
                {
                    continue;
                }

                Console.Write(i);
            }
            ```
            <details>  
                <summary>출력 결과</summary>  

                13
            </details>  

            위의 예제는 1부터 4까지의 숫자 중 홀수만을 출력하는 예제입니다.  
            짝수일 경우 continue키워드를 만나 출력하는 코드를 실행하지 않게 됩니다.  
            그렇기에 홀수인 숫자만 출력되는 것입니다.

        + ### goto
            goto키워드는 위에서 나온 키워드들과 사용법이 많이 다릅니다.  
            또한 사용하는것을 추천하지 않는 키워드입니다.  

            우선 goto 키워드의 기본적인 형식은 아래와 같습니다.
            ```cs
            goto 레이블명;

            레이블명:
            //실행할 코드
            ```
            >여기서 레이블이란 goto키워드로 가고싶은 지점에 임의의 이름을 부여한다고 생각하시면 됩니다.

            아래의 예제는 위에서 알아본 break 키워드의 예제를 goto 키워드로 구현한 것입니다.  
            ```cs
            for(int i = 0; i < 5; i++)
            {
                if(i == 2)
                {
                    goto EXIT;
                }

                Console.Write(i);
            }

            EXIT :
            Console.Write("Exit");
            ```
            <details>  
                <summary>출력 결과</summary>  

                01Exit
            </details>  
            
            goto 키워드는 사용은 정말 편리해보이지만 코드의 흐름을 파악하기 힘들다는 큰 단점이 존재합니다.  
            때문에 goto 키워드는 사용하지 않는 것이 좋습니다.

+ # enum
    >상수를 의미있는 단어로 나타내고 싶을 때  
      
    enum을 한글로는 열거형 이라고 부릅니다.  
      
    그 말대로 enum은 열거형 상수들을 알아보기 쉽게 표현하기 위한 키워드로, 상수 숫자들을 의미있는 단어로 표현하고 싶을 때 주로 사용합니다.  
      
    enum을 사용하게 되면 일반적인 상수를 사용하는 것보다 코드의 가독성이 높아집니다.  
      
    그러면 enum을 사용하는 방법을 알아보도록 하겠습니다.  
    ```cs
    enum Color
    {
        RED,
        BLUE,
        YELLOW,
        GREEN,
    }
    ```
    위의 예제는 Color라는 enum을 정의한 예시입니다.  
    맨 위에 선언한 값인 RED는 0의 값을 갖고, 아래의 값들은 차례대로 1, 2, 3의 값을 갖게 됩니다.  
      
    ```cs
    class Program
    {
        enum Color
        {
            RED,
            BLUE,
            YELLOW = 5,
            GREEN = 10,
        }

        static void Main(string[] args)
        {
            Color color;
            
            // enum 타입에 값을 대입하는 방법
            color = Color.YELLOW;

            // enum 타입을 형변환 하는 방법
            int colorValue = (int)color; 

            if (color == Color.YELLOW) // enum 타입을 비교하는 방법
            {
                Console.WriteLine(Color.YELLOW);
            }
        }
    }
    ```
    <details>  
        <summary>출력 결과</summary>  

        YELLOW
    </details>  

    위의 예제에서 enum선언부를 보면 알 수 있듯이 원하는 값에 원하는 숫자를 할당할 수도 있습니다.  
      
    enum을 사용하려면 선언한 enum의 이름을 자료형으로 변수를 선언하는 것과 같이 사용하면 됩니다.  
      
    값을 대입하고 싶다면 `enum의 이름.값의 이름` 으로 접근하면 됩니다.  
      
    enum의 값에 숫자를 넣어놓은 만큼 int 형으로 형변환이 가능합니다.  
    >단 as 키워드는 사용할 수 없습니다.

+ # struct
    >당신이 원하는 자료형

    struct, 즉 구조체는 사용자 정의 자료형입니다.  
    int, float 등과 같이 기본적으로 제공되는 자료형이 아닌 사용자가 원하는 형식의 자료형을 만들기 위해서 사용됩니다.  
      
    아래의 예제는 Student라는 자료형을 구조체로 정의한 것 입니다.  
    ```cs
    struct Student
    {
        public string _name; //학생의 이름
        public int _number; //학생의 학번
        public int _grade; //학생의 학년
        public int _class; //학생의 반
    }      
    ```
    구조체 안에 원하는 변수를 마음껏 선언하여 사용할 수 있습니다.  
      
    아래의 예제는 위에서 선언한 구조체를 사용하는 예제입니다.
    ```cs
    class Program
    {
        struct Student
        {
            public string _name; //학생의 이름
            public int _number; //학생의 학번
            public int _grade; //학생의 학년
            public int _class; //학생의 반
        }      

        static void Main(string[] args)
        {
            Student student1, student2;

            student1._name = "남상현"; //이름은 남상현
            student1._number = 1; //번호는 1번
            student1._grade = 2; //학년은 2학년
            student1._class = 3; // 반은 3반

            student2._name = "손환주"; //이름은 손환주
            student2._number = 6; //번호는 6번
            student2._grade = 1; //학년은 1학년
            student2._class = 1; // 반은 1반

            Console.Write("이름 : " + student1._name + ", ");
            Console.Write("번호 : " + student1._number + "번, ");
            Console.Write("학년 : " + student1._grade + "학년, ");
            Console.WriteLine("반 : " + student1._class + "반");

            Console.Write("이름 : " + student2._name + ", ");
            Console.Write("번호 : " + student2._number + "번, ");
            Console.Write("학년 : " + student2._grade + "학년, ");
            Console.WriteLine("반 : " + student2._class + "반");
        }
    }
    ```
    <details>  
        <summary>출력 결과</summary>  

        이름 : 남상현, 번호 : 1번, 학년 : 2학년, 반 : 3반
        이름 : 손환주, 번호 : 6번, 학년 : 1학년, 반 : 1반
    </details>  

    구조체 안에 있는 변수에 접근할 때는 `.`을 사용합니다.  
      
    c#의 구조체에는 다음과 같은 특징들이 존재합니다.  
      
    - C# 구조체에 메소드, 필드, 속성등을 가질 수 있습니다.  
    - C# 구조체에 생성자를 정의할 수 있습니다.  
    - C# 프로그램에서 new 연산자를 이용하여 struct 객체를 생성할 수 있습니다.  
    - C# 구조체에 기본(Default) 생성자를 정의할 수 없습니다.  
    - C# 구조체에 소멸자를 정의할 수 없습니다.  
    - C# 구조체는 다른 구조체나 클래스의 기본 구조체(상속하기 위한)가 될 수 없습니다.  
      
    위에서 나온 생성자, 소멸자, 상속 등의 개념은 나중에 클래스를 배울 때 더 자세히 다룰 예정이니, 지금은 이런게 있다 정도만 알아두시면 될 것 같습니다.

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
