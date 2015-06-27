atom编辑器
=================

今天在github上看到他推荐的编辑器.
试用了一下, 感觉不错.
把配置记录到下面


config
=====================

"*":
  "exception-reporting":
    userId: "2d59eb64-8971-3550-ee30-874a9f534ce2"
  welcome:
    showOnStartup: false
  core:
    projectHome: "e:\\project\\"
    themes: [
      "one-light-ui"
      "one-light-syntax"
    ]
  editor:
    invisibles: {}
    fontFamily: "consolas"
    fontSize: 25
    showIndentGuide: true
    softWrap: true
    softWrapAtPreferredLineLength: true
    tabLength: 4
  "autocomplete-plus": {}
  autosave:
    enabled: true
  "bracket-matcher":
    wrapSelectionsInBrackets: false
  "tree-view": {}
  tabs:
    enableVcsColoring: true
  "status-bar": {}
  "spell-check": {}
  "markdown-preview": {}
  whitespace:
    ensureSingleTrailingNewline: false
    ignoreWhitespaceOnCurrentLine: false
  "color-picker":
    preferredFormat: "HEX"





keymap
=============

'atom-workspace atom-text-editor:not([mini])':
  'alt-down': 'editor:move-line-down'
  'alt-up': 'editor:move-line-up'

  'alt-1': 'editor:toggle-line-comments'
  'ctrl-enter': 'unset!'


'.platform-win32 atom-text-editor, .platform-linux atom-text-editor':
  'f3': 'unset!'


'atom-text-editor':
  'alt-h': 'unset!'
  'shift-enter': 'editor:move-to-end-of-screen-line'
  'alt-;': 'editor:move-to-first-character-of-line'
  'alt-/': 'autocomplete-plus:activate'
  'alt-3': 'bracket-matcher:go-to-matching-bracket'
  'f2': 'unset!'
  'alt-d': 'unset!'

'body':
  'alt-h': 'core:move-left'
  'alt-l': 'core:move-right'
  'alt-k': 'core:move-up'
  'alt-j': 'core:move-down'
  'alt-s': 'core:backspace'
  'alt-d': 'core:delete'
  'ctrl-k h': 'pane:split-left'
  'ctrl-k j': 'pane:split-down'
  'ctrl-k k': 'pane:split-up'
  'ctrl-k l': 'pane:split-right'
  'f2': 'pane:show-previous-item'
  'f3': 'pane:show-next-item'


'atom-text-editor:not([mini])':
  'ctrl-d': 'editor:delete-line'


'atom-workspace, atom-workspace atom-text-editor':
  'ctrl-m k': 'markdown-preview:toggle'
