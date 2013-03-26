##  기본 문제 모음

* [http://niceaji.github.com/javascript-study/?doc=question1](http://niceaji.github.com/javascript-study/?doc=question1)
* [전체보기](https://github.com/niceaji/javascript-study/blob/gh-pages/doc/question1.md)
* [Source](https://github.com/niceaji/javascript-study)

*** 

##  기본 문제1

* 1부터 100까지 출력하는 프로그램을 작성
* 1~100사이의 홀수(짝수)를 출력하는 프로그램을 작성
* 구구단 

***

##  기본 문제2

prompt()를 이용하여 숫자를 입력받아 그 숫자의 합을 구함

* 함수화
* prompt()에 값이 없으면 숫자의 합 출력
* [동작예제](http://www.youtube.com/watch?v=_5dvqecYCco)

***

## OOP 문제1

* 스마트폰 클래스화

***

## OOP 문제2

* 기본문제 1,2로 정적(static) 클래스 만들기 

***

## OOP 문제3

* 영희, 일희 두명의 학생이 있다. 학교 강의 시간에 폰으로 문자를 주고 받고있다
* 영희는 아이폰, 일희는 갤럭시노트를 사용하고 있다
* JS Class를 이용하여 메세지를 주고 받는 프로그래밍을 구현

## Person Class

* 생성자 인자로 이름, 폰 받을것
* sendSMS()
* getSMS()

## Phone Class

* 상속개념을 사용하여, IPhone Class, Android Class 구현
* 생성자 인자로 폰번호 받을것
* 폰번호는 private이고, getNumber 함수를 구현할것
* getType() // iPhone or Android or feature 셋중하나 리턴

## 예

    var zero = new Person('영희', new IPhone('001'));
    var one = new Person('철수', new Android('002'));
    zero.sendSMS(one, '안녕? 철수야.');
    one.sendSMS(zero, '반가워. 영희야');


    //zero.sendSMS(one, '안녕? 철수야.');
    [영희]철수에게 '안녕? 철수야.' 메시지를 보냈습니다.
    001(iphone) -> 002 : 안녕? 철수야.
    [철수]영희에게 '안녕? 철수야.' 메시지를 받았습니다.

    //one.sendSMS(zero, '반가워. 영희야');
    [철수]영희에게 '반가워. 영희야' 메시지를 보냈습니다.
    002(android) -> 001 : 반가워. 영희야
    [영희]철수에게 '반가워. 영희야' 메시지를 받았습니다.


