## UIWindow、UIView、CALayer 三者和联系？


简单来说，UIView 是对 CALayer 的一个封装。

UIView中有一个CALayer类型的属性layer和backgroundColor等，background等属性实际是对CALayer类型下同名属性的包装；
UIView的显示部分是由CALayer的contents属性决定的，contents对应的backing store（bit map类型的位图），最终显示到屏幕上的控件，实际就是位图
UIView为CAlayer提供内容，以及负责处理触摸事件，参与响应链
CALayer只负责显示内容contents


