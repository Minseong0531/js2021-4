# 연민성 [201840216]
## [04월 13일]

익명 함수

함수가 코드의 집합이라는 의미는 중괄호 내부에 넣는다.
함수는 중괄호ㅓ 내부에 코드를 넣어 코드를 하나의 덩어리로 만들 수 있음.

선언적 함수

익명 함수와 마찬가지로 중괄호 내부에 코드를 넣는다.
이렇게 만든 코드 덩어리는 함수 뒤에 괄호를 붙여 호출한다.

함수의 기본형태

function 함수이름 (매개변수) {
	함수코드
	리턴 리턴값

}

함수 매개 변수 초기화

자바스크립트는 매개 변수를 입력하지 않아도 함수가 호출됨

콜백 함수

자바스크립트는 함수를 변수에 저장할 수 있어 함수의 매개 변수로 전달 가능
이 때 함수의 매개 변수로 전달되는 함수를 '콜백 함수' 라고 한다.

표준 내장 함수

자바스크립트는 기본적으로 몇 가지 필요한 함수를 지원한다.

숫자 변환 함수 
parselnt, parseFloat
문자열 > 숫자

타이머 함수
setTimeout
setlnterval
특정 시간 후에 or 특정 시간 마다

clearinterval
특정 시간마다 실행하던 함수 호출 정지



## [04월 06일]
<h2>배열</h2>

- 여러 개의 자료를 한꺼번에 다룰 수 있는 자료형

- let 이름 = [ 자료, 자료, 자료, 자료, 자료]

- 배열[인덱스]

for 반복문 기본

1. 초기식을 비교
2. 조건식을 비교 조건이 false이면 반복문을 종료한다.
3. 문장을 실행
4. 종결식 이행
5. 2단계로 이동

1~100까지 덧셈하는 코딩

>// 변수를 선언
let output = 0;
// 반복 수행
for (let i = 0; i<= 100; i++){
	output +=i;
}
//출력
console.out(output);

=> 5050이 나온다.

역 for 반복문
>let foo = [1, 2, 3, 4, 5, 6];
for (let i = foo.length; i>=0; i--){
    console.log(foo[i]);
}


=>  
6
5
4
3
2
1

직각 삼각형 만들기 for문

>let output = "";
for(let i = 0; i < 10; i++){
    for(let j = 0; j <i + 1; j++ ){
        output +="*";
    }
    output += '\n';
}
console.log(output);

break 키워드

break 키워드는 조건문이나 반복문을 벗어날 때 사용한다.

반복문이 항상 참이므로 무한 반복할때 내부에서 break를 사용해서 벗어난다.

contunue 키워드

반복문 내부에서 현재 반복을 멈추고 다음 반복을 진행하게 한다.

20

## [03월 30일]

중첩 조건문

>if else 조건문 기본형태
>if (< 불 표현식>){
>	//불 표현식이 참일 때 실행할 문장
>} else {
>	// 불 표현식이 거짓일 때 실행할 문장
>}


if else if 조건문
- 중복되지 않는 세 가지 이상의 조건을 구분할 때 사용

>if else if조건문 기본형태
>if (< 불 표현식>){
>
>} else if{(< 불 표현식>){
>
>} else if{(< 불 표현식>){
>
>} else {
>	
>}
>


switch 조건문
- 홀수와 짝수를 구분하는 수
>
>switch (<비교할 값>) {
>	case <값>:
>		문장
>		break;
>	case <값>:
>		문장
>		break;
>	default:
>		문장
>		break;
>}


삼항 연산자
- 숫자의 부호를 비교해서 0보다 큰지 안큰지 판별

><불 표현식> ? <참> : <거짓>

짧은 초기화 조건문
- || 연산자를 불이 아닌 자료에 사용할 경우
		- A||B에서 참이라면 A로 대치
		- A||B에서 거짓이라면 B로 대치



<h1>배열</h1>

- 여러 개의 자료를 한꺼번에 다룰 수 있는 자료형
- 대괄호 내부의 각 자료는 쉼료포 구분
- 배열에는 여러 자료형이 섞여 있을 수 있음
- 요소 : 배열 안에 들어 있는 각 자료

while 반복문
- while 반복문은 가장 기본적인 반복문

for 반복문
- 초기식을 실행하고 조건식을 확인한다. 조건식이 false이면 반복문을 빠져나가고 true이면 문장과 종결식을 차례로 실행해 다시 조건식이 true인지 확인함




## [03월 23일]

템플릿 문자열

> '안녕하세요'
= '안녕하세요'

>'52 + 273 = ${52 + 273}'
'52 + 273 = 325'

불

참과 거짓의 표현 : true 와 false
> true
true
> false
false

52 < 273 false
52 > 273 true


비교 연산자 
( == ) 같습니다.
( != ) 다릅니다.
( > )  왼쪽 피연산자가 큽니다.
( < )  오른쪽 피연산자가 큽니다.
( >= ) 왼족 피연산자가 크거나 같습니다.
( <= ) 오른쪽 피연산자가 크거나 같습니다.

> console.log(52 < 273);
console.log(52 > 273);
console.log("하마" > "가방");

true
false
false

- 불을 이용하면 논리 연산자를 만들 수 있습니다.

논리 부정 연산자

>console.log(!true);
console.log(!false);
console.log(!(52 < 273))
console.log(!(52 > 273))

false
true
false
true

-10 도는 !true처럼 - 연산자와 ! 연산자도 피연산자를 하나만 갖습니다.
이러한 연산자를 단향 연산자라고 하고, 반대로 피연산자가 2개라면 이항연산자, 
3개라면 삼항 연산자 라고 합니다.

- 논리 부정 연산자(!)는 단항 연산자 
- 논리합 연산자(||)와 논리곱 연산자(&&)는 이항 연산자

논리합 연산자는 2개의 피연산자 중에 하나만 true이면 전체가 true가 되는 연산자이다. (or)

논리곱 연산자는 2개의 피연산자 모두가 true이면 전체가 true가 되는 연산자이다. (and)


-변수
	값을 저장할 때 사용하는 식별자, 변수 선언 후 변수에 값을 할당

	- 변수 선언
		let 식별자;

	- 변수 pi를 선언
		> let pi;
		undefined
	
	- 변수 pi에 값을 할당
		> let pi;
		undefined
		>pi = 3.14159265;
		undefined
	- 변수 초기화

	- 변수 활용
		>let pi = 3.14159265;
		undefined
		>console.log(pi);
		undefined

복합 대입 연산자

복합 대입 연산자는 자료형에 적용하는 기본 연산자와 = 연산자를 함께 사용해 구성한다.

- 숫자열의 복합 대입 연산자

+= 숫자 덧셈 후 대입 연산자
-= 숫자 뺄셈 후 대입 연산자
*= 숫자 곱셈 후 대입 연산자
/= 숫자 나눗셈 후 대입 연산자

- 문자열의 복합 대입 연산자

+= 문자열 연결 후 대입 연산자

>let output = "hello ";
output = output + "world ";
output = output + "!";
console.log(output);

결과값 = hello world !

증감 연산자

변수에 적용할 수 있는 연산자 변수앞이나 뒤에 ++기호와 --기호를 붙여 사용한다.

변수++ 기존 변수 값에 1을 더합니다.(후위)
++변수 기존 변수 값에 1을 더합니다.(전위)
변수-- 기존 변수 값에 1을 뺍니다.(후위)
--변수 기존 변수 값에 1을 뺍니다.(전위)

> let number = 10;
number++;
console.log(number);
number--;
console.log(number);


결과값 :
11
10

자료형 검사

typeof (변수이름)
해당 변수의 자료형을 출력함

> typeof(10)
'number'
typeof("문자열")
'string'

JSP에는 여섯가지의 문자열 존재 string, number, boolean, function, object, undefined

undefined 자료형

변수를 선언했으나 초기화하지 않았을 때 나타나는 자료형이다.

일치 연산자

JSP에만 존재하는 특수한 연산자


( === ) 자료형과 값이 같은지 비교
( !== ) 자료형과 값이 다른지 비교


 강제 자료형 변환

- 숫자로 변환할 때는 Number() 함수 사용, 숫자로 변환할 수 없는 값을 강제로 숫자로 변환하면 NaN(Not a Number)이 출력됨

- 문자열로 변활할 때에는 String() 함수를 사용

- 불로 변환할 때에는 Boolean() 함수를 사용 (참, 거짓)

- 불로 변환할 때 false로 변환되는 것은 0, NaN, 빈 문자열, null, undefined다.

3장

IF 조건문

>if (<불 표현식>){	

>}

불 표현식이 true면 문장을 실행하고, false면 문장을 무시합니다.

>let input = 32;
>
>if (input % 2 == 0){
>	console.log("짝수입니다!");
>}
>if (input % 2 == 1){
>	console.log("홀수입니다!");
>}

결과값 : 짝수입니다!

if else 조건문


>if (<불 표현식>){	
	// 불 표현식이 참일 때 실행할 문장
>}

> else (<불 표현식>){	
	// 불 표현식이 거짓일 때 실행할 문장
>}

중첩 조건문

조건문 아넹 조건문을 중첩해 사용하는 것을 중첩 조건문이라고 한다.

## [03월 16일]
> 오늘 배운 내용 요약
    2장

1. 기본 용어
◇ 표현식과 문장

	문장 : 표현식이 하나 이상 모일 경우, 마지막에 종결할 때 세미콜론을 찍음
	프로그램 : 문장이 모여 프로그램이 됨

◇ 키워드

	교재 49p 표 2-1 참고

◇ 식별자
	이름을 붙일 때 사용하는 단어, 변수와 함수 이름 등으로 사용
		키워드 사용 안됨
		특수문자는 _와 $만 허용
		숫자로 시작하면 안됨
		공백은 입력하면 안됨

	식별자 사용 규칙
		1. 생성자 함수의 이름은 항상 대문자 ex) will out => willOut
		2. 변수, 함수, 속성, 메소드의 이름은 항상 소문자 ex) will return => willReturn
		3. 여러 단어로 된 식별자는 각 단어의 첫 글자를 대문자 ex) i am a boy => iAmABoy

◇ 주석
	프로그램의 진행에 영향을 주지 않는 코드
	( Ctrl + / ) 누르면 해당 언어에 맞게 주석처리 해줌
 
2. 출력

◇ 출력 메소드
	console 객체의 log() 메소드 사용 : console.log() 메소드
	console.log("문자열")
◇ PEPL을 사용한 출력
	곧바로 문장을 입력해서 출력
	"안녕" + "하세요"

3. 기본 자료형

◇ 숫자
	가장 기본적인 자료형
	
	숫자 생성 ( 54p 표 2-3 ~ 2-4 )
	console.log(52)
	console.log(52.271)

	기본적인 사칙 연산자
	+, -, *, /

	나머지 연산자
	%

◇ 문자열
	문자의 집합
	문자열 생성시 큰 따옴표나 작은따옴표 사용
	>"안녕하세요" or '안녕하세요'
	        '안녕하세요'

	이스케이프 문자
		따옴표를 문자 그대로 사용 가능
		문자열 줄바꿈 할 경우 사용

	문자열 합하기
	>" A " + " B "
	 'AB'
1장

1. JSP의 발전

◇ 세계에서 가장 오해를 많이 받는 프로그래밍 언어
	-부수적인 프로그래밍 언어로 취급

◇ 풍부한 경험을 제공하는 인터넷 애플리케이션(RIA)
	-구글 지도의 등장(JSP로 개발
		-JSP로만 만든 웹 페이지가 데스크톱에서도 사용하는 애플리케이션의 형태를 가짐 
		 => 기존의 지도에 비해 강력한 지도 제공
		-RIA : 풍부한 경험을 선사하는 웹 애플리케이션

	시대의 흐름에 따라 데스크탑 -> 모바일로 바뀌면서 JSP가 스포트라이트를 받음


◇  Node.js
	
	2008년 구글에서 개발

	-이벤트 기반
		동기 방식
			부분이 아닌 홈페이지 전체를 
		
		비동기방식(스레드Thread)
			

		Node.js : 모든 모듈이 처음부터 비동기 기반의 프로그램을 만들 수
			있도록 설계되어 초보자도 쉽게 프로그램을 만들 수 있음


2. JSP로 할 수 있는 일

◇ 웹 클라이언트 애플리케이션 개발
	웹 브라우저에서 실행되는 웹 클라이언트 개발 목적
	웹 브라우저에서 실행 할 수 있는 유일한 프로그래밍 언어

◇ 웹 서버 개발
	기존에 웹 개발은 두 가지 이상 프로그래밍 언어가 필요 =>( HTML , CSS , PERL 등등)
		웹 클라이언트, 웹 서버를 다른 언어로 개발

	Node.js가 등장하면서 웹 서버도 JSP로 개발 가능

	HTML이나 CSS에 비해 JSP가 용량이 큰 경우가 있음.
	<head> 사이에 JSP보다 <body> 사이에 삽입. (홈페이지의 로딩 때문)

	웹 페이지를 출력하지 않아도 웹 프로토콜(HTTP or HTTPS 등)을 활용
	하면 웹 서버로 칭함. (페이팔 결제 시스템 = Node.js활용)

	Node.js는 웹 개발과 관련해서 간단한 모듈들만 제공
	
	데이터 처리와 예외 처리 등이 복잡한게 단점 하지만 빠르다는 장점이 있음
	=>Linkedin에서 서버를 다시 개발할 떄, Node.js로 교체하면서 20배 빨라짐

◇ 모바일 애플리케이션 개발
	-네이티브 애플리케이션
		스마트에서 인식할 수 있는 프로그래밍 언어로 만든 앱
		기업에서 앱을 만들 경우 2가지 언어로 만들기에 비용이 2배가 됨
		JSP를 사용하면 1개의 앱만 개발해도 동작 가능
		=> 기업에서 개발자 수급이 편해짐
	-페이스북의 React Native
		JSP로 네이티브 앱을 개발(내부적으로 프로그래밍 언어 변환)
◇ 데스크톱 애플리케이션 개발
	-일렉트론(Electron) 모듈 : 자바스크립트로 개발 전용 텍스트 에디터를 만들어 배포
				=> 본격적으로 데스크톱 애플리 케이션 개발
	
1. JSP의 발전

◇ 세계에서 가장 오해를 많이 받는 프로그래밍 언어
	-부수적인 프로그래밍 언어로 취급

◇ 풍부한 경험을 제공하는 인터넷 애플리케이션(RIA)
	-구글 지도의 등장(JSP로 개발
		-JSP로만 만든 웹 페이지가 데스크톱에서도 사용하는 애플리케이션의 형태를 가짐 
		 => 기존의 지도에 비해 강력한 지도 제공
		-RIA : 풍부한 경험을 선사하는 웹 애플리케이션

	시대의 흐름에 따라 데스크탑 -> 모바일로 바뀌면서 JSP가 스포트라이트를 받음


◇  Node.js
	
	2008년 구글에서 개발

	-이벤트 기반
		동기 방식
			부분이 아닌 홈페이지 전체를 
		
		비동기방식(스레드Thread)
			

		Node.js : 모든 모듈이 처음부터 비동기 기반의 프로그램을 만들 수
			있도록 설계되어 초보자도 쉽게 프로그램을 만들 수 있음


2. JSP로 할 수 있는 일

◇ 웹 클라이언트 애플리케이션 개발
	웹 브라우저에서 실행되는 웹 클라이언트 개발 목적
	웹 브라우저에서 실행 할 수 있는 유일한 프로그래밍 언어

◇ 웹 서버 개발
	기존에 웹 개발은 두 가지 이상 프로그래밍 언어가 필요 =>( HTML , CSS , PERL 등등)
		웹 클라이언트, 웹 서버를 다른 언어로 개발

	Node.js가 등장하면서 웹 서버도 JSP로 개발 가능

	HTML이나 CSS에 비해 JSP가 용량이 큰 경우가 있음.
	<head> 사이에 JSP보다 <body> 사이에 삽입. (홈페이지의 로딩 때문)

	웹 페이지를 출력하지 않아도 웹 프로토콜(HTTP or HTTPS 등)을 활용
	하면 웹 서버로 칭함. (페이팔 결제 시스템 = Node.js활용)

	Node.js는 웹 개발과 관련해서 간단한 모듈들만 제공
	
	데이터 처리와 예외 처리 등이 복잡한게 단점 하지만 빠르다는 장점이 있음
	=>Linkedin에서 서버를 다시 개발할 떄, Node.js로 교체하면서 20배 빨라짐

◇ 모바일 애플리케이션 개발
	-네이티브 애플리케이션
		스마트에서 인식할 수 있는 프로그래밍 언어로 만든 앱
		기업에서 앱을 만들 경우 2가지 언어로 만들기에 비용이 2배가 됨
		JSP를 사용하면 1개의 앱만 개발해도 동작 가능
		=> 기업에서 개발자 수급이 편해짐
	-페이스북의 React Native
		JSP로 네이티브 앱을 개발(내부적으로 프로그래밍 언어 변환)
◇ 데스크톱 애플리케이션 개발
	-일렉트론(Electron) 모듈 : 자바스크립트로 개발 전용 텍스트 에디터를 만들어 배포
				=> 본격적으로 데스크톱 애플리 케이션 개발

◇ 게임 개발
	원래 게임은 서버와 클라이언트 모두 c++로 제작(속도↑)
	스마트폰이 활성화 되면서 '한 번에 여러 스마트폰 운영체제에서 실행 할 수 있는 앱을 개발하는것'이
	경제적으로 이득이 됨
	유니티(Unity) 게임 엔진 등장 : 자바스크립트 기반

◇ DB 관리
	DB
		데이터를 저장할 때 사용하는 프로그램 (My SQL 프로그래밍 언어 사용)
		NoSQL : 기존에 SQL은 복잡하고 무거워 사용하기 쉬운 데이터베이스 등장

> 요약
    1장. JSP의 역사와 개발 발전에 관한 내용과
         JSP로 할 수 있는 개발과 간단한 실습 환경 만들기
    
>    2장. JSP를 개발하면서 필요한 기초 지식과
         기본 용어와 규칙정리
