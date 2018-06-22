---
path: "/docs/align-content"
title: "Align Content"
hasPlayground: true
initialPlayground: eyJ3aWR0aCI6NTAwLCJoZWlnaHQiOjUwMCwiYWxpZ25Db250ZW50IjoxLCJmbGV4V3JhcCI6MSwiY2hpbGRyZW4iOlt7IndpZHRoIjoxMDAsImhlaWdodCI6MTAwLCJtaW5XaWR0aCI6bnVsbCwibWF4V2lkdGgiOm51bGwsIm1pbkhlaWdodCI6bnVsbCwibWF4SGVpZ2h0IjpudWxsfSx7IndpZHRoIjoxMDAsImhlaWdodCI6MTAwLCJtaW5XaWR0aCI6bnVsbCwibWF4V2lkdGgiOm51bGwsIm1pbkhlaWdodCI6bnVsbCwibWF4SGVpZ2h0IjpudWxsfSx7IndpZHRoIjoxMDAsImhlaWdodCI6MTAwLCJtaW5XaWR0aCI6bnVsbCwibWF4V2lkdGgiOm51bGwsIm1pbkhlaWdodCI6bnVsbCwibWF4SGVpZ2h0IjpudWxsfSx7IndpZHRoIjoxMDAsImhlaWdodCI6MTAwLCJtaW5XaWR0aCI6bnVsbCwibWF4V2lkdGgiOm51bGwsIm1pbkhlaWdodCI6bnVsbCwibWF4SGVpZ2h0IjpudWxsfSx7IndpZHRoIjoxMDAsImhlaWdodCI6MTAwLCJtaW5XaWR0aCI6bnVsbCwibWF4V2lkdGgiOm51bGwsIm1pbkhlaWdodCI6bnVsbCwibWF4SGVpZ2h0IjpudWxsfSx7IndpZHRoIjoxMDAsImhlaWdodCI6MTAwLCJtaW5XaWR0aCI6bnVsbCwibWF4V2lkdGgiOm51bGwsIm1pbkhlaWdodCI6bnVsbCwibWF4SGVpZ2h0IjpudWxsfSx7IndpZHRoIjoxMDAsImhlaWdodCI6MTAwLCJtaW5XaWR0aCI6bnVsbCwibWF4V2lkdGgiOm51bGwsIm1pbkhlaWdodCI6bnVsbCwibWF4SGVpZ2h0IjpudWxsfSx7IndpZHRoIjoxMDAsImhlaWdodCI6MTAwLCJtaW5XaWR0aCI6bnVsbCwibWF4V2lkdGgiOm51bGwsIm1pbkhlaWdodCI6bnVsbCwibWF4SGVpZ2h0IjpudWxsfSx7IndpZHRoIjoxMDAsImhlaWdodCI6MTAwLCJtaW5XaWR0aCI6bnVsbCwibWF4V2lkdGgiOm51bGwsIm1pbkhlaWdodCI6bnVsbCwibWF4SGVpZ2h0IjpudWxsfSx7IndpZHRoIjoxMDAsImhlaWdodCI6MTAwLCJhbGlnbkNvbnRlbnQiOjIsIm1pbldpZHRoIjpudWxsLCJtYXhXaWR0aCI6bnVsbCwibWluSGVpZ2h0IjpudWxsLCJtYXhIZWlnaHQiOm51bGx9XSwibWluV2lkdGgiOm51bGwsIm1heFdpZHRoIjpudWxsLCJtaW5IZWlnaHQiOm51bGwsIm1heEhlaWdodCI6bnVsbH0=
---

## Align Content

Align content defines the distribution of lines along the cross-axis. This only
has effect when items are wrapped to multiple lines using [`flex wrap`](/docs/flex-wrap).

컨텐츠 Align은 교차축(cross-axis)을 따라 선이 배치되는 것을 정의한다. 이는 아이템들이 여러개의 선으로
묶여있을 때만 효과가 있습니다. 

**FLEX START (DEFAULT)** Align wrapped lines to the start of the container's cross axis.
**FLEX START (DEFAULT)** 아이템들을 containor의 cross-axis 시작부분에 정렬시킨다.

**FLEX END** Align wrapped lines to the end of the container's cross axis.
**FLEX END** 아이템들을 containor의 cross-axis 끝부분에 정렬시킨다.

**STRETCH** Stretch wrapped lines to match the `height` of the container's cross axis.
**STRETCH** containor의 cross-axis 높이에 균등하게 아이템들을 정렬시킨다.

**CENTER** Align wrapped lines in the center of the container's cross axis.
**CENTER** containor의 cross-axis 중앙에 아이템들을 정렬시킨다.

**SPACE BETWEEN** Evenly space wrapped lines across the container's main axis, distributing
remaining space between the lines.
**SPACE BETWEEN** containor의 cross-axis 시작과 끝에 걸쳐 아이템을 정렬시킨다.

**SPACE AROUND** Evenly space wrapped lines across the container's main axis, distributing
remaining space around the lines. Compared to `space between` using
`space around` will result in space being distributed to the begining of
the first lines and end of the last line.
**SPACE AROUND** containor의 cross-axis 시작부터 끝에 걸쳐 균등하게 나뉜 공간에 아이템을 정렬시킨다. 
'SPACE BETWEEN'과 비교했을 때의 차이점이 있다면 아이템이 시작하기 전과 끝난 후에도 공간이 분배된다는 점이다.

<controls prop="alignContent"></controls>
