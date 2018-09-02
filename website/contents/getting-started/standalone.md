---
path: "/getting-started/standalone"
title: "Standalone"
hasPlayground: false
---

# Standalone

<!-- Adding Yoga to a project is as simple as adding the dependency to your package manager of choice. -->
프로젝트에 Yoga를 추가하는것은 선택한 패키지 관리자에 dependency를 추가하는 만큼 간단합니다.

### Android

```groovy
dependencies {
	compile 'com.facebook.yoga.android:yoga-layout:x.x.x'
}
```

### Javascript

<!-- The JavaScript bindings for Yoga can be used from node.js and within the browser.
When using Yoga from node.js the native library is used, in browesers a pure JS
version is used (corss-compiled using [emscripten](http://kripken.github.io/emscripten-site/)). -->
요가를 위한 Javascript 바인딩은 node.js 와 브라우저에서 사용할 수 잇습니다. node.js에서 요가를 사용할 때 네이티브 라이브러리가 이용되고, 브라우저들에서는 순수한 JS 버전이 사용됩니다. (corss-compiled using [emscripten](http://kripken.github.io/emscripten-site/))

```
$> yarn add yoga-layout
```

<!-- This is an example on how to use Yoga in JavaScript, for a full API reference,
have a look at the [flow-type definitions](https://github.com/facebook/yoga/blob/master/javascript/sources/entry-common.js#L123). -->
이건 전체 API 레퍼런스를 위해 Javascript에서 Yoga를 어떻게 사용하는지에 대한 예제입니다.
[flow-type definitions]를 살펴 보십시요.
(https://github.com/facebook/yoga/blob/master/javascript/sources/entry-common.js#L123).

```js
import yoga, {Node} from 'yoga-layout';

const root = Node.create();
root.setWidth(500);
root.setHeight(300);
root.setJustifyContent(yoga.JUSTIFY_CENTER);

const node1 = Node.create();
node1.setWidth(100);
node1.setHeight(100);

const node2 = Node.create();
node2.setWidth(100);
node2.setHeight(100);

root.insertChild(node1, 0);
root.insertChild(node2, 1);

root.calculateLayout(500, 300, yoga.DIRECTION_LTR);
console.log(root.getComputedLayout());
// {left: 0, top: 0, width: 500, height: 300}
console.log(node1.getComputedLayout());
// {left: 150, top: 0, width: 100, height: 100}
console.log(node2.getComputedLayout());
// {left: 250, top: 0, width: 100, height: 100}
```

### iOS

```
pod 'YogaKit', '~> 1.7'
```

<!-- ## Including Yoga From Source -->
## Source에서 Yoga 포함하기

<!-- If you plan to include Yoga from Source in a C++ project then all you have to do is inlude
the top level `yoga` folder. Make sure to look at the top level `BUCK` file to ensure you build
using the same compiler flags. -->

C++ 프로젝트 소스에서 Yoga를 포함 시킬거라면 당신이 할 일은 최상위 `yoga` 폴더를 포함하는 것입니다.
최상위 수준의 `BUCK` 파일을 보고 동일한 compiler flags를 사용해 빌드하십시요.


