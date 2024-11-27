`sm:` is 超過 640px 的螢幕都會套用這樣式。 (>= 640px 的意思)

```css
@media (min-width: 640px) {
  /* CSS rules for screens that are 600px or less */
}
```

預設是 gray-200，sm 是 yellow-300，md 是 blue-300，lg 是 green-300，xl 是 pink-300，2xl 是 red-300。

```html
<body
  class="bg-gray-200 sm:bg-yellow-300 md:bg-blue-300 lg:bg-green-300 xl:bg-pink-300 2xl:bg-red-300"
></body>
```

---

bradgashler.htmltagwrap

A quick search on the Visual Studio Code marketplace: htmltagwrap.

Launch Visual Studio Code Quick Open (Ctrl + P)

Paste ext install htmltagwrap and Enter.

Select HTML

press Alt + W (Option + W for Mac).

---

Select All Occurrences of Find Match editor.action.selectHighlights.

Ctrl+Shift+L

Cmd+Shift+L or Cmd+Ctrl+G on Mac

---

Ctrl+Shift+L to select all occurrences of current selection

and

Ctrl+F2 to select all occurrences of current word

---

Multiple selections (multi-cursor)

VS Code supports multiple cursors for fast simultaneous edits. You can add secondary cursors (rendered thinner) with Alt+Click. Each cursor operates independently based on the context it sits in. A common way to add more cursors is with Ctrl+Alt+Down or Ctrl+Alt+Up that insert cursors below or above.

https://code.visualstudio.com/docs/editor/codebasics#_multiple-selections-multicursor

https://www.youtube.com/watch?v=hX1zUdj4Dw4&list=PL5f_mz_zU5eXWYDXHUDOLBE0scnuJofO0&index=4

---

 select the current word

On Mac OS: Cmd+D
On Windows & Linux: Ctrl+D

OR

You are looking for Shrink/Expand Selection.

Trigger it with Shift+Alt+Left and Shift + Alt +Right

---

Shift + UpArrow/DownArrow - this text line by line

Shift +  LefeArrow/RightArrow - select text character by character

Ctrl + BackSpace - this will delete text word by word