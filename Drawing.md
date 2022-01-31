# Drawing

## Make a circle stroke


```swift
    let layer = CAShapeLayer()
    let center = CGPoint(x: bounds.width / 2, y: bounds.height / 2) // Center of circle
    let circlePath = UIBezierPath(arcCenter: center, 
                                  radius: 30, startAngle: -0.5 * CGFloat.pi, 
                                  endAngle: 1.5 * CGFloat.pi, clockwise: true)
    layer.path = circlePath.cgPath
    layer.strokeColor = trackColor
    layer.lineWidth = 3
    layer.fillColor = UIColor.clear.cgColor
    layer.lineCap = CAShapeLayerLineCap.round
    layer.strokeEnd = 1 // Filling percent
    view.addSublayer(layer);
```