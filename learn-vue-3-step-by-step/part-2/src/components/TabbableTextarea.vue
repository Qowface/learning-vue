<script setup>
function onTabPress(e) {
  let textarea = e.target

  // get caret position/selection
  let val = textarea.value
  let start = textarea.selectionStart
  let end = textarea.selectionEnd

  // set textarea value to: text before caret + tab + text after caret
  textarea.value = val.substring(0, start) + '\t' + val.substring(end)

  // put caret at right position again
  textarea.selectionStart = textarea.selectionEnd = start + 1
}
</script>

<template>
  <textarea @keydown.tab.prevent="onTabPress"></textarea>
</template>
