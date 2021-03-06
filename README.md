# Object-Detection
Reviews for object detection papers

## 용어 정리

receptive field : 출력 공간에 영향을 미치는 영역


## 1-1. SSD

기본적으로 Backbone - neck- head의 구성을 갖는다.

1. Default Box의 Feature Map에 대한 상대적인 크기는 고정되어 있다.
2. 각각의 Default Box는 C+4개의 Ouput을 갖게되며 (클래스 숫자와 Offset을 합한 크기), 1개의 m*n의 feature map에 대해 (c+4)*k*m*n의 Output을 갖게 된다.
3. Non-maximum suppression을 이용해 가장 클래스가 있을 법한 Default Box 만을 고르게 되는데, NMS는 각각의 박스를 Confidence Score가 높은 순으로 정렬하고 IOU가 0.5인 박스를 삭제함으로써 얻어진다.
4. 이 박스에 대해 Loss를 적용한다. 이 Loss는 Input 사이즈에 영향받지 않는다.
5. Default Box의 Scale을 결정하는 알고리즘들이 따로 존재한다.

## 1-2 YOLO v3 (head 부분만)


## 1-3 YOLO v4

## Feature Pyramid Networks for Object Detection
