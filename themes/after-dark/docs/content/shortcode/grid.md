+++
title = "Grid"
description = "Display a responsive grid with cells."
categories = ["experience"]
tags = []
html_attributes = ["class"]
custom_attributes = []
snippets_used = ["cell", "card", "button"]
[[copyright]]
  owner = "Josh Habdas"
  date = "2019"
  license = "agpl-3.0-or-later"
+++

Containing three [Cell](../cell) of equal size:

{{< highlight html "linenos=inline" >}}
{{</* hackcss-grid >}}
  {{< hackcss-cell class="-4of12" text="4" />}}
  {{< hackcss-cell class="-4of12" text="4" />}}
  {{< hackcss-cell class="-4of12" text="4" />}}
{{< /hackcss-grid */>}}
{{< /highlight >}}

{{< hackcss-grid class="unset-margin" >}}
  {{< hackcss-cell class="-4of12" text="4" />}}
  {{< hackcss-cell class="-4of12" text="4" />}}
  {{< hackcss-cell class="-4of12" text="4" />}}
{{< /hackcss-grid >}}

With two columns of odd size:

```html
{{</* hackcss-grid >}}
  {{< hackcss-cell class="-4of12" text="4" />}}
  {{< hackcss-cell class="-8of12" text="8" />}}
{{< /hackcss-grid */>}}
```

{{< hackcss-grid class="example" >}}
  {{< hackcss-cell class="-4of12" text="4" />}}
  {{< hackcss-cell class="-8of12" text="8" />}}
{{< /hackcss-grid >}}

With 12 columns:

```html
{{</* hackcss-grid >}}
  {{< hackcss-cell class="-1of12" text="1" />}}
  {{< hackcss-cell class="-1of12" text="1" />}}
  {{< hackcss-cell class="-1of12" text="1" />}}
  {{< hackcss-cell class="-1of12" text="1" />}}
  {{< hackcss-cell class="-1of12" text="1" />}}
  {{< hackcss-cell class="-1of12" text="1" />}}
  {{< hackcss-cell class="-1of12" text="1" />}}
  {{< hackcss-cell class="-1of12" text="1" />}}
  {{< hackcss-cell class="-1of12" text="1" />}}
  {{< hackcss-cell class="-1of12" text="1" />}}
  {{< hackcss-cell class="-1of12" text="1" />}}
  {{< hackcss-cell class="-1of12" text="1" />}}
{{< /hackcss-grid */>}}
```

{{< hackcss-grid >}}
  {{< hackcss-cell class="-1of12" text="1" />}}
  {{< hackcss-cell class="-1of12" text="1" />}}
  {{< hackcss-cell class="-1of12" text="1" />}}
  {{< hackcss-cell class="-1of12" text="1" />}}
  {{< hackcss-cell class="-1of12" text="1" />}}
  {{< hackcss-cell class="-1of12" text="1" />}}
  {{< hackcss-cell class="-1of12" text="1" />}}
  {{< hackcss-cell class="-1of12" text="1" />}}
  {{< hackcss-cell class="-1of12" text="1" />}}
  {{< hackcss-cell class="-1of12" text="1" />}}
  {{< hackcss-cell class="-1of12" text="1" />}}
  {{< hackcss-cell class="-1of12" text="1" />}}
{{< /hackcss-grid >}}

Enclosing [Cards](../card/) with various [Buttons](../button/) inside:

```html
{{</* hackcss-grid >}}
  {{< hackcss-cell class="-4of12" >}}
    {{< hackcss-card header="Step 1" >}}
      {{< hackcss-button type="primary" isblock="true" isghost="true" >}}
        <svg id="i-download" viewBox="0 0 32 32" width="24" height="24" fill="none" stroke="currentcolor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2">
          <path d="M9 22 C0 23 1 12 9 13 6 2 23 2 22 10 32 7 32 23 23 22 M11 26 L16 30 21 26 M16 16 L16 30"></path>
        </svg>&nbsp;&nbsp;Download
      {{< /hackcss-button >}}
    {{< /hackcss-card >}}
  {{< /hackcss-cell >}}
  {{< hackcss-cell class="-4of12" >}}
    {{< hackcss-card header="Step 2" >}}
      {{< hackcss-button type="info" isblock="true" isghost="true" >}}
        <svg id="i-code" aria-labelledby="source-label" viewBox="0 0 32 32" width="24" height="24" fill="none" stroke="currentcolor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2">
          <path d="M10 9 L3 17 10 25 M22 9 L29 17 22 25 M18 7 L14 27" />
        </svg>&nbsp;&nbsp;Install
      {{< /hackcss-button >}}
    {{< /hackcss-card >}}
  {{< /hackcss-cell >}}
  {{< hackcss-cell class="-4of12" >}}
    {{< hackcss-card header="Step 3" >}}
      {{< hackcss-button type="success" isblock="true" isghost="true" >}}
        <svg id="i-creditcard" viewBox="0 0 32 32" width="24" height="24" fill="none" stroke="currentcolor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2">
          <path d="M2 7 L2 25 30 25 30 7 Z M5 18 L9 18 M5 21 L11 21" />
          <path d="M2 11 L2 13 30 13 30 11 Z" fill="currentColor" />
        </svg>&nbsp;&nbsp;Profit
      {{< /hackcss-button >}}
    {{< /hackcss-card >}}
  {{< /hackcss-cell >}}
{{< /hackcss-grid */>}}
```

{{< hackcss-grid >}}
  {{< hackcss-cell class="-4of12" >}}
    {{< hackcss-card header="Step 1" >}}
      {{< hackcss-button type="primary" isblock="true" isghost="true" >}}
        <svg id="i-download" viewBox="0 0 32 32" width="24" height="24" fill="none" stroke="currentcolor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2">
          <path d="M9 22 C0 23 1 12 9 13 6 2 23 2 22 10 32 7 32 23 23 22 M11 26 L16 30 21 26 M16 16 L16 30"></path>
        </svg>&nbsp;&nbsp;Download
      {{< /hackcss-button >}}
    {{< /hackcss-card >}}
  {{< /hackcss-cell >}}
  {{< hackcss-cell class="-4of12" >}}
    {{< hackcss-card header="Step 2" >}}
      {{< hackcss-button type="info" isblock="true" isghost="true" >}}
        <svg id="i-code" aria-labelledby="source-label" viewBox="0 0 32 32" width="24" height="24" fill="none" stroke="currentcolor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2">
          <path d="M10 9 L3 17 10 25 M22 9 L29 17 22 25 M18 7 L14 27" />
        </svg>&nbsp;&nbsp;Install
      {{< /hackcss-button >}}
    {{< /hackcss-card >}}
  {{< /hackcss-cell >}}
  {{< hackcss-cell class="-4of12" >}}
    {{< hackcss-card header="Step 3" >}}
      {{< hackcss-button type="success" isblock="true" isghost="true" >}}
        <svg id="i-creditcard" viewBox="0 0 32 32" width="24" height="24" fill="none" stroke="currentcolor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2">
          <path d="M2 7 L2 25 30 25 30 7 Z M5 18 L9 18 M5 21 L11 21" />
          <path d="M2 11 L2 13 30 13 30 11 Z" fill="currentColor" />
        </svg>&nbsp;&nbsp;Profit
      {{< /hackcss-button >}}
    {{< /hackcss-card >}}
  {{< /hackcss-cell >}}
{{< /hackcss-grid >}}

Aligning three [SVG Favicons]({{< relref "svg-favicon" >}}) using `-around` modifier:

```html
{{</* hackcss-grid class="-around" >}}
  {{< hackcss-cell class="-2of12" >}}
    <img src="data:image/svg+xml,%3Csvg%20viewBox='0%200%2046%2045'%20xmlns='http://www.w3.org/2000/svg'%3E%3Ctitle%3EAfter%20Dark%3C/title%3E%3Cpath%20d='M.708%2045L23%20.416%2045.292%2045H.708zM35%2038L23%2019%2011%2038h24z'%20fill='%23f00'/%3E%3C/svg%3E">
  {{< /hackcss-cell >}}
  {{< hackcss-cell class="-2of12" >}}
    <img src="data:image/svg+xml,%3Csvg%20viewBox='0%200%2046%2045'%20xmlns='http://www.w3.org/2000/svg'%3E%3Ctitle%3EAfter%20Dark%3C/title%3E%3Cpath%20d='M.708%2045L23%20.416%2045.292%2045H.708zM35%2038L23%2019%2011%2038h24z'%20fill='lime'/%3E%3C/svg%3E">
  {{< /hackcss-cell >}}
  {{< hackcss-cell class="-2of12" >}}
    <img src="data:image/svg+xml,%3Csvg%20viewBox='0%200%2046%2045'%20xmlns='http://www.w3.org/2000/svg'%3E%3Ctitle%3EAfter%20Dark%3C/title%3E%3Cpath%20d='M.708%2045L23%20.416%2045.292%2045H.708zM35%2038L23%2019%2011%2038h24z'%20fill='%2300f'/%3E%3C/svg%3E">
  {{< /hackcss-cell >}}
{{< /hackcss-grid */>}}
```

{{< hackcss-grid class="-around" >}}
  {{< hackcss-cell class="-2of12" >}}
    <img src="data:image/svg+xml,%3Csvg%20viewBox='0%200%2046%2045'%20xmlns='http://www.w3.org/2000/svg'%3E%3Ctitle%3EAfter%20Dark%3C/title%3E%3Cpath%20d='M.708%2045L23%20.416%2045.292%2045H.708zM35%2038L23%2019%2011%2038h24z'%20fill='%23f00'/%3E%3C/svg%3E">
  {{< /hackcss-cell >}}
  {{< hackcss-cell class="-2of12" >}}
    <img src="data:image/svg+xml,%3Csvg%20viewBox='0%200%2046%2045'%20xmlns='http://www.w3.org/2000/svg'%3E%3Ctitle%3EAfter%20Dark%3C/title%3E%3Cpath%20d='M.708%2045L23%20.416%2045.292%2045H.708zM35%2038L23%2019%2011%2038h24z'%20fill='lime'/%3E%3C/svg%3E">
  {{< /hackcss-cell >}}
  {{< hackcss-cell class="-2of12" >}}
    <img src="data:image/svg+xml,%3Csvg%20viewBox='0%200%2046%2045'%20xmlns='http://www.w3.org/2000/svg'%3E%3Ctitle%3EAfter%20Dark%3C/title%3E%3Cpath%20d='M.708%2045L23%20.416%2045.292%2045H.708zM35%2038L23%2019%2011%2038h24z'%20fill='%2300f'/%3E%3C/svg%3E">
  {{< /hackcss-cell >}}
{{< /hackcss-grid >}}

See the {{< external text="hackcss" href="https://hackcss.egoist.moe/" />}} docs for full list of flexbox modifiers available. Reference the following resources for additional help:

- {{< external "https://philipwalton.github.io/solved-by-flexbox/" "Solved by Flexbox" />}} for cleaner, hack-free CSS
- {{< external "https://www.w3.org/TR/css-flexbox-1/" "CSS Flexible Box Layout Module" />}} for Level 1 spec on W3C
