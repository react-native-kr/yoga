---
path: "/docs/align-items"
title: "Align Items / Self"
hasPlayground: true
---

## Align Items

Align items describes how to align children along the cross axis of their container.
Align items is very similar to [`justify content`](/docs/justify-content) but instead of
applying to the main axis, `align items` applies to the cross axis.

Align items는 containor의 cross axis에 어떻게 children 요소들을 정렬 시킬지를 정한다. 
Align items [`justify content`](/docs/justify-content)와 매우 유사하지만 `justify content`가
main-axis를 기준으로 정렬되는 반면, `align items`는 cross-axis를 기준으로 정렬된다.

**STRETCH (DEFAULT)** Stretch children of a container to match the `height` of the container's cross axis.

**STRETCH (DEFAULT)** children의 높이를 containor의 cross-axis 길이와 같게 늘린다.

**FLEX START** Align children of a container to the start of the container's cross axis.

**FLEX START** children을 containor의 cross-axis 시작 부분에 정렬시킨다.

**FLEX END** Align children of a container to the end of the container's cross axis.

**FLEX END** children을 containor의 cross-axis 끝 부분에 정렬시킨다.

**CENTER** Align children of a container in the center of the container's cross axis.

**CENTER** children을 containor의 cross-axis 중앙에에 정렬시킨다.

<controls prop="alignItems"></controls>

## Align Self

Align self has the same options and effect as `align items` but instead of
affecting the children within a container, you can apply this property to
a single child to change its alignment within its parent. `align self`
overrides any option set by the parent with `align items`.

Align self는 `align items`과 같은 옵션을 갖는다. 다만, containor의 children에 적용하는 대신
child 각각에 parent를 기준으로 정렬 되도록 해당 속성을 적용할 수 있다. `align self`는 이전에
설정된 `align items` 속성을 override 한다.

<controls prop="alignSelf"></controls>
