# 의존 역전 원칙



> 의존 역전 원칙 \(Dependency Inversion principle\) - DIP

* 정의

고수준 모듈은 저수준 모듈에 종속되어서는 안된다.

* 원칙 위반시 증상
  * 저수준에서 변경 발생 가능성이 많은 데 변경될 때마다 고수준 모듈에 수정사항이 발생한다.
* 원칙 적용 방법
  * 고수준 모듈의 변화되는 부분을 추상화한다.
  * 저수준 모듈을 추상화에 의존 시킨다.

