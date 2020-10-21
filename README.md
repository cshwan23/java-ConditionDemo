# java-ConditionDemo
조건문(if문, else문, elseif문, 조건 중첩문, 논리연산(switch문)


    package org.opentutorials.javatutorials.condition;

    public class Condition1Demo {

	  public static void main(String[] args) {
	

1. if (true) { } 

		if (true) {
			
	   System.out.println("result : true");
			
	   }
		
2. if (false)	{ }	

		
		if (false) {
			
			System.out.println(1);
			System.out.println(2);
			System.out.println(3);
			System.out.println(4);
			
		}
		
		System.out.println(5);
	
		
false 이면 중괄호를 띄어넘고 실행이 된다.
		
3. else 문
		
    
        if ( true / false ) {
		
		    //true면 여기가 실행
		
	      } else {
		
		    //false면 여기가 실행
		
	      } 

		
		if (true) {
			
				System.out.println(1);
				
		}else{
			
				System.out.println(2);
		
		}
		
		
	4. else if 문
		
		 if (true/false) {
		
		 //true면 이구간이 실행이 된다.
		 //false면 else if 로 넘어간다
		
		 } else if (true/false ) {
		
		 //true면 이구간이 실행된다.
		 //false면 else구문이 실행된다.
		
		 } else {
		
		 //false면 이구간이 실행된다.
		
		}

		
		
	   if (false) {
		
		 System.out.println(1);
		
	    } else if (true) {
		
	  	System.out.println(2);   // 이부분이 출력된다. 나머지는 뛰어넘는

    	} else if (true) {
		
	  	System.out.println(3);

	    } else {
		
	  	System.out.println(4);

	    }

	
지금은 값들이 다 정해져 있다.
어떨때는 트루 어떨땐 폴스여야 조건문으로서의 가치, 효용이 있게된다.
	
	
5. 변수와 비교 연산자 그리고 조건문
LoginDemo
	프로그래머가 되면
	소비자로서의 삶에서 벗어나
	생산자로서의 삶이 된다면
	정말 가볍게 여겨지지않고 귀한게 늘어나게된다..
	

 	String id = args[0];
	if (id.equals("egoing")) {
		System.out.println("right");
	}else{
		System.out.println("wrong");
	}
	
 String id = args[0];
배열을 의미하는데 args[0]이 첫번째 입력값(egoing)
의미한다고 이해하자.
입력한 값이 egoing과 같은지 비교하는 구문은
id.equals("egoing")이다.	
	
6. 조건문의 중첩
	
	    String id1 = args[0];
    	String password = args[1];

    	if (id1.equals("egoing")) {
		
	  	if (password.equals("1111")) {
			
			System.out.println("right");
		
	  	}else{
			
			System.out.println("wrong");
		
		  }
		
    	} else {
		
		  System.out.println("wrong");
		
	  }

	
	
7.논리연산(Switch문)
	
	
default  값이 정의 되어있다면 default로 넘어간다 조건에 모두 안맞을때
	
	
    System.out.println("switch(1)");

    switch(1) {

    case 1:
	  
    System.out.println("one");

    case 2:
	
    System.out.println("two");

    case 3:
	
    System.out.println("three");
	
    }

switch(1)이면 case 1이 실행되고
case2,3이 순차적으로 실행된다.
	

    System.out.println("switch(2)");

    switch (2) {

    case 1:
	
    System.out.println("one");

    case 2:
	
    System.out.println("two");

    case 3:
	
    System.out.println("three");
    
    }
	
switch(2)이면case 1은 건너뛰고 case 2부 실행되고
case3이 순차적으로 실행된다.


7-2 switch break

	
    System.out.println("switch(1)");

    switch (1) {

    case 1:
	
    System.out.println("one");
	  break;
   
    case 2:
	  
    System.out.println("two");
	  break;

    case 3:
	  
    System.out.println("three");
	  break;
    }

break;를 걸어버리면 로직이 끝나면 다음 순차로 이어지는게
 아니라 switch문 밖으로 나가버린다.
	

	
7-2 switch default
	

    System.out.println("switch(1)");

    switch (4) {

    case 1:
    System.out.println("one");
    break;
    case 2:
    System.out.println("two");
    break;
    case 3:
    System.out.println("three");
    break;

    default:
	  System.out.println("default");
	  break;
    }

 입력값이 case에 해당되는 값이 없때
 디폴트 구문을 만들어주면 디폴트로 연결이되어
 디폴트의 값이 출력되게 된다.
 
