# Drawing

## Make a circle stroke


```swift
    let circleLayer = CAShapeLayer()
    let center = CGPoint(x: bounds.width / 2, y: bounds.height / 2) // Center of circle
    let circlePath = UIBezierPath(arcCenter: center, 
                                  radius: 30, startAngle: -0.5 * CGFloat.pi, 
                                  endAngle: 1.5 * CGFloat.pi, clockwise: true)
    circleLayer.path = circlePath.cgPath
    circleLayer.strokeColor = trackColor
    circleLayer.lineWidth = 3
    circleLayer.fillColor = UIColor.clear.cgColor
    circleLayer.lineCap = CAShapeLayerLineCap.round
    circleLayer.strokeEnd = 1 // Filling percent
    layer.addSublayer(circleLayer);
```