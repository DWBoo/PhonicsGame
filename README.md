# 기본적인 구조
![image](https://github.com/DWBoo/PhonicsGame/assets/147593910/3bcec62e-6b6e-45e2-a452-1dc0c9e5d049)</br>
최상위 오브젝트 하나에 모든 페이지가 포함되어 있으며, 하나의 프리팹으로 저장 후 사용
![image](https://github.com/DWBoo/PhonicsGame/assets/147593910/37119766-8ce1-4aef-8eec-84717b237387)</br>
모든 페이지는 Page 클래스를 상속하여 Open과 Close 메소드를 용도에 맞게 정의하고 이전 페이지로 이동할 수 있도록 모든 페이지의 참조는 AppManager에 Page로 업캐스팅하여 Stack에서 관리
