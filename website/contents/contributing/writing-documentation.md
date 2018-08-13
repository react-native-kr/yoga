---
path: "/contributing/writing-documentation"
title: "Writing Documentation"
hasPlayground: false
---

<!-- ## Writing Documentation -->
## 문서 작성하기

<!-- Documentation pages are generated from Markdown files in `contents/`.
The files are organized in 4 sections/folders (getting-started, properties,
examples, contributing) which are dynamically listed on the docs overview page.
The Markdown files should contain a header with metadata. -->

문서화 페이지는 `contents/`의 Markdown 파일에서 생성됩니다.
4개의 색션과 폴더(getting-started, properties, examples, contributing)로 구성된 파일들은 문서 개요페이지에 동적으로 나열되어집니다.
Markdown 파일들에는 메타 데이터가 포함 된 헤더가 있어야합니다.

```markdown
---
path: "docs/flexDirection"
title: "Flex Direction"
hasPlayground: true
initialPlayground: eyJ3aWR0aCI6IjYwMCIsImhlaWdodCI6NTAwLCJjaGlsZHJlbiI6W3t9LHt9LHt9XX0=
---
```

<!-- - The `path` indicates the URL path this page will be available at.
- The `title` is used as the page's HTML-title and when referencing
  the file from the documentation overview.
- The `hasPlayground` property indicates whether this documentation
  has an associated playground to test out the documented feature.
- The `initialPlayground` property is only relevant for documentation
  pages with playgrounds and contains the initial playground state.
  This base64 string is a reference to the hash (content after #)
  of a [playground](/playground) url.
 - The `redirect` property allows to redirect to the other page, the path of which is mentioned in the property `path`. -->
- `path`는 페이지를 사용할 수있는 URL 경로를 나타냅니다.
- `title`은 페이지의 HTML-title과 문서 개요에서 파일을 참조할때 사용됩니다.
- `hasPlayground` 속성은 이 문서가 문서화된 기능을 테스트 할 수 있는 playground을 제공합니다.
- `initialPlayground` 속성은 문서에만 관련이 있습니다. playground가 있는 페이지는 초기 playground 상태를 포함합니다.,
  [playground](/playground) url의 base64 문자열은 해시 (# 이후의 내용)에 대한 참조입니다.
  of a [playground](/playground) url.
 - `redirect`는 다른 페이지로 리디렉트(redirect) 할 수 있습니다,이 페이지의 경로는 `path` 속성에서 언급됩니다.


<!-- Within the markdown of a documentation page which has an associated
playground you can add controls to let the user play around with the feature
directly from the documenation page. -->


관련된 playground 문서 페이지의 Markdown 내에서
당신은 사용자가 기능을 사용하여 놀 수있는 컨트롤을 사용자가 기능을 가지고 놀 수 있는 문서 페이지에 추가 할 수 있습니다.

```markdown
<controls prop="alignContent"></controls>
```

<!-- If you would like to redirect to another page (potentially an external link) the header would look something like this. -->

만약 다른 페이지 (잠재적 외부 링크)로 리디렉트(redirect)하려는 경우 헤더는 다음과 같습니다.

```markdown
---
path: "/playground#eyJ3aWR0aCI6IjYwMCIsImhlaWdodCI6NTAwLCJjaGlsZHJlbiI6W3t9LHt9LHt9XX0="
title: "Flex Direction"
redirect: true
---

```
