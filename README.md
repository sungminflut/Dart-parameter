# Dart-parameter

positional parameter - 순서가 중요한 파라미터
 addNumbers(int x, int y, int z)
 void main() {
   addNumbers(10, 20, 30);
 }

optional parameter - 있어도 되고 없어도 되는 파라미터
 addNumbers(int x, [int y = 20, int z = 30])
 void main() {
  addNumbers(10);
 }

named parameter - 이름이 있는 피라미터 (순서가 중요하지 않다.)
 addNumbers({
  required int x,
  required int y,
  required int z, // optional parameter 하는 법 -> int z = 30,
 })
 void main() {
  addNumbers(x: 10, y: 20, z: 30); // optional parameter 로 선언했을 경우 z 값 안넣어줘도 됨.
 }

* 함수 선언 시 맨 앞에 void 가 아닌 int 등을 사용할 경우 return 을 해줘야 함.

arrow function - 화살표 함수
 int addNumbers(int x, {
  required int y,
  int z = 30,
}) => x + y + z; // return
