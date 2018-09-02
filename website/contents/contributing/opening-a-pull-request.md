---
path: "/contributing/opening-a-pull-request"
title: "Opening a Pull Request"
hasPlayground: false
---
<!--
# Opening a Pull Request
-->
# Pull Request 열기

<!--
Before opening your first pull request to Yoga you have to know how to get the code,
install build time dependencies, and test the code locally.
-->
첫 pull request를 열기전 Yoga로 부터 코드를 받는 방법,
의존성(dependencies) 설치(install) 및 빌드(build), 그리고 로컬에서 코드 테스트 하는 법을 알아야 합니다.

<!--
### Clone
-->
### 클론(Clone)

```
$> git clone https://github.com/facebook/yoga.git
$> cd yoga
```
<!--
### Install dependencies
-->
### 의존성 설치(Install dependencies)

```
$> git submodule init
$> git submodule update
$> brew install buck
```
<!--
### Build and Test
-->
### 빌드와 테스트(Build and Test)

```
$> buck build //:yoga
$> buck test //:yoga
```
<!--
## Making a Change
-->
## 변경내용 작성하기(Making a Change)

<!--
Now all you need to do is make your change and test it before submitting a pull request for review.
Below is the general structure of the repo and where you may want to make your change. One you have
made your change see the [testing documentation](/contributing/testing) for more on how to test your change.
-->
이제 검토를 위한 pull request 제출전 당신의 변경내용과 테스트를 작성하십시오.
아래는 일반적인 repo 구조와 당신의 변경내용 작성할 위치입니다.
더 자세한 정보와 당신의 변경내용을 어떻게 테스트 할지에 대해서는 [testing documentation](/contributing/testing)를 참조하십시요.

``` bash
/yoga
|-- yoga                  # Home to the main Yoga codebase written in C++. Any algorithmic changes should be made here
|-- lib                   # Yoga external dependencies. Be thoughtful adding any new ones
|-- tests                 # Yoga's C++ test suite. Both manaul and generated tests
|-- gentest
|   |-- fixtures          # html fixtures for generated tests    
|-- java         
|   |-- com/facebook/yoga # Java binding code
|   |-- jni               # JNI binding code
|-- yogacore              # Android bindings without View support
|-- android               # Android View bindings
|-- YogaKit               # iOS UIView bindings
|-- javascript            # emscripten / javascript bindings
|-- csharp                # .NET bindings in c#
```