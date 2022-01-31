# Animations


## CABasicAnimation
This animates circle stroke filling
```swift
    let strokeAnimation = CABasicAnimation(keyPath: "strokeEnd")
    strokeAnimation.fromValue = 0
    strokeAnimation.toValue = 1
    strokeAnimation.duration = CFTimeInterval(animationDuration)
    strokeAnimation.fillMode = .forwards
    strokeAnimation.isRemovedOnCompletion = true
    strokeAnimation.delegate = self
    animatingStrokeLayer?.add(strokeAnimation, forKey: "strokeAnimation")
```