---
path: "/docs/absolute-relative-layout"
title: "Absolute/Relative Layout"
hasPlayground: true
---
## Absolute/Relative Layout

The `position type` of an element defines how it is
positioned within its parent.

`position type`은 해당 요소가 부모요소 내에서 어떻게 배치될지를 결정한다.

**RELATIVE (DEFAULT)** By default an element is positioned
relatively. This means an element is positioned according to the
normal flow of the layout, and then offset relative to that position
based on the values of `top`, `right`, `bottom`, and `left`.
The offset does not affect the position of any sibling or parent elements.

**RELATIVE (DEFAULT)** 요소는 Relative를 default 값으로 배치된다.
즉 요소는 레이아웃의 일반적인 흐름에 따라 배치되고, `top`, `right`, `bottom`, 
그리고 `left` 값을 통해 offset 지정이 가능하다. offset으로 배치될 때
이는 형제요소 또는 부모요소에 영향을 주지 않는다.


**ABSOLUTE** When positioned absolutely an element doesn't take
part in the normal layout flow. It is instead laid out independent 
of its siblings. The position is determined based on the
`top`, `right`, `bottom`, and `left` values. 

**ABSOLUTE** 요소가 absolute 하게 배치될 때 그 요소는 더이상 레이아웃의
일반적인 흐름의 일부가 아니게 된다. 그대신 형제 요소들로부터 독립되어 구성된다.
위치는 `top`, `right`, `bottom`, 그리고 `left` 값을 통해 배치된다.


<controls prop="positionType"></controls>

The position values `top`, `right`, `bottom`, and `left` behave
differently depending on the `position type` of the element. For
a `relative` element they offset the position of the element in the
direction specified. For `absolute` element though these properties
specify the offset of the element's side from the same side on the parent.

`top`, `right`, `bottom`, 그리고 `left`의 offset 값은 해당요소의 `position type`에
따라 다른게 적용된다. `relative`값을 가진 요소는 설정된 offset의 값만큼 자신의 위치에서부터 
해당 방향으로 이동한다. 반면 `absolute`는 부모요소의 시작점에서부터 offset 값만큼 이동하며,
형제요소들은 해당요소가 없는 것처럼 행동한다.

<controls prop="position"></controls>
