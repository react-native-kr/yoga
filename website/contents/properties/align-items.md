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

**FLEX START** 

**FLEX END** Align children of a container to the end of the container's cross axis.

**FLEX END**

**CENTER** Align children of a container in the center of the container's cross axis.

**CENTER**

<controls prop="alignItems"></controls>

## Align Self

Align self has the same options and effect as `align items` but instead of
affecting the children within a container, you can apply this property to
a single child to change its alignment within its parent. `align self`
overrides any option set by the parent with `align items`.

<controls prop="alignSelf"></controls>
