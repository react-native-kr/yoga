---
path: "/docs/justify-content"
title: "Justify Content"
hasPlayground: true
---

## Justify Content

<!-- Justify content describes how to align children within the main axis of their container.
For example, you can use this property to center a child horizontally within a container
with `flex direction` set to `row` or vertically within a container with `flex direction`
set to `column`. -->
Justify Content는 어떻게 children이 그들의 container의 주축에서 정렬하는지를 설명합니다.
예를 들어, 당신은 이 속성을 통해 `flex direction`을 `row`로 설정함으로써 container내 child를 수평으로 배치하거나
`flex direction`을 `column`으로 설정함으로써 container내에서 수직으로 배치 가능합니다.

<!-- **FLEX START (DEFAULT)** Align children of a container to the start of the container's main axis. -->
**FLEX START (DEFAULT)** container의 children를 container의 주축의 시작지점에 정렬시킵니다.

<!-- **FLEX END** Align children of a container to the end of the container's main axis. -->
**FLEX END** container의 children를 container의 주축의 끝에 정렬 시킵니다.

<!-- **CENTER** Align children of a container in the center of the container's main axis. -->
**CENTER** container의 children를 container의 주축의 중앙에 정렬 시킵니다.

<!-- **SPACE BETWEEN** Evenly space of children across the container's main axis, distributing
remaining space between the children. -->
**SPACE BETWEEN** container의 주축을 가로지르는 children의 균등한 공간, children 사이에 남은 공간 제공.

<!-- **SPACE AROUND** Evenly space of children across the container's main axis, distributing
remaining space around the children. Compared to `space between` using
`space around` will result in space being distributed to the beginning of
the first child and end of the last child. -->

**SPACE AROUND** container의 주축을 가로지르는 children의 균등한 공간, children 사이에 남은 공간 제공.
`space between`과 비교하여 `space around`는 첫 번째 child의 시작 부분과 마지막 child의 끝 부분에 공간을 분배 할것입니다.


<controls prop="justifyContent"></controls>
