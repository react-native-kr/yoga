---
path: "/docs/min-max"
title: "Max / Min Width and Height"
hasPlayground: true
---

## Max / Min Width and Height

이 프로퍼티들은 엘리먼트의 최대 및 최소 크기의 제약을 설정하며, 다른 모든 프로퍼티들보다 항상 더 높은 우선순위를 갖게됩니다.
이 제약들은 절대적 픽셀 값이나 부모 엘리먼트 크기의 백분율로 명시될 수 있습니다.
기본적으로, 이 제약들은 `undefined` 값을 갖고 있습니다.
<!--
All the following properties set the maximum and minimum size constraints of an element. These properties have higher priority than all other properties and will always be respected. Constraints can be specified as either absolute pixel values or as percentages of their parent's size. By default all these constraints are undefined.
-->

### Max Width

<controls prop="maxWidth"></controls>

### Min Width

<controls prop="minWidth"></controls>

### Max Height

<controls prop="maxHeight"></controls>

### Min Height

<controls prop="minHeight"></controls>