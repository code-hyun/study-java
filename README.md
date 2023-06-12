# 코리아 IT 아카데미 국비과정

<!-- ABOUT THE PROJECT -->
## Java
<br>

#### JAVA - 프로그래밍 언어
    프로그래밍 언어는 개발자와 컴퓨터가 소통하기 위한 언어이다.
#### 소스코드 
    명령어를 작성해 놓은 것. 
    개발자와 컴퓨터가 소통할 것을 글로 작성해 놓은 것.  
#### 컴파일
    사람의 언어를 컴퓨터 언어로 바꿔주는 작업.
#### 컴파일러
    컴파일을 해주는 프로그램 또는 명령어.
#### 컴파일러 해석 방향
    위에서 아래로 좌에서 우로 번역.
#### 콘솔
    개발자와 운영체제가 소통한 결과를 보여주는 창.
#### 프로그램
    소스코드로 잘 짜여진 틀.
    
<br>

#### ▶ 일반프로그램
    프로그램
	OS(운영체제): 하드웨어에 적절한 전기신호를 흘려주는 역할.
	하드웨어

	- 일반 프로그램은 이식성이 좋지 않다.

#### ▶ JAVA 프로그램
    프로그램
    JVM: JAVA 프로그램을 OS에 맞게 번역한다.
    OS
    하드웨어
	
	  - JAVA 프로그램은 이식성이 좋다.
-------------------------------------------------------------------------------------

JVM(Java Virtual Machine)
	JAVA 프로그램을 실행해 줌.

JRE(Java Runtime Environment)
	JVM을 생성하며, 실행할 때 필요한 라이브러리 파일들을 가지고 있다.

JDK(Java Development Kit)
	JRE외에 개발에 필요한 도구들을 가지고 있다.
	컴파일 명령어와 실행 명령어를 담고 있다.
  
-------------------------------------------------------------------------------------

기본 구조
	프로젝트
		패키지
			클래스(대문자)
				메소드(이름 뒤에 소괄호)
					소스코드
          
-------------------------------------------------------------------------------------
#### 출력 메소드
	print(): 마지막에 자동으로 줄바꿈이 되지 않고 아래의 문장과 이어서 출력된다.
	println(): 마지막에 자동으로 줄바꿈된다.
	printf()

#### 출력 메소드 목적
	전달받은 데이터 및 전달할 데이터 검사, 오류 발생 지점 구체화 및 검사
  
-------------------------------------------------------------------------------------

#### 변수 : 저장공간
	
     x	      =	    10
     저장공간의대입	 값
     이름	          연산자

#### 자료형(type, 종류)
	자료형	type	byte	값

	정수형	int	4	10, 32, 543, -32, 2147483647, ...
	실수형	float	4	10.5F, -0.9F, 0.0F, 123.4563F, ...
		double	8	10.5, -0.9, 0.0, 123.4563, ...
	문자형	char	2	'강', '일', '1', '0', '-', ...
	문자열	String	?	"0", "0.0", "1", "A", "ABC", "안녕~~~", ...

#### 변수의 선언
    type name = value;
    예)
    int x = 10;
    x라는 이름의 저장공간이 할당(allocation)되고 그 안에 10이 들어간다.


RAM(메모리)
<hr>
OS Kernel Space	- 드라이버
<hr>
Stack		- 지역변수, 매개변수
<hr>
Free
<hr>
Heap		- 동적 메모리
<hr>
BSS		- 초기화되지 않은 전역변수
<hr>
Data 영역	- 전역변수, 정적변수
<hr>
Text 영역	- 상수, 코드
<hr>

int x = 10;
x라는 이름의 저장공간이 RAM에 할당되고 10이라는 값이 들어간다.

#### 주소(해시코드)
	int x = 10;
	x라는 이름의 저장공간이 RAM에 할당되면 고유한 값인 주소값이 부여된다.
	계속 실행되거나 종료되는 프로그램이 있기 때문에, 주소값을 변경될 수 있으나
	중복은 없다.

#### 변수의 사용
	int data = 20; // 선언
	data = 30; // 선언
	System.out.print(data + 9); // 사용
	data = data + 7; // 선언, 사용
	data - 9; // 사용

#### 변수의 선언
	자료형 변수명 = 초기값; //초기화
	자료형 변수명;

#### 변수의 선언 시 주의사항
	1. 같은 이름의 변수로 선언할 수 없다.
	2. 초기화를 해준다.
	3. 되도록 선언부에 한꺼번에 선언한다(영역 상단).

#### 변수명 주의사항
	문자로 시작해야 한다.
	특수문자는 사용할 수 없다. 단, _는 허용한다.
	소문자로 시작한다.
	공백을 사용할 수 없다.
	
	goodBoy : 카멜 표기법(JAVA)
	good_boy : 파스칼 표기법, 스네이크 표기법, 팟홀 표기법, 언더바 표기법(DBMS)

	되도록 한글은 사용하지 않는다.
	명사로 사용한다.
	뜻이 있는 단어를 사용한다.
	a, b, c, d, e, ... (X)
	data, number, age, name, ...(O)

#### 변수를 사용하는 이유
	1. 반복되는 값을 쉽게 관리할 수 있다.
	2. 의미 없는 값을 하나의 정보로 만들기 위해서(자료구조).

-------------------------------------------------------------------------------------

#### 서식문자(format)
	반드시 따옴표 안에서 작성한다.
	
	%d : decimal(10진수 정수)
	%o : ocatal(8진수 정수)
	%x : hexadecimal(16진수 정수)
	%f : float(실수)
	%c : character(문자)
	%s : string(문자열)

#### 출력메소드
	printf() : 서식 문자를 사용하여 출력할 수 있으며, 자동으로 줄바꿈되지 않는다.

-------------------------------------------------------------------------------------

#### 상수
	항상 그대로인 수.
	값을 변경할 수 없도록 한다.

	final type name = value;

#### 상수를 사용하느 이유
	1. 의미 없는 값에 의미를 부여하기 위해서
	2. 오타 방지

-------------------------------------------------------------------------------------

#### 형변환
	- 자동 형변환
		정수 + 정수 = 정수
		정수 + 실수 = 실수
		3 + 0.0 = 3.0
		5 / 2 = 2
		5.0 / 2 = 2.5

		문자 + 정수 = 정수

	- 강제 형변환
		(type)value
		(double)3

#### 문자열 형변환
	1. 다른 자료형을 문자열로
		문자열과 다른 일반 자료형을 연결하면 결과는 문자열이 된다.

	2. 문자열을 다른 자료형으로
		일반 자료형은 일반 자료형끼리만 형변환이 가능하다.
		문자열 타입은 클래스 타입이므로, 일반 자료형의 클래스타입의 도움을 받아야한다.

		Integer.parseInt("")	=> 문자열에서 변환된 정수 값
		Float.parseFloat("")	=> 문자열에서 변환된 실수 값
		Double.parseDouble("")	=> 문자열에서 변환된 실수 값
		...

-------------------------------------------------------------------------------------

#### 입력
	커서가 깜빡이고 있는 상태.
	입력하기 전에 출력을 통해 어떤 값을 입력해야할지 사용자에게 알려주어야 한다.

#### 입력 클래스
	Scanner sc = new Scanner(System.in);

#### 입력 메소드
	next() : 사용자가 입력한 문자열 값
		- 사용자가 입력한 값 중 공백 또는 줄바꿈 문자를 구분점으로 각 문자열을 분리한다.
		- 첫 번째 문자열을 첫 번째 next()에 담고
		  두 번째 문자열은 두 번째 next()에 담는다.

	nextLine() : 사용자가 입력한 문자열 값
		- 공백 또는 줄바꿈 문자도 값으로 취급하기 때문에 그대로 입력받는다.

-------------------------------------------------------------------------------------

#### 연산자
	기능이 있는 특수문자

#### 연산자의 우선순위
	최우선 연산자
	단항 연산자
	산술 연산자
	쉬프트 연산자
	관계 연산자
	논리 연산자
	삼항 연산자
	대입 연산자

#### 결합성
	하나의 수식에 동일한 연산자가 여러 개 사용되면 알맞은 방향으로 결합되어 연산되는 성질

#### 비트연산
	논리 연산자
		& (AND, 논리곱), A & B, 두 비트가 모두 1이면 1
		| (OR, 논리합), A | B, 둘 중 하나라도 1이면 1
		^ (XOR, 배타논리합), A ^ B, 두 비트가 서로 달라야 1

	단항 연산자
		~ (NOT, 논리부정), ~A, 0은 1로 1은 0으로 변경, ~a = -a-1

	쉬프트 연산자
		<< (LEFT SHIFT, 좌쉬프트), A << B, A를 왼쪽으로 B만큼 비트이동
		>> (RIGHT SHIFT, 우쉬프트), A >> B, A를 오른쪽으로 B만큼 비트이동
    
----------------------------------------------------------------------------------------

#### 논리형(boolean)
	참 : true
	거짓 : false

	boolean(1byte) = true, false

#### 조건식
	결과가 참 또는 거짓, 둘 중 하나가 나오는 식.
	참 또는 거짓 값.

	관계 연산자
		==	: 같다
		!=	: 같지 않다
		>, <	: 초과, 미만
		>=, <=	: 이상, 이하

	논리 연산자
		&&, A && B, 두 조건식 모두 참이면 참
		||, A || B, 둘 중 하나라도 참이면 참

	단항 연산자
		!(NOT), !A, 조건식이 참이면 거짓으로, 거짓이면 참으로 변경
    
----------------------------------------------------------------------------------

#### 삼항 연산자( ? : ) : 값으로 봐야한다!
	조건식 ? 참 : 거짓

	int result = 10 > 9 ? 10 : 9;
	단, 참과 거짓 자리에는 값만 작성할 수 있다.

#### 삼항 연산자를 사용할 때
	조건식이 딱 한 개 있을 때에만 사용하자!

----------------------------------------------------------------------------------

#### ▶ 조건문
	▷ if문

	if(조건식){
		실행할 문장;
	}
	if(조건식){
		실행할 문장;
	}
	if(조건식){
		실행할 문장;
	}...


	if(조건식){
		실행할 문장;
	}
	else if(조건식){
		실행할 문장;
	}
	...
	}
	else {
		실행할 문장
	}

	▷ switch문	

	switch(변수명){
	case 값1:
		실행할 문장;
		break;
	case 값2:
		실행할 문장;
		break;
	case 값3:
		실행할 문장;
		break;
	case 값4:
		실행할 문장;
		break;
	...
	default:
		실행할 문장;
		break;
	}


#### ▶ 반복문



---------------------------------------------------------------------

#### 삼항 연산자, if문, switch문의 비교
	삼항 연산자: 조건식이 1개 있을 경우 사용
	if문: 조건식에 비교(>, <, >=, <=) 연산자를 사용하거나, 여러 개의 조건식을 논리 연산자(&&, ||)로 연결할 때 사용
	switch문: 하나의 변수에 여러 개의 값이 담길 수 있고, 각 값이 같은 지를 비교할 때 사용
  
---------------------------------------------------------------------------------------------------

#### 대입 연산자(복합 대입 연산자, 누적 연산자)
	+=, -=, /=, *=, %=, ...

	int money = 10000;
	//money = money - 1000;
	money -= 1000;
	System.out.print(money);

	int data = 10;
	//data = data + 1;
	//data += 1;
	data++;
	System.out.println(data);

#### 증감 연산자
	++, --

	전위형 : 해당 라인부터 바로 적용
		++data
	후위형 : 다음 라인부터 바로 적용
		data++

-------------------------------------------------------------------------------------------------
#### 반복문

▷ for문	
	int i=0;  i<10;  i=i+1
	for(초기식; 조건식; 증감식){
		실행할 문장;
	}

	1. 초기식
	------------
	2. 조건식
	3. 실행할 문장
	4. 증감식
	5. 조건식
	6. 실행할 문장
	7. 증감식
	...
	

▷ while문
	while(조건식){
		실행할 문장;
	}


for문과 while문의 목적
	- for : 몇 번 반복할 지 알 때
	- while : 몇 번 반복할 지 모를 때

▷ do~while문

	do {
		실행할 문장;
	} while(조건식);

	무조건 한 번은 실행되어야 할 때 사용한다.
  
---------------------------------------------------------------------------------------------

#### 기타 제어문
	break : 즉시 해당 중괄호 영역을 탈출한다.
		- if문 안에서 사용 시 if문을 탈출하지 않고 if문을 감싸고 있는 중괄호 영역을 탈출한다.

	continue : 즉시 다음 반복.
		- 아래의 코드를 실행하지 않기 위해서 사용한다.
    
---------------------------------------------------------------------------------------------

#### 배열 : 저장공간의 나열

	1.
		변수를 여러 개 선언하면 이름도 여러 개 생긴다. 이 때 각 저장공간을 관리하기가 불편하다.
		따라서 n칸 배열을 한 번만 선언하면 저장공간도 n개 생기고, 이름도 한 개이기 때문에 관리하기 편하다.

	2.
		규칙성이 없는 값에 규칙성을 부여하기 위해서


#### 배열의 선언
	자료형[] 배열명 = {값1, 값2, ...}; // 어떤 값을 넣을 지 알 때 사용
	자료형[] 배열명 = new 자료형[칸수]; // 어떤 값을 넣을 지는 모르나, 몇 칸 만들지는 알 때 사용
	자료형[] 배열명 = null; // 어떤 값을 넣을지도 모르고, 몇 칸 만들지도 모를 때 사용한다.
	배열명 = new 자료형[칸수];

	※ new: Heap 메모리에 할당, 초기값으로 자동 초기화
	※ null: 주소의 초기값, 어떤 주소를 넣을 지 모를 때 작성하는 초기값
	※ 자바에서 배열은 항상 Heap(동적 메모리)에 할당되기 때문에 메모리 상으로는 동적배열만 존재한다.

#### 배열의 구조
	int[] arData = {3, 5, 1, 2, 8};

	arData라는 이름의 저장공간은 한 개 만들어지며, 여기에는 한 개의 값만 담을 수 있다.
	5개의 값을 담기 위해서는 5칸이 필요하며, 이는 Heap 메모리에 할당된다. 5칸의 저장공간 중
	첫 번째 저장공간의 주소값이 arData 저장공간으로 들어가며, 다음 주소에 접근하기 위해서는
	+ n을 한다. 예를 들어 arData + 2는 1이라는 값이 담긴 주소값이 되며,
	*(arData + 2)는 해당 주소에 가서 읽어온 1이라는 값이 된다. JAVA에서는 직접 주소에 접근하는
	연산자가 없기 때문에 위와 같은 식을 []로 치환하여 사용하며, arData[2]로 사용한다.
	각각의 방 번호는 index라고 부르며, 배열은 시작주소를 가지고 있기 때문에 인덱스 번호는 항상 0부터 시작된다.

#### length
	배열을 선언하면 length라는 상수가 선언되고, 해당 배열의 길이가 담긴다.
	배열명.length로 사용하게 된다.

#### 배열의 사용
	int[] arData = new int[5]; // 선언
	arData[0] = 10; // 선언
	arData[0] + 9; // 사용
	System.out.println(arData); // 주소값
	arData[2] = arData[0] + arData[1]; // 선언, 사용
	System.out.println(arData[5]); // 오류
  
------------------------------------------------------------------------------------------------

#### 2차원 배열 : 배열 안에 배열
	
	1차원 배열을 여러 개 선언할 때 관리하기 힘들기 때문에
	2차원 배열을 한 번 선언한다.
	
	※ 2차원 배열부터는 메모리 낭비가 심하므로 선호하지 않는다.

#### 2차원 배열 선언
	자료형[][] 배열명 = {{값1, 값2, 값3,...}, {값4, 값5, 값6,...}};
	자료형[][] 배열명 = new 자료형[행][열];
	자료형[][] 배열명 = null;


	int[][] arrData = new int[2][3];

	□	arrData		arrData.length(행의 길이)
	□□	arrData[행]	arrData[행].length(열의 길이)
     □□□ □□□	arrData[행][열]
--------------------------------------------------------------------------------


---------------------------------------------------------------------


#### 메소드
	이름 뒤에 소괄호.
	단, 키워드 뒤에 소괄호는 메소드가 아니다.

	f 	(x) = 2x + 1
       ---	---   ------	
      메소드명	매개   리턴값
		변수

##### 메소드 선언
	(1)리턴타입 (2)메소드명(자료형 (3)매개변수명, ...){
		(4)실행할 문장;
		(5)return 리턴값;
	}

	(1) 리턴 값이 있다면 리턴 값의 자료형을 작성하고, 리턴 값이 없다면 비워놓지 않고 void를 작성한다.
	(2) 동사로 작성한다(연필(매개변수)을 쓴다(메소드)).
	(3) 외부에서 전달받을 값이 있다면, 자료형과 순서에 맞게 선언해준다.
	    생략 시, 외부에서 값을 전달받을 수 없게 된다.
	(4) 생략이 가능하다. 메소드의 기능을 구현하는 로직을 작성한다.
	(5) 생략이 가능하다. 리턴값이 있다면, 사용한 부분 통채로를 리턴값으로 봐야한다.

##### 메소드 선언 순서
	문제) 두 정수의 덧셈 메소드 선언

	1. 메소드의 이름을 생각한다.
		add(){}

	2. 매개변수를 생각한다.
		add(int num1, int num2){}

	3. 실행할 문장을 생각한다.
		add(int num1, int num2){
			int result = num1 + num2;
		}

	4. 리턴값을 생각한다.
		add(int num1, int num2){
			int result = num1 + num2;
			return result;
		}		

	5. 리턴타입을 결정한다.
		int add(int num1, int num2){
			int result = num1 + num2;
			return result;
		}		

##### 메소드 주의사항
	메소드를 선언할 때에는 {}(중괄호)가 있으며, 반드시 메소드 밖에서 선언한다.
	메소드를 사용할 때에는 {}(중괄호)가 없으며, 반드시 메소드 안에서 사용한다.

##### 메소드 사용
	메소드의 리턴 타입이 void라면 실행 메소드이므로 값으로 봐서는 절대 안된다.
	메소드의 리턴 타입이 void가 아니라면 사용한 부분 통채로가 리턴값이다.


##### 메소드 목적
	1. 재사용(특정성을 부여해서는 안된다).
	2. 소스코드 간결화

##### 리턴해야 할 때
	사용한 쪽에 로직의 결과를 전달해야 할 때.

##### 리턴하면 안될 때
	사용한 쪽에 로직의 결과를 전달할 필요가 없을 때.








---------------------------------------------------------------------

#### 클래스(반)
	공통요소를 한 번만 선언해놓고 가져다 사용만 하도록 설계한다.

	1. 타입이다.
		클래스 안에 선언된 변수와 메소드를 사용하고 싶다면,
		해당 클래스 타입으로 객체를 선언해야 한다.

	2. 주어이다.
		원숭이가 먹는다 바나나를.
		Monkey.eat("바나나");

#### 클래스 선언
	class 클래스명 {
		필드(변수, 메소드);
	}

#### 클래스의 필드 사용
	1. 객체화(instance): 객체(instance variable)를 만드는 작업, 추상적인 개념을 구체화시키는 작업.	
		클래스명 객체명 = new 생성자();
		객체명.필드명
		※ .(마침표): 하위 연산자, 멤버변수 접근 연산자, 닷 연산자, 점 연산자
			    주소값 뒤에서만 사용이 가능하며 해당 주소를 참조하는 명령어이다.
	2.

#### 생성자
	클래스 이름 뒤에 소괄호가 있는 형태, 메소드와 기능이 똑같지만 메소드라고 부르지 않는다.
	생성자는 리턴이라는 기능이 존재하지 않기 때문이다.

	1. 해당 클래스의 필드를 메모리에 할당한 후 부여된 주소값을 가져온다.
	2. 초기화

#### 기본 생성자
	매개변수가 없는 생성자이며, 클래스 선언 시 자동으로 선언된다.
	사용자가 직접 생성자를 선언하게 되면 기본 생성자는 없어진다.

#### this
	필드에 접근한 객체가 누구인지 알아야 해당 필드에 접근할 수 있다.
	이 때 접근한 객체가 가지고 있는 필드의 주소값을 this라는 변수에 자동으로 담긴다.
  
----------------------------------------------------------------------------------------------

#### Storage class(저장 기억 부류)

		Stack		Data영역
		지역변수, 매개변수	전역변수, 정적변수(static)

1. 초기화		직접		자동	
2. 생명주기	}		new, 프로그램 종료 시

static
	모든 객체가 공유해야 할 때 사용한다.
  
--------------------------------------------------------------------------------------------

#### 다형성(polymorphism)
	1. 오버로딩(Overloading)
		매개변수의 개수 또는 타입이 다르면 동일한 이름의 메소드로 선언할 수 있다.
	2.
  
-----------------------------------------------------------------------------------------------

#### 클래스 심화 실습
	- 주제: 원하는 직업을 클래스로 선언
	- 반드시 수익 창출이 되어야 한다.
	- 확률을 추가한다.
	- 구현에 필요한 필드는 얼마든지 추가 선언이 가능하다.
		예) 승진, 티어 승급, 연속 5회 성공 시 레벨 업 등


---------------------------------------------------------------------------------------------
#### 상속(inheritance)
	1. 기존에 선언된 클래스의 필드를 새롭게 만들 클래스의 필드로 사용하고자 할 때
	2. 여러 클래스 선언 시 필드가 겹칠 때 부모 클래스를 먼저 선언하고 공통 필드를 묶어서
	   자식 클래스들에게 상속해준다.

#### 상속 문법
	class A {
		A 필드
	}

	class B extends A{
		A, B 필드
	}

A: 부모 클래스, 상위 클래스, 슈퍼 클래스, 기반 클래스
B: 자식 클래스, 하위 클래스, 서브 클래스, 파생 클래스

super() : 부모 생성자
	자식 클래스 타입의 객체로 부모필드에 접근할 수 있다.
	하지만 자식 생성자만 호출하기 때문에, 자식 필드만 메모리에 할당된다고 생각할 수 있다.
	사실 자식 생성자에는 항상 부모 생성자를 호출하기 때문에 자식 생성자 호출 시 부모와 자식 필드 모두
	메모리에 할당된다. 이 때 부모 생성자를 호출하는 방법은 super()를 사용하는 것이다.
	만약, super()를 작성하지 않더라도 컴파일러가 자동으로 작성해준다.

다형성(polymorphism)
	1. 오버로딩
	2. 오버라이딩(재정의)
		부모 필드에서 선언한 메소드를 자식 필드에서 수정하고자 할 때 재정의를 해야 한다.
		이는 자식에서 부모 필드의 메소드와 동일한 이름으로 선언하는 것이다.
		부모 필드가 메모리에 먼저 할당되고 a라는 메소드가 먼저 올라간다고 하면,
		자식 필드가 메모리에 할당되면서 재정의한 a메소드가 새롭게 만들어지는 것이 아니라
		기존에 할당된 a메소드 저장공간에 새롭게 재정의한 자식 필드의 소스코드 주소가 들어가게 된다.
		따라서 자식 객체로 a메소드에 접근하면 자식 필드에서 재정의한 소스코드의 내용이 읽히게 된다.
-------------------------------------------------------------------------------------------------
#### 접근 권한 제어자(접근자)
	default: 다른 패키지에서 접근 불가
	public: 모든 곳에서 접근 가능, 해당 파일의 메인 클래스일 경우만 사용 가능
	protected: 다른 패키지에서 접근 불가, 자식은 가능
	private: 다른 클래스에서 접근 불가, 메소드(getter, setter)로만 접근하자!

-------------------------------------------------------------------------------------------------
※ 모든 자식은 부모타입이다.

#### Casting
	1. up casting : 자식 값을 부모타입으로 형변환
	2. down casting : up casting된 객체를 자식타입으로 형변환
	※ 부모 값을 자식 타입으로 형변환 시 오류

#### Casting을 사용하는 이유
	모든 자식 값을 전달받기 위해서는 동일한 타입의 저장공간으로 받아야 한다.
	하지만 자식끼리는 서로 타입이 다르기 때문에 한 번에 전달받을 수가 없다.
	이 때 up casting을 사용하면, 모든 자식이 부모 타입이므로 하나의 저장공간에
	모든 자식을 받을 수 있게 된다.
	만약 up casting으로 자식 값을 전달받았다면, 자식에서 새롭게 구현한 기능들은 사용할 수 없기 때문에
	down casting을 통해서 복구하여 사용한다.

#### instanceof(객체 간 타입 비교)
	a instanceof A : 조건식

	- a가 A타입이면 true
	- a가 A타입이 아니라면 false



---------------------------------------------------------------------

#### 추상 클래스
	필드 안에 구현이 안된 메소드가 선언되어 있는 클래스를 추상 클래스라고 한다.
	이 때 구현되지 않은 메소드를 추상 메소드라고 부른다.
	반드시 재정의를 통해 구현을 해야지만 메모리에 할당되기 때문에
	"강제성"을 부여하기 위해서 추상 메소드로 선언한다.

#### 추상 클래스 선언
	abstract class 클래스명 {
		abstract 리턴타입 메소드명(매개변수, ...);
		일반 메소드 선언가능.
	}
  
---------------------------------------------------------------------

#### 인터페이스(interface) : 틀
	추상 클래스를 고도화시킨 문법.
	상수와 추상메소드만 존재한다.
	구현은 지정한 클래스에서 진행하고, 인터페이스를
	다른 클래스에 지정할 때에는 implements 키워드를 사용한다.
	
#### 추상 클래스와 인터페이스 간의 관계
	인터페이스를 클래스에 바로 지정하면 모든 메소드에 강제성이 부여되어서
	전부 다 구현해야 한다. 하지만 일반적인 상황에서는 모든 것이 아닌,
	필요한 메소드를 골라서 재정의해야한다.
	인터페이스를 직접 지정하지 않고 다른 클래스에 지정한 후 바디를 만들어 놓는다면,
	강제성이 소멸되고 이 클래스를 상속받아서 필드를 구현한다면, 골라서 재정의할 수 있게 된다.
	이 때 중간에서 강제성을 없애주는 클래스를 추상클래스로 선언하기로 하며,
	추상클래스 이름 뒤에는 Adapter를 붙여서 목적을 알려준다.
  
--------------------------------------------------------------------------------------

#### 마커 인터페이스(Marker Interface)
	클래스들을 그룹화하기 위한 목적으로 사용한다.
	인터페이스는 지정한 클래스의 부모이며, 모든 자식은 부모의 타입이므로
	마커 인터페이스를 지정받은 클래스들이 하나의 타입으로 묶이게 된다.
	이름 뒤에 Marker를 붙여줘야 한다.
  
--------------------------------------------------------------------------------------

#### 내부 클래스(Inner Class)
	하나의 클래스에서 a작업과 b작업이 있을 때에는 따로 분리하여 클래스로 만들지 않고,
	클래스 안에 클래스를 선언하여 설계한다. 이 때 밖에 있는 클래스를 외부 클래스라고 하며,
	안에 선언된 클래스를 내부 클래스라고 한다. 외부 클래스가 메모리에 할당되어야
	내부 클래스를 객체화할 수 있기 때문에 클래스를 숨기기 위해서 내부 클래스를 사용하기도 하며,
	이를 캡슐화 또는 은닉화라고 한다. 내부 클래스는 외부 클래스의 필드이기 때문에
	외부 클래스의 필드를 자신의 필드처럼 가져다 사용할 수 있지만 상속관계가 아니기 때문에
	내부 클래스일지라도 extends를 통해 다른 클래스를 상속받아서 사용할 수 있다.

#### 익명 클래스(Anonymous Inner Class)
	이름이 없는 클래스이며 구현되지 않은 필드를 구현하기 위해 일회성으로 생성되는 클래스이다.
  
----------------------------------------------------------------------------------------

#### 심화 실습(클래스 ~ 익명 클래스)

- 스타벅스 본사 클래스 선언(register(Form form))
- 본사 제출 양식 인터페이스 선언(Form)
- 건물 클래스 선언(main 메소드)

스타벅스 지점 오픈 시 본사에 양식을 작성하여 제출
- 제출 양식에는 메뉴판(getMenu())과 판매 방식(sell(String menu))을 작성한다.
- 강남점은 메뉴 그대로 판매할 수 있어야 하고, 잠실점은 무료 나눔 행사중이다.
- 무료 나눔 행사중인 지점은 판매 방식이 따로 없다.

나이키 본사 클래스 선언
- 나머지는 위와 동일(잠실 정상, 강남 무료 나눔)

-----------------------------------------------------------------------------------------

#### 다중 상속
	여러 부모 클래스를 상속하는 것을 다중 상속이라고 한다.
	JAVA는 모호성 때문에 다중 상속을 지원하지 않는다.
	하지만 JDK8버전부터는 인터페이스에 default메소드를 선언할 수 있으며,
	여러 개를 지정할 수 있는 인터페이스 특성상 다중 상속을 지원하는 것이나 다름이 없다.

#### 모호성(ambiguity)
	하나의 자식이 여러 부모를 상속받을 때 부모 필드에 동일한 이름의 필드가 있다면,
	어떤 부모의 필드인지 알 수가 없다. 이를 모호성이라고 부른다.

#### 모호성 해결 방법
- 상황1: 두 개의 인터페이스 내에 이름과 매개변수가 똑같은 메소드가 선언되어 있다.
- 해결1: 자식 클래스에서 재정의하여 사용한다. 
        원하는 부모의 필드에 접근하기 위해서는 재정의된 메소드에서 "부모명.super.필드명"을 작성한다.

- 상황2: 부모 클래스의 메소드와 인터페이스의 디폴트 메소드의 이름과 매개변수가 똑같이 선언되어 있다.
- 해결2: 부모 클래스의 메소드가 사용된다.

----------------------------------------------------------------------------------------

#### 함수형 인터페이스(Functional interface)
	인터페이스 중 추상 메소드를 하나만 가지고 있는 인터페이스를 함수형 인터페이스라고 한다.
	이 때 @FunctionalInterface를 인터페이스 위에 작성하여 단 하나의 추상 메소드만
	선언할 수 있도록 제한해야 한다.

#### 람다식(Lambda Expression)
	이름이 없는 메소드로서 값처럼 사용이 가능하며, 매개변수로도 전달이 가능하다.
	함수형 인터페이스는 추상 메소드가 한 개만 선언되기 때문에 메소드 이름이 필요 없다.
	따라서 람다식을 익명 메소드(Anonymous Method)라고도 부른다.

#### 람다식 문법
	1. (매개변수 형식 나열, ...) -> 리턴값;
	2. (매개변수 형식 나열, ...) -> { 2개 이상의 문장 작성; return 리턴값;}
	3. 소괄호 전부 생략 가능


---------------------------------------------------------------------

#### 예외 처리
	컴파일 시, 빌드 시, 런타임 시 오류가 발생하면
	이를 제어문으로 막을 수 있으나, 제어문으로도 막을 수 없는
	오류들을 직접 처리할 수 있어야 한다.

#### 예외 처리 문법
	try {
		예외가 발생할 수 있는 문장

	} catch(예외이름 객체명){
		예외 발생 시 실행할 문장

	} catch(예외이름 객체명){
		예외 발생 시 실행할 문장

	} ...

	} finally {
		예외 발생 여부에 상관없이 무조건 실행할 문장
		※ 외부 장치와 연결했을 경우 다시 닫을 때 주로 사용한다.
	}

#### 예외 발생
	직접 예외를 발생시키기 위해서는 예외 던지기를 사용해야 하며, 이 때에는 생성자 호출 전 throw 키워드를 사용한다.
	예) throw new BadWordException();

#### 사용자 정의 예외
	기본적으로 제공되는 예외가 아닌 특정 상황에서 직접 예외를 만들어야 한다면, Exception 혹은
	RuntimeException을 상속받아서 예외 클래스를 선언해야 한다.
	Exception은 컴파일러가 체크를 하기 때문에 예외처리를 강제로 해야하고,
	RuntimeException은 컴파일러가 체크하지 않기 때문에 예외처리를 선택할 수 있다.
------------------------------------------------------------------------------------------------
#### API(Apllication Programming Interface)
	개발에 필요한 라이브러리들의 집합.
	선배 개발자들이 만들어 놓은 소스코드.

	- 내부 API
		JDK 설치 시 제공해주는 기본 API
		docs.oracle.com/javase

	- 외부 API
		선배 개발자들이 개발한 패키지 및 클래스들을 의미한다.
		보통 JAR파일로 배포하며 자바 프로젝트의 build path에 추가하여 사용할 수 있다.

#### JAR 파일로 배포하기
	배포할 클래스 또는 패키지 우클릭
	> Export > JAVA/JAR file 선택 > Next
	> destination을 원하는 경로로 선택
	> Export Java source files... 체크
	> Finish

#### JAR 파일을 프로젝트에 추가하기
	배포된 JAR파일을 다운 받기
	> 프로젝트 우클릭 > Build Path > Configure Build Path
	> Libraries 탭 클릭 > ClassPath(안되면 ModulePath) 클릭 > Add External JARs
	> 저장된 경로의 .jar파일을 더블 클릭으로 추가 > Apply 클릭
	> Orders and Exports 탭 클릭
	> Select All 클릭 > Apply and Close
  
----------------------------------------------------------------------------------------------

#### Object 클래스
	1. toString()
		항상 객체명을 출력할 때에는 toString()을 붙여서 출력해준다.
		따라서 객체명만 출력메소드에 전달하더라도 toString() 문자열 값이 출력된다.
		기본적으로 Object에서는 소속과 필드 주소를 문자열로 리턴해주지만,
		실사용에서는 불필요한 정보이기 때문에, 재정의한 뒤 필드의 정보를 확인하도록 구현한다.
		실무에서는 클래스 선언 시 각 필드의 초기화 여부를 확인하기 위해 toString()을 재정의하여 사용한다.

	2. equals()
		주소값 비교(==)
		String 클래스에서 equals()를 값 비교로 재정의하여 사용하기 때문에
		문자열 비교는 무조건 equals()로 비교한다.
		
	3. hashCode()
		JVM에서 관리하는 중복 없는 값. 실제 메모리에 할당되는 주소와 다르다.
		String 클래스에서는 필드의 해시코드 값이 아닌 문자열 상수값의 해시코드 값을
		리턴하도록 재정의하였다.
		※ 컬렉션 프레임워크 챕터에서 재정의 목적을 이해하도록 한다.
------------------------------------------------------------------------------------------------
#### Wrapper Class: 기본 자료형들의 클래스 타입
	클래스타입 객체 = new 클래스타입(일반타입의 값); //boxing, 권장하지 않는다(Deprecated).
	클래스타입 객체 = 클래스타입.valueOf(일반타입의 값); //boxing
	일반타입 변수 = 객체.000Value(); //unboxing

	JDK4버전 이상부터는 auto를 지원한다.

	클래스타입 객체 = 일반타입의 값; //auto boxing;
	일반타입 변수 = 객체; //auto unboxing;
-------------------------------------------------------------------------------------

#### 알고리즘
	어떤 문제가 발생되었을 때 해결할 수 있는 절차 혹은 순서.

#### 자료구조
	의미 없는 데이터를 하나의 정보로 만들어주는 알고리즘들의 집합.
	수집한 자료를 저장하는 방법.

#### 컬렉션 프레임워크(Collection Framework)
	많은 데이터를 쉽고 효과적으로 관리할 수 있는 표준화된 방법을 제공하는 클래스들의 집합.

##### 1. List extends Collection
	- Vector: 용량 관리, 보안성 강화, 처리량 감소
	- LinkedList: FILO로 인해 넣을 때는 빨라도 원하는 위치의 데이터를 가져오는 것이 상대적으로 느리다.
	- ArrayList: 인덱스로 데이터를 관리한다. 컬렉션 클래스 중 실무에서 가장 많이 사용되는 클래스이다.
		     배열의 특징인 인덱스를 이용하여 값을 저장하고 관리한다.

	※ 배열과 ArrayList의 차이
		배열은 길이에 제한을 두어야할 때 자주 사용되고,
		ArrayList는 몇 개의 데이터가 들어올 지 알 수 없을 때 사용한다.
    

----------------------------------------------------------------------------------------

##### 2. Set extends Collection
- 구현 클래스
	HashSet
		집합에서는 중복되는 원소를 포함할 수 없는 것 처럼
		HashSet이라는 자료구조는 중복되는 값을 무시한다.
		저장된 값들은 인덱스가 없기 때문에 순서가 없다.
		값의 유무 검사에 특화되어 있는 자료구조이고
		해시코드로 유무 검사가 진행되기 때문에 속도가 상대적으로 좋다.

- 순서 부여
	iterator()
	순서가 없는 객체에 순서를 부여하거나, 순서가 있어도 iterator방식의 순서로
	변경하고자 할 때 사용한다.
	hasNext()를 통해 다음 값이 있는 지 검사하고, next()를 사용해서 값을 가져온다.
  
----------------------------------------------------------------------------------------

##### 3. Map

- 구현 클래스
	HashMap(서버 간 데이터 교환)
		Key와 Value 한 쌍으로 저장되며, 검색의 목적을 가지고 있다.
		Key에 중복된 값을 중복된 값을 넣으면 Value가 최근 값으로 수정되고
		중복되지 않은 값을 넣으면 새롭게 추가된다. Value는 중복이 가능하다.

---------------------------------------------------------------------
#### 쓰레드

프로그램
	실행되지 않은 상태.

프로세스
	실행된 프로그램.

쓰레드
	프로세스 처리 경로.

	- 단일 쓰레드
		처리 경로를 한 개만 가지고 있기 때문에 직렬적이다.
		동시에 많은 양을 처리하기 힘들기 때문에 상대적으로 비효율적이다.
		하지만 하나의 작업에 문제가 발생하더라도 다른 작업에는 영향을 끼치지 않는다.
		따라서 안정성이 보장되고 설계 시 멀티 쓰레드에 비해 쉽다.

	- 멀티 쓰레드
		하나의 프로세스를 동시에 처리하는 것처럼 보이지만 사실은 매우 짧은 단위로 분할해서 차례로 처리한다.
		여러 개의 처리 경로를 가질 수 있도록 하며, 동시 작업이 가능해진다.
		설계하기 굉장히 어려우며, 하나의 쓰레드 문제 발생 시 모든 쓰레드에 문제가 발생하게 된다.
		JAVA 웹 서버가 대표적인 멀티 쓰레드이다. 멀티 쓰레드로 설계했다면, 처리량 증가, 효율성 증가,
		처리비용 감소의 장점이 있기 때문에 단점을 감수하고 설계하는 편이다.

멀티 쓰레드 구현 방법
	핵심 : run() 메소드 재정의

	1. Thread 클래스 상속
	2. Runnable 인터페이스 지정
-----------------------------------------------------------------------------------------
[실습]
동석이네 동물원에는 3마리의 동물이 있다.
각 동물은 울음 소리가 다르고 2마리의 동물은 동시에 운다.
나머지 1마리 동물은 2마리 동물이 모두 울고 나서 마지막에 운다.

package명은 threadTask으로 만들고 클래스는 2개만 선언한다.
하나의 클래스에는 main 쓰레드가 있다.
Runnable 인터페이스로 멀티 쓰레드를 구현하고 반드시 join()을 사용한다.
※ 각 동물은 10번씩만 운다.


- 주석을 작성하였는가
- Thread의 name필드를 사용할 수 있는가
- 배열을 사용하였는가
- 클래스를 두 개 선언하였는가
- 가산점 : 람다식을 사용하였는가, main 쓰레드를 사용하였는가


---------------------------------------------------------------------

#### 동기화(Synchronized)
   하나의 쓰레드가 자원에 접근 중일 때 다른 쓰레드가 동시에 같은 자원을 접근하지 못하게 막는 것.
   즉, 자원 공유 문제를 해결할 수 있다.
   각 쓰레드를 제어해야 할 때에도 자주 사용된다.

##### 동기화 문법
   - 블럭: synchronized(mutex) {...}

   - 키워드: synchronized
      영역 전체에 동기화를 걸어주며, 메소드 리턴 타입 앞에 작성하면
      해당 메소드 전체에 동기화가 걸린다.

##### Thread 종료 방법
   1. 필드에 boolean 타입의 변수를 선언하고 run()안에 있는 반복문에 해당 변수가 true일 경우 break 하도록 설계한다.
   2. sleep() 또는 wait(), join() 등의 메소드를 통해 쓰레드 일시정지 상태일 경우
       Thread객체.interrupt()를 사용하여 InterruptedException을 발생시킨다.
       이 때 일시정지 시킨 메소드 부분의 catch를 통해 예외를 잡아주고 원하는 문장을 작성하면 된다.
   3. 쓰레드를 일시정지하는 코드가 없을 경우 Thread.interrupted()의 상태를 확인한다.
       Thread객체.interrupt() 사용 시 Thread.interrupted()의 상태는 true로 변경된다.
            권장하지 않는 방법이다.
   4. System.exit(0)를 사용하면 전체 쓰레드 종료(프로세스 종료)

---------------------------------------------------------------------
#### 파일 입출력( Java Application 관점 )
	Stream 이라는 연결통로를 통해 원본 데이터가 알맞는 인코딩 방식으로 전송된다.
	byte단위로 입출력되기 때문에 개별처리이며, 상세 연산이 필요하지 않다면 Buffer를 사용한 입출력을 권장한다. Buffer를 사용하면 일괄처리가 가능해진다.
	Stream -> 용량이 큰거
	Buffer -> 용량이 작은거

※ 인코딩 방식	
	인코딩 방식은 완성형과 조합형이 있다.
	- 완성형 : 각, 간, 갈, 감, ...., 갛 ...
	- 조합형 : ㄱ + ㅏ + ㄱ
	
조합형이 효율적이며 byte 단위로 데이터를 전송할 때 고정된 byte가 아니기 때문에 가변형 인코딩 방식을 선호한다. 조합형이면서 가변형인 인코딩 방식은 UTF-8이며, 전 세계에서 가장 많이 사용되는 방식이다.


##### writer (출력) 
	BufferWriter : 버퍼를 사용한 출력 클래스
	FileWriter : 전달한 경로의 파일을 출력하기 위한 목적으로 열어준다.
	전달한 경로에 파일이 없다면 새롭게 만든 후 열어준다.
	객체화를 하면 파일이 열린다.


##### Reader (입력)
	BufferedReader : 버퍼를 사용한 입력 클래스
	FileReader : 전달한 경로의 파일을 입력하기 위한 목적으로 열어준다.
	전달한 경로에 파일이 없다면 FileNotFoundException이 발생한다.

##### File (파일 정보)
	전달한 경로에 있는 파일의 정보를 담는 타입.
	디렉터리 생성, 해당 경로의 전체 파일 목록, 파일 삭제 등

=============================================

#### 소프트웨어 디자인 설계 패턴

##### ▶ MVC
   M(Model): DB에서 조회된 결과 값을 담기 위한 변수들이 선언된 클래스
        - 클래스명 뒤에 VO, DTO라는 문자열을 붙여준다.
        - VO(Value Object): 테이블을 보고 그대로 만든 객체
        - DTO(Data Transfer Object): 화면에 필요한 데이터를 담은 객체
	-domain


   V(View): 사용자에게 보여질 화면을 구성하는 부분

   C(Controller): DB에 접근할 수 있는 메소드들이 선언된 클래스
         - 접근 후 결과 값이 있을 경우 Model 객체에 담은 후 처리
         - 클래스명 뒤에 DAO라는 문자열을 붙여준다.
         - DAO(Data Access Obejct)






### Built With

This section should list any major frameworks/libraries used to bootstrap your project. Leave any add-ons/plugins for the acknowledgements section. Here are a few examples.

* [![Next][Next.js]][Next-url]
* [![React][React.js]][React-url]
* [![Vue][Vue.js]][Vue-url]
* [![Angular][Angular.io]][Angular-url]
* [![Svelte][Svelte.dev]][Svelte-url]
* [![Laravel][Laravel.com]][Laravel-url]
* [![Bootstrap][Bootstrap.com]][Bootstrap-url]
* [![JQuery][JQuery.com]][JQuery-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Prerequisites

This is an example of how to list things you need to use the software and how to install them.
* npm
  ```sh
  npm install npm@latest -g
  ```

### Installation

_Below is an example of how you can instruct your audience on installing and setting up your app. This template doesn't rely on any external dependencies or services._

1. Get a free API Key at [https://example.com](https://example.com)
2. Clone the repo
   ```sh
   git clone https://github.com/your_username_/Project-Name.git
   ```
3. Install NPM packages
   ```sh
   npm install
   ```
4. Enter your API in `config.js`
   ```js
   const API_KEY = 'ENTER YOUR API';
   ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources.

_For more examples, please refer to the [Documentation](https://example.com)_

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

- [x] Add Changelog
- [x] Add back to top links
- [ ] Add Additional Templates w/ Examples
- [ ] Add "components" document to easily copy & paste sections of the readme
- [ ] Multi-language Support
    - [ ] Chinese
    - [ ] Spanish

See the [open issues](https://github.com/othneildrew/Best-README-Template/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Your Name - [@your_twitter](https://twitter.com/your_username) - email@example.com

Project Link: [https://github.com/your_username/repo_name](https://github.com/your_username/repo_name)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

Use this space to list resources you find helpful and would like to give credit to. I've included a few of my favorites to kick things off!

* [Choose an Open Source License](https://choosealicense.com)
* [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
* [Malven's Flexbox Cheatsheet](https://flexbox.malven.co/)
* [Malven's Grid Cheatsheet](https://grid.malven.co/)
* [Img Shields](https://shields.io)
* [GitHub Pages](https://pages.github.com)
* [Font Awesome](https://fontawesome.com)
* [React Icons](https://react-icons.github.io/react-icons/search)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: images/screenshot.png
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com 
