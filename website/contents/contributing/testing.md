---
path: "/contributing/testing"
title: "Testing"
hasPlayground: false
---

# Testing

<!-- Yoga tries to be as close as possible to chrome in its flexbox behaviour.
To ensure this most of Yoga's test suite is automatically generateded from
running the corresponding layout in chrome using a webdriver which then generates 
C++ test which asserts that Yoga will produce matching outputs for that layout. -->
Yoga는 가능한 크롬에 근접한 flexbox 동작을 시도합니다.
To ensure this most of Yoga's test suite is automatically generateded from
running the corresponding layout in chrome using a webdriver which then generates 
C++ test which asserts that Yoga will produce matching outputs for that layout.

<!-- ## Running the Test Suite -->
## 테스트 슈츠 실행하기

<!-- 1. Yoga builds with [buck](https://buckbuild.com). Follow their documentation to get up and running.
2. For testing Yoga relies on [gtest](https://github.com/google/googletest) as a submodule. After cloning Yoga run `git submodule init` followed by `git submodule update`.
3. In a terminal from the root of your Yoga checkout run `buck test //:yoga`. -->
1. Yoga는 [buck](https://buckbuild.com)로 구성되어있습니다. 설명서를 따라 실행 하십시요..
2. 테스트를 위해 Yoga는 [gtest](https://github.com/google/googletest)를 submodule로 다룹니다. cloning Yoga 이후 `git submodule init` followed by `git submodule update`.
3. 체크아웃된 Yoga 루트 폴더에서 실행하십시요. `buck test //:yoga`.

<!-- ## Adding a Test -->
## 테스트 추가하기

<!-- Instead of manually writing a test which ensures parity with web implementations
of Flexbox we make use of a generated test suite. We use `gentest/gentest.rb` to
generate this test suite. Write the html which you want to verify in Yoga and put
it in the `gentest/fixtures` folder, such as the following. -->
수동으로 Flexbox 웹 구현과 패리티를 구성한 테스트를 작성하는 대신에 우리는 생성된 테스트 슈츠를 사용합니다. `gentest / gentest.rb`를 사용하여이 테스트 슈츠를 생성합니다. Yoga에서 확인하고 싶은 HTML을 작성하고 `gentest / fixtures` 폴더에 입력하십시오, 예를 들면 다음과 같습니다.



```html
<div id="my_test" style="width: 100px; height: 100px; align-items: center;">
  <div style="width: 50px; height: 50px;"></div>
</div>
```

<!-- Run `gentest/gentest.rb` to generate test code and re-run `buck test //:yoga`
to validate the behavior. One test case will be generated for every root `div`
in the input html with the string in the `id` corresponding to the test name. -->
`gentest / gentest.rb`를 실행하여 테스트 코드를 생성하고 `buck test // : yoga`를 다시 실행해 행동을 확인 하십시요.
하나의 테스트 케이스가 테스트 이름에 해당하는`id` 문자열과 함께 입력 HTML안 모든 루트`div`에 대하여 생성됩니다.

<!-- You may need to install the latest watir gem (`gem install watir`) and
[ChromeDriver](https://sites.google.com/a/chromium.org/chromedriver/) to
run `gentest/gentest.rb` Ruby script. -->
최신 watir gem (`gem install watir`)을 설치해야 할 수 있고 
[ChromeDriver](https://sites.google.com/a/chromium.org/chromedriver/)에서 
`gentest/gentest.rb` Ruby script를 실행하십시요.

## Manual test

<!-- For some aspects of Yoga we cannot generate a test using the test generation
infrastructure described earlier. For these cases we manually write a test in 
the `/tests` directory.	 -->
Yoga의 일부 측면에 대해 우리는 앞에서 설명한 테스트 세대 하부구조를 이용하여 테스트를 생성할 수 없습니다.
이 경우 우리는 `/ tests` 디렉토리에서 수동으로 테스트를 작성합니다.