---
path: "/docs/aspect-ratio"
title: "Aspect Ratio"
hasPlayground: true
---

## Aspect Ratio

AspectRatio is a property introduced by Yoga and is not present as a settable
property in the css flexbox specification. Flexbox does has the notion of
aspect ratio though for things with intrinsic aspect ratio such as images.

AspectRatio는 Yoga가 제공하는 property이며 css flexbox의 specification에서 제공하는 property는 아니다.
Flexbox에 aspect ratio의 개념이 있기는 하지만, image와 같이 원래 aspect ratio를 가진 요소들에 해당한다.

The `aspect ratio` property in Yoga has the following properties:

Yoga의 `aspect ratio` property는 다음과 같은 속성을 갖는다:

- Accepts any floating point value > 0, the default is undefined.

- 0보다 큰 어떤 floating point를 가질 수 있으며, default는 undefined 이다.

- Defined as the ratio between the `width` and the `height` of a node e.g. if a node has an aspect ratio of 2 then its `width` is twice the size of its `height`.

- 

- Respects the `min` and `max` dimensions of an item.
- Has higher priority than `flex grow`
- If `aspect ratio`, `width`, and `height` are set then the cross axis dimension is overridden.

<controls prop="aspectRatio"></controls>
