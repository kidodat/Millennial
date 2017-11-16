# Object-oriented design

## [is-a] and [has-a]
### [is-a]
クラスの間に継承関係があること。
* A truck is a car.
* A bust is a car.
```
class Car{}
class Truck extends Car{}
class Bus extends Car{}
```
### [has-a]
あるクラスで他のクラスを利用する
* A car has four tires.
* A car has a steering wheel.

```
class Car
{
    Tire[] tire;
    SteeringWheel sw;
}
```
### 凝集度と結合度

#### 凝集度
凝集度はクラスの機能（メソッド）と属性（変数）の関連性の強さを表す。なるべく凝集度を高く持った方がシステムの補修生と拡張性が向上する。

整理すると、お互い関連する機能と属性を分散するより、纏めた方が良いということ。

####　結合度
