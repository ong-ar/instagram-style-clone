- margin

  - auto: 수평만 적용

- flex

  - flex-grow, flex-shrink, flex-basis

- flex-basis
  flex-basis 속성은 항목의 크기를 결정합니다. 이 속성의 기본값은 auto이며, 이 경우 브라우저는 항목이 크기를 갖는지 확인합니다. 위의 사진 예시의 경우 항목의 크기가 100 픽셀이므로 flex-basis의 값으로 100 픽셀이 사용됩니다.
  flex 항목에 크기가 지정되어 있지 않으면, flex 항목의 내용물 크기가 flex-basis 값으로 사용됩니다. 따라서 flex 컨테이너에서 display: flex 속성만을 지정하면 flex항목들이 각 내용물 크기만큼 공간을 차지하게 됩니다.

- flex-grow
  flex-grow값을 양수로 지정하면 flex 항목별로 주축 방향 크기가 flex-basis 값 이상으로 늘어날 수 있게 됩니다. 위의 사진 예시에서 모든 항목의 flex-grow 값을 1로 지정하면 사용가능한 공간은 각 항목에게 동일하게 분배되며, 각 항목은 주축을 따라 분배받은 값만큼 사이즈를 늘려 공간을 차지합니다.
  첫 항목의 flex-grow 값을 2로 지정하고 나머지 두 개의 항목을 1로 지정한다면 각 항목에 지정된 flex-grow 값의 비율에 따라 남은 공간이 분배됩니다. 각 항목의 flex-grow 비율이 2:1:1 이므로 첫 항목에게 100 픽셀, 두 번째와 세 번째 항목에게 50 픽셀씩 분배됩니다.

- flex-shrink
  flex-grow 속성이 주축에서 남는 공간을 항목들에게 분배하는 방법을 결정한다면 flex-shrink 속성은 주축의 공간이 부족할때 각 항목의 사이즈를 줄이는 방법을 정의합니다. 만약 flex 컨테이너가 flex 항목을 모두 포함할 만큼 넉넉한 공간을 갖고 있지 않고 flex-shrink 값이 양수이면 flex 항목은 flex-basis에 지정된 크기보다 작아집니다. 또한, flex-grow 속성과 마찬가지로 더 큰 flex-shrink 값을 갖는 항목의 사이즈가 더 빨리 줄어듭니다.
