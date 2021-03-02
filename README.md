# Object-Detection
Reviews for object detection papers


## 1-1. 1-stage detector & default box

Multi-scale Feature map for detection

각각의 feature map에서 Default Box를 뽑아서 Ground truth box와 비교한다. 그리고 3x3xp kernel은 class score와 default box coordinates에 상대적인 shape offset을 만든다.

Bounding Box의 offset은 각 feature map상의 default box에 상대적으로 측정된다.

그리고 Default Bounding Box 좌표를 각 Feature Map에 타일링한다. 그러고 나서 Bounding Box의 해당 Default Box와 상대적인 offset 값을 통해 나타낸다.


