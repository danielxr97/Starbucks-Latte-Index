<!DOCTYPE html>

<html lang="en">
<head><meta charset="utf-8"/>
<meta content="width=device-width, initial-scale=1.0" name="viewport"/>
<title>drabi_a3</title><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script>
<style type="text/css">
    pre { line-height: 125%; }
td.linenos .normal { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
span.linenos { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
td.linenos .special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
span.linenos.special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
.highlight .hll { background-color: var(--jp-cell-editor-active-background) }
.highlight { background: var(--jp-cell-editor-background); color: var(--jp-mirror-editor-variable-color) }
.highlight .c { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment */
.highlight .err { color: var(--jp-mirror-editor-error-color) } /* Error */
.highlight .k { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword */
.highlight .o { color: var(--jp-mirror-editor-operator-color); font-weight: bold } /* Operator */
.highlight .p { color: var(--jp-mirror-editor-punctuation-color) } /* Punctuation */
.highlight .ch { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Hashbang */
.highlight .cm { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Multiline */
.highlight .cp { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Preproc */
.highlight .cpf { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.PreprocFile */
.highlight .c1 { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Single */
.highlight .cs { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Special */
.highlight .kc { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Constant */
.highlight .kd { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Declaration */
.highlight .kn { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Namespace */
.highlight .kp { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Pseudo */
.highlight .kr { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Reserved */
.highlight .kt { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Type */
.highlight .m { color: var(--jp-mirror-editor-number-color) } /* Literal.Number */
.highlight .s { color: var(--jp-mirror-editor-string-color) } /* Literal.String */
.highlight .ow { color: var(--jp-mirror-editor-operator-color); font-weight: bold } /* Operator.Word */
.highlight .pm { color: var(--jp-mirror-editor-punctuation-color) } /* Punctuation.Marker */
.highlight .w { color: var(--jp-mirror-editor-variable-color) } /* Text.Whitespace */
.highlight .mb { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Bin */
.highlight .mf { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Float */
.highlight .mh { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Hex */
.highlight .mi { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Integer */
.highlight .mo { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Oct */
.highlight .sa { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Affix */
.highlight .sb { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Backtick */
.highlight .sc { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Char */
.highlight .dl { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Delimiter */
.highlight .sd { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Doc */
.highlight .s2 { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Double */
.highlight .se { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Escape */
.highlight .sh { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Heredoc */
.highlight .si { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Interpol */
.highlight .sx { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Other */
.highlight .sr { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Regex */
.highlight .s1 { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Single */
.highlight .ss { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Symbol */
.highlight .il { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Integer.Long */
  </style>
<style type="text/css">
/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*
 * Mozilla scrollbar styling
 */

/* use standard opaque scrollbars for most nodes */
[data-jp-theme-scrollbars='true'] {
  scrollbar-color: rgb(var(--jp-scrollbar-thumb-color))
    var(--jp-scrollbar-background-color);
}

/* for code nodes, use a transparent style of scrollbar. These selectors
 * will match lower in the tree, and so will override the above */
[data-jp-theme-scrollbars='true'] .CodeMirror-hscrollbar,
[data-jp-theme-scrollbars='true'] .CodeMirror-vscrollbar {
  scrollbar-color: rgba(var(--jp-scrollbar-thumb-color), 0.5) transparent;
}

/* tiny scrollbar */

.jp-scrollbar-tiny {
  scrollbar-color: rgba(var(--jp-scrollbar-thumb-color), 0.5) transparent;
  scrollbar-width: thin;
}

/* tiny scrollbar */

.jp-scrollbar-tiny::-webkit-scrollbar,
.jp-scrollbar-tiny::-webkit-scrollbar-corner {
  background-color: transparent;
  height: 4px;
  width: 4px;
}

.jp-scrollbar-tiny::-webkit-scrollbar-thumb {
  background: rgba(var(--jp-scrollbar-thumb-color), 0.5);
}

.jp-scrollbar-tiny::-webkit-scrollbar-track:horizontal {
  border-left: 0 solid transparent;
  border-right: 0 solid transparent;
}

.jp-scrollbar-tiny::-webkit-scrollbar-track:vertical {
  border-top: 0 solid transparent;
  border-bottom: 0 solid transparent;
}

/*
 * Lumino
 */

.lm-ScrollBar[data-orientation='horizontal'] {
  min-height: 16px;
  max-height: 16px;
  min-width: 45px;
  border-top: 1px solid #a0a0a0;
}

.lm-ScrollBar[data-orientation='vertical'] {
  min-width: 16px;
  max-width: 16px;
  min-height: 45px;
  border-left: 1px solid #a0a0a0;
}

.lm-ScrollBar-button {
  background-color: #f0f0f0;
  background-position: center center;
  min-height: 15px;
  max-height: 15px;
  min-width: 15px;
  max-width: 15px;
}

.lm-ScrollBar-button:hover {
  background-color: #dadada;
}

.lm-ScrollBar-button.lm-mod-active {
  background-color: #cdcdcd;
}

.lm-ScrollBar-track {
  background: #f0f0f0;
}

.lm-ScrollBar-thumb {
  background: #cdcdcd;
}

.lm-ScrollBar-thumb:hover {
  background: #bababa;
}

.lm-ScrollBar-thumb.lm-mod-active {
  background: #a0a0a0;
}

.lm-ScrollBar[data-orientation='horizontal'] .lm-ScrollBar-thumb {
  height: 100%;
  min-width: 15px;
  border-left: 1px solid #a0a0a0;
  border-right: 1px solid #a0a0a0;
}

.lm-ScrollBar[data-orientation='vertical'] .lm-ScrollBar-thumb {
  width: 100%;
  min-height: 15px;
  border-top: 1px solid #a0a0a0;
  border-bottom: 1px solid #a0a0a0;
}

.lm-ScrollBar[data-orientation='horizontal']
  .lm-ScrollBar-button[data-action='decrement'] {
  background-image: var(--jp-icon-caret-left);
  background-size: 17px;
}

.lm-ScrollBar[data-orientation='horizontal']
  .lm-ScrollBar-button[data-action='increment'] {
  background-image: var(--jp-icon-caret-right);
  background-size: 17px;
}

.lm-ScrollBar[data-orientation='vertical']
  .lm-ScrollBar-button[data-action='decrement'] {
  background-image: var(--jp-icon-caret-up);
  background-size: 17px;
}

.lm-ScrollBar[data-orientation='vertical']
  .lm-ScrollBar-button[data-action='increment'] {
  background-image: var(--jp-icon-caret-down);
  background-size: 17px;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-Widget {
  box-sizing: border-box;
  position: relative;
  overflow: hidden;
}

.lm-Widget.lm-mod-hidden {
  display: none !important;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.lm-AccordionPanel[data-orientation='horizontal'] > .lm-AccordionPanel-title {
  /* Title is rotated for horizontal accordion panel using CSS */
  display: block;
  transform-origin: top left;
  transform: rotate(-90deg) translate(-100%);
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-CommandPalette {
  display: flex;
  flex-direction: column;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-CommandPalette-search {
  flex: 0 0 auto;
}

.lm-CommandPalette-content {
  flex: 1 1 auto;
  margin: 0;
  padding: 0;
  min-height: 0;
  overflow: auto;
  list-style-type: none;
}

.lm-CommandPalette-header {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.lm-CommandPalette-item {
  display: flex;
  flex-direction: row;
}

.lm-CommandPalette-itemIcon {
  flex: 0 0 auto;
}

.lm-CommandPalette-itemContent {
  flex: 1 1 auto;
  overflow: hidden;
}

.lm-CommandPalette-itemShortcut {
  flex: 0 0 auto;
}

.lm-CommandPalette-itemLabel {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.lm-close-icon {
  border: 1px solid transparent;
  background-color: transparent;
  position: absolute;
  z-index: 1;
  right: 3%;
  top: 0;
  bottom: 0;
  margin: auto;
  padding: 7px 0;
  display: none;
  vertical-align: middle;
  outline: 0;
  cursor: pointer;
}
.lm-close-icon:after {
  content: 'X';
  display: block;
  width: 15px;
  height: 15px;
  text-align: center;
  color: #000;
  font-weight: normal;
  font-size: 12px;
  cursor: pointer;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-DockPanel {
  z-index: 0;
}

.lm-DockPanel-widget {
  z-index: 0;
}

.lm-DockPanel-tabBar {
  z-index: 1;
}

.lm-DockPanel-handle {
  z-index: 2;
}

.lm-DockPanel-handle.lm-mod-hidden {
  display: none !important;
}

.lm-DockPanel-handle:after {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  content: '';
}

.lm-DockPanel-handle[data-orientation='horizontal'] {
  cursor: ew-resize;
}

.lm-DockPanel-handle[data-orientation='vertical'] {
  cursor: ns-resize;
}

.lm-DockPanel-handle[data-orientation='horizontal']:after {
  left: 50%;
  min-width: 8px;
  transform: translateX(-50%);
}

.lm-DockPanel-handle[data-orientation='vertical']:after {
  top: 50%;
  min-height: 8px;
  transform: translateY(-50%);
}

.lm-DockPanel-overlay {
  z-index: 3;
  box-sizing: border-box;
  pointer-events: none;
}

.lm-DockPanel-overlay.lm-mod-hidden {
  display: none !important;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-Menu {
  z-index: 10000;
  position: absolute;
  white-space: nowrap;
  overflow-x: hidden;
  overflow-y: auto;
  outline: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-Menu-content {
  margin: 0;
  padding: 0;
  display: table;
  list-style-type: none;
}

.lm-Menu-item {
  display: table-row;
}

.lm-Menu-item.lm-mod-hidden,
.lm-Menu-item.lm-mod-collapsed {
  display: none !important;
}

.lm-Menu-itemIcon,
.lm-Menu-itemSubmenuIcon {
  display: table-cell;
  text-align: center;
}

.lm-Menu-itemLabel {
  display: table-cell;
  text-align: left;
}

.lm-Menu-itemShortcut {
  display: table-cell;
  text-align: right;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-MenuBar {
  outline: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-MenuBar-content {
  margin: 0;
  padding: 0;
  display: flex;
  flex-direction: row;
  list-style-type: none;
}

.lm-MenuBar-item {
  box-sizing: border-box;
}

.lm-MenuBar-itemIcon,
.lm-MenuBar-itemLabel {
  display: inline-block;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-ScrollBar {
  display: flex;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-ScrollBar[data-orientation='horizontal'] {
  flex-direction: row;
}

.lm-ScrollBar[data-orientation='vertical'] {
  flex-direction: column;
}

.lm-ScrollBar-button {
  box-sizing: border-box;
  flex: 0 0 auto;
}

.lm-ScrollBar-track {
  box-sizing: border-box;
  position: relative;
  overflow: hidden;
  flex: 1 1 auto;
}

.lm-ScrollBar-thumb {
  box-sizing: border-box;
  position: absolute;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-SplitPanel-child {
  z-index: 0;
}

.lm-SplitPanel-handle {
  z-index: 1;
}

.lm-SplitPanel-handle.lm-mod-hidden {
  display: none !important;
}

.lm-SplitPanel-handle:after {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  content: '';
}

.lm-SplitPanel[data-orientation='horizontal'] > .lm-SplitPanel-handle {
  cursor: ew-resize;
}

.lm-SplitPanel[data-orientation='vertical'] > .lm-SplitPanel-handle {
  cursor: ns-resize;
}

.lm-SplitPanel[data-orientation='horizontal'] > .lm-SplitPanel-handle:after {
  left: 50%;
  min-width: 8px;
  transform: translateX(-50%);
}

.lm-SplitPanel[data-orientation='vertical'] > .lm-SplitPanel-handle:after {
  top: 50%;
  min-height: 8px;
  transform: translateY(-50%);
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-TabBar {
  display: flex;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-TabBar[data-orientation='horizontal'] {
  flex-direction: row;
  align-items: flex-end;
}

.lm-TabBar[data-orientation='vertical'] {
  flex-direction: column;
  align-items: flex-end;
}

.lm-TabBar-content {
  margin: 0;
  padding: 0;
  display: flex;
  flex: 1 1 auto;
  list-style-type: none;
}

.lm-TabBar[data-orientation='horizontal'] > .lm-TabBar-content {
  flex-direction: row;
}

.lm-TabBar[data-orientation='vertical'] > .lm-TabBar-content {
  flex-direction: column;
}

.lm-TabBar-tab {
  display: flex;
  flex-direction: row;
  box-sizing: border-box;
  overflow: hidden;
  touch-action: none; /* Disable native Drag/Drop */
}

.lm-TabBar-tabIcon,
.lm-TabBar-tabCloseIcon {
  flex: 0 0 auto;
}

.lm-TabBar-tabLabel {
  flex: 1 1 auto;
  overflow: hidden;
  white-space: nowrap;
}

.lm-TabBar-tabInput {
  user-select: all;
  width: 100%;
  box-sizing: border-box;
}

.lm-TabBar-tab.lm-mod-hidden {
  display: none !important;
}

.lm-TabBar-addButton.lm-mod-hidden {
  display: none !important;
}

.lm-TabBar.lm-mod-dragging .lm-TabBar-tab {
  position: relative;
}

.lm-TabBar.lm-mod-dragging[data-orientation='horizontal'] .lm-TabBar-tab {
  left: 0;
  transition: left 150ms ease;
}

.lm-TabBar.lm-mod-dragging[data-orientation='vertical'] .lm-TabBar-tab {
  top: 0;
  transition: top 150ms ease;
}

.lm-TabBar.lm-mod-dragging .lm-TabBar-tab.lm-mod-dragging {
  transition: none;
}

.lm-TabBar-tabLabel .lm-TabBar-tabInput {
  user-select: all;
  width: 100%;
  box-sizing: border-box;
  background: inherit;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-TabPanel-tabBar {
  z-index: 1;
}

.lm-TabPanel-stackedPanel {
  z-index: 0;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Collapse {
  display: flex;
  flex-direction: column;
  align-items: stretch;
}

.jp-Collapse-header {
  padding: 1px 12px;
  background-color: var(--jp-layout-color1);
  border-bottom: solid var(--jp-border-width) var(--jp-border-color2);
  color: var(--jp-ui-font-color1);
  cursor: pointer;
  display: flex;
  align-items: center;
  font-size: var(--jp-ui-font-size0);
  font-weight: 600;
  text-transform: uppercase;
  user-select: none;
}

.jp-Collapser-icon {
  height: 16px;
}

.jp-Collapse-header-collapsed .jp-Collapser-icon {
  transform: rotate(-90deg);
  margin: auto 0;
}

.jp-Collapser-title {
  line-height: 25px;
}

.jp-Collapse-contents {
  padding: 0 12px;
  background-color: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  overflow: auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* This file was auto-generated by ensureUiComponents() in @jupyterlab/buildutils */

/**
 * (DEPRECATED) Support for consuming icons as CSS background images
 */

/* Icons urls */

:root {
  --jp-icon-add-above: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPGcgY2xpcC1wYXRoPSJ1cmwoI2NsaXAwXzEzN18xOTQ5MikiPgo8cGF0aCBjbGFzcz0ianAtaWNvbjMiIGQ9Ik00Ljc1IDQuOTMwNjZINi42MjVWNi44MDU2NkM2LjYyNSA3LjAxMTkxIDYuNzkzNzUgNy4xODA2NiA3IDcuMTgwNjZDNy4yMDYyNSA3LjE4MDY2IDcuMzc1IDcuMDExOTEgNy4zNzUgNi44MDU2NlY0LjkzMDY2SDkuMjVDOS40NTYyNSA0LjkzMDY2IDkuNjI1IDQuNzYxOTEgOS42MjUgNC41NTU2NkM5LjYyNSA0LjM0OTQxIDkuNDU2MjUgNC4xODA2NiA5LjI1IDQuMTgwNjZINy4zNzVWMi4zMDU2NkM3LjM3NSAyLjA5OTQxIDcuMjA2MjUgMS45MzA2NiA3IDEuOTMwNjZDNi43OTM3NSAxLjkzMDY2IDYuNjI1IDIuMDk5NDEgNi42MjUgMi4zMDU2NlY0LjE4MDY2SDQuNzVDNC41NDM3NSA0LjE4MDY2IDQuMzc1IDQuMzQ5NDEgNC4zNzUgNC41NTU2NkM0LjM3NSA0Ljc2MTkxIDQuNTQzNzUgNC45MzA2NiA0Ljc1IDQuOTMwNjZaIiBmaWxsPSIjNjE2MTYxIiBzdHJva2U9IiM2MTYxNjEiIHN0cm9rZS13aWR0aD0iMC43Ii8+CjwvZz4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGNsaXAtcnVsZT0iZXZlbm9kZCIgZD0iTTExLjUgOS41VjExLjVMMi41IDExLjVWOS41TDExLjUgOS41Wk0xMiA4QzEyLjU1MjMgOCAxMyA4LjQ0NzcyIDEzIDlWMTJDMTMgMTIuNTUyMyAxMi41NTIzIDEzIDEyIDEzTDIgMTNDMS40NDc3MiAxMyAxIDEyLjU1MjMgMSAxMlY5QzEgOC40NDc3MiAxLjQ0NzcxIDggMiA4TDEyIDhaIiBmaWxsPSIjNjE2MTYxIi8+CjxkZWZzPgo8Y2xpcFBhdGggaWQ9ImNsaXAwXzEzN18xOTQ5MiI+CjxyZWN0IGNsYXNzPSJqcC1pY29uMyIgd2lkdGg9IjYiIGhlaWdodD0iNiIgZmlsbD0id2hpdGUiIHRyYW5zZm9ybT0ibWF0cml4KC0xIDAgMCAxIDEwIDEuNTU1NjYpIi8+CjwvY2xpcFBhdGg+CjwvZGVmcz4KPC9zdmc+Cg==);
  --jp-icon-add-below: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPGcgY2xpcC1wYXRoPSJ1cmwoI2NsaXAwXzEzN18xOTQ5OCkiPgo8cGF0aCBjbGFzcz0ianAtaWNvbjMiIGQ9Ik05LjI1IDEwLjA2OTNMNy4zNzUgMTAuMDY5M0w3LjM3NSA4LjE5NDM0QzcuMzc1IDcuOTg4MDkgNy4yMDYyNSA3LjgxOTM0IDcgNy44MTkzNEM2Ljc5Mzc1IDcuODE5MzQgNi42MjUgNy45ODgwOSA2LjYyNSA4LjE5NDM0TDYuNjI1IDEwLjA2OTNMNC43NSAxMC4wNjkzQzQuNTQzNzUgMTAuMDY5MyA0LjM3NSAxMC4yMzgxIDQuMzc1IDEwLjQ0NDNDNC4zNzUgMTAuNjUwNiA0LjU0Mzc1IDEwLjgxOTMgNC43NSAxMC44MTkzTDYuNjI1IDEwLjgxOTNMNi42MjUgMTIuNjk0M0M2LjYyNSAxMi45MDA2IDYuNzkzNzUgMTMuMDY5MyA3IDEzLjA2OTNDNy4yMDYyNSAxMy4wNjkzIDcuMzc1IDEyLjkwMDYgNy4zNzUgMTIuNjk0M0w3LjM3NSAxMC44MTkzTDkuMjUgMTAuODE5M0M5LjQ1NjI1IDEwLjgxOTMgOS42MjUgMTAuNjUwNiA5LjYyNSAxMC40NDQzQzkuNjI1IDEwLjIzODEgOS40NTYyNSAxMC4wNjkzIDkuMjUgMTAuMDY5M1oiIGZpbGw9IiM2MTYxNjEiIHN0cm9rZT0iIzYxNjE2MSIgc3Ryb2tlLXdpZHRoPSIwLjciLz4KPC9nPgo8cGF0aCBjbGFzcz0ianAtaWNvbjMiIGZpbGwtcnVsZT0iZXZlbm9kZCIgY2xpcC1ydWxlPSJldmVub2RkIiBkPSJNMi41IDUuNUwyLjUgMy41TDExLjUgMy41TDExLjUgNS41TDIuNSA1LjVaTTIgN0MxLjQ0NzcyIDcgMSA2LjU1MjI4IDEgNkwxIDNDMSAyLjQ0NzcyIDEuNDQ3NzIgMiAyIDJMMTIgMkMxMi41NTIzIDIgMTMgMi40NDc3MiAxMyAzTDEzIDZDMTMgNi41NTIyOSAxMi41NTIzIDcgMTIgN0wyIDdaIiBmaWxsPSIjNjE2MTYxIi8+CjxkZWZzPgo8Y2xpcFBhdGggaWQ9ImNsaXAwXzEzN18xOTQ5OCI+CjxyZWN0IGNsYXNzPSJqcC1pY29uMyIgd2lkdGg9IjYiIGhlaWdodD0iNiIgZmlsbD0id2hpdGUiIHRyYW5zZm9ybT0ibWF0cml4KDEgMS43NDg0NmUtMDcgMS43NDg0NmUtMDcgLTEgNCAxMy40NDQzKSIvPgo8L2NsaXBQYXRoPgo8L2RlZnM+Cjwvc3ZnPgo=);
  --jp-icon-add: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE5IDEzaC02djZoLTJ2LTZINXYtMmg2VjVoMnY2aDZ2MnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-bell: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE2IDE2IiB2ZXJzaW9uPSIxLjEiPgogICA8cGF0aCBjbGFzcz0ianAtaWNvbjIganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMzMzMzMzIgogICAgICBkPSJtOCAwLjI5Yy0xLjQgMC0yLjcgMC43My0zLjYgMS44LTEuMiAxLjUtMS40IDMuNC0xLjUgNS4yLTAuMTggMi4yLTAuNDQgNC0yLjMgNS4zbDAuMjggMS4zaDVjMC4wMjYgMC42NiAwLjMyIDEuMSAwLjcxIDEuNSAwLjg0IDAuNjEgMiAwLjYxIDIuOCAwIDAuNTItMC40IDAuNi0xIDAuNzEtMS41aDVsMC4yOC0xLjNjLTEuOS0wLjk3LTIuMi0zLjMtMi4zLTUuMy0wLjEzLTEuOC0wLjI2LTMuNy0xLjUtNS4yLTAuODUtMS0yLjItMS44LTMuNi0xLjh6bTAgMS40YzAuODggMCAxLjkgMC41NSAyLjUgMS4zIDAuODggMS4xIDEuMSAyLjcgMS4yIDQuNCAwLjEzIDEuNyAwLjIzIDMuNiAxLjMgNS4yaC0xMGMxLjEtMS42IDEuMi0zLjQgMS4zLTUuMiAwLjEzLTEuNyAwLjMtMy4zIDEuMi00LjQgMC41OS0wLjcyIDEuNi0xLjMgMi41LTEuM3ptLTAuNzQgMTJoMS41Yy0wLjAwMTUgMC4yOCAwLjAxNSAwLjc5LTAuNzQgMC43OS0wLjczIDAuMDAxNi0wLjcyLTAuNTMtMC43NC0wLjc5eiIgLz4KPC9zdmc+Cg==);
  --jp-icon-bug-dot: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiPgogICAgICAgIDxwYXRoIGZpbGwtcnVsZT0iZXZlbm9kZCIgY2xpcC1ydWxlPSJldmVub2RkIiBkPSJNMTcuMTkgOEgyMFYxMEgxNy45MUMxNy45NiAxMC4zMyAxOCAxMC42NiAxOCAxMVYxMkgyMFYxNEgxOC41SDE4VjE0LjAyNzVDMTUuNzUgMTQuMjc2MiAxNCAxNi4xODM3IDE0IDE4LjVDMTQgMTkuMjA4IDE0LjE2MzUgMTkuODc3OSAxNC40NTQ5IDIwLjQ3MzlDMTMuNzA2MyAyMC44MTE3IDEyLjg3NTcgMjEgMTIgMjFDOS43OCAyMSA3Ljg1IDE5Ljc5IDYuODEgMThINFYxNkg2LjA5QzYuMDQgMTUuNjcgNiAxNS4zNCA2IDE1VjE0SDRWMTJINlYxMUM2IDEwLjY2IDYuMDQgMTAuMzMgNi4wOSAxMEg0VjhINi44MUM3LjI2IDcuMjIgNy44OCA2LjU1IDguNjIgNi4wNEw3IDQuNDFMOC40MSAzTDEwLjU5IDUuMTdDMTEuMDQgNS4wNiAxMS41MSA1IDEyIDVDMTIuNDkgNSAxMi45NiA1LjA2IDEzLjQyIDUuMTdMMTUuNTkgM0wxNyA0LjQxTDE1LjM3IDYuMDRDMTYuMTIgNi41NSAxNi43NCA3LjIyIDE3LjE5IDhaTTEwIDE2SDE0VjE0SDEwVjE2Wk0xMCAxMkgxNFYxMEgxMFYxMloiIGZpbGw9IiM2MTYxNjEiLz4KICAgICAgICA8cGF0aCBkPSJNMjIgMTguNUMyMiAyMC40MzMgMjAuNDMzIDIyIDE4LjUgMjJDMTYuNTY3IDIyIDE1IDIwLjQzMyAxNSAxOC41QzE1IDE2LjU2NyAxNi41NjcgMTUgMTguNSAxNUMyMC40MzMgMTUgMjIgMTYuNTY3IDIyIDE4LjVaIiBmaWxsPSIjNjE2MTYxIi8+CiAgICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-bug: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik0yMCA4aC0yLjgxYy0uNDUtLjc4LTEuMDctMS40NS0xLjgyLTEuOTZMMTcgNC40MSAxNS41OSAzbC0yLjE3IDIuMTdDMTIuOTYgNS4wNiAxMi40OSA1IDEyIDVjLS40OSAwLS45Ni4wNi0xLjQxLjE3TDguNDEgMyA3IDQuNDFsMS42MiAxLjYzQzcuODggNi41NSA3LjI2IDcuMjIgNi44MSA4SDR2MmgyLjA5Yy0uMDUuMzMtLjA5LjY2LS4wOSAxdjFINHYyaDJ2MWMwIC4zNC4wNC42Ny4wOSAxSDR2MmgyLjgxYzEuMDQgMS43OSAyLjk3IDMgNS4xOSAzczQuMTUtMS4yMSA1LjE5LTNIMjB2LTJoLTIuMDljLjA1LS4zMy4wOS0uNjYuMDktMXYtMWgydi0yaC0ydi0xYzAtLjM0LS4wNC0uNjctLjA5LTFIMjBWOHptLTYgOGgtNHYtMmg0djJ6bTAtNGgtNHYtMmg0djJ6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-build: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTYiIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE0LjkgMTcuNDVDMTYuMjUgMTcuNDUgMTcuMzUgMTYuMzUgMTcuMzUgMTVDMTcuMzUgMTMuNjUgMTYuMjUgMTIuNTUgMTQuOSAxMi41NUMxMy41NCAxMi41NSAxMi40NSAxMy42NSAxMi40NSAxNUMxMi40NSAxNi4zNSAxMy41NCAxNy40NSAxNC45IDE3LjQ1Wk0yMC4xIDE1LjY4TDIxLjU4IDE2Ljg0QzIxLjcxIDE2Ljk1IDIxLjc1IDE3LjEzIDIxLjY2IDE3LjI5TDIwLjI2IDE5LjcxQzIwLjE3IDE5Ljg2IDIwIDE5LjkyIDE5LjgzIDE5Ljg2TDE4LjA5IDE5LjE2QzE3LjczIDE5LjQ0IDE3LjMzIDE5LjY3IDE2LjkxIDE5Ljg1TDE2LjY0IDIxLjdDMTYuNjIgMjEuODcgMTYuNDcgMjIgMTYuMyAyMkgxMy41QzEzLjMyIDIyIDEzLjE4IDIxLjg3IDEzLjE1IDIxLjdMMTIuODkgMTkuODVDMTIuNDYgMTkuNjcgMTIuMDcgMTkuNDQgMTEuNzEgMTkuMTZMOS45NjAwMiAxOS44NkM5LjgxMDAyIDE5LjkyIDkuNjIwMDIgMTkuODYgOS41NDAwMiAxOS43MUw4LjE0MDAyIDE3LjI5QzguMDUwMDIgMTcuMTMgOC4wOTAwMiAxNi45NSA4LjIyMDAyIDE2Ljg0TDkuNzAwMDIgMTUuNjhMOS42NTAwMSAxNUw5LjcwMDAyIDE0LjMxTDguMjIwMDIgMTMuMTZDOC4wOTAwMiAxMy4wNSA4LjA1MDAyIDEyLjg2IDguMTQwMDIgMTIuNzFMOS41NDAwMiAxMC4yOUM5LjYyMDAyIDEwLjEzIDkuODEwMDIgMTAuMDcgOS45NjAwMiAxMC4xM0wxMS43MSAxMC44NEMxMi4wNyAxMC41NiAxMi40NiAxMC4zMiAxMi44OSAxMC4xNUwxMy4xNSA4LjI4OTk4QzEzLjE4IDguMTI5OTggMTMuMzIgNy45OTk5OCAxMy41IDcuOTk5OThIMTYuM0MxNi40NyA3Ljk5OTk4IDE2LjYyIDguMTI5OTggMTYuNjQgOC4yODk5OEwxNi45MSAxMC4xNUMxNy4zMyAxMC4zMiAxNy43MyAxMC41NiAxOC4wOSAxMC44NEwxOS44MyAxMC4xM0MyMCAxMC4wNyAyMC4xNyAxMC4xMyAyMC4yNiAxMC4yOUwyMS42NiAxMi43MUMyMS43NSAxMi44NiAyMS43MSAxMy4wNSAyMS41OCAxMy4xNkwyMC4xIDE0LjMxTDIwLjE1IDE1TDIwLjEgMTUuNjhaIi8+CiAgICA8cGF0aCBkPSJNNy4zMjk2NiA3LjQ0NDU0QzguMDgzMSA3LjAwOTU0IDguMzM5MzIgNi4wNTMzMiA3LjkwNDMyIDUuMjk5ODhDNy40NjkzMiA0LjU0NjQzIDYuNTA4MSA0LjI4MTU2IDUuNzU0NjYgNC43MTY1NkM1LjM5MTc2IDQuOTI2MDggNS4xMjY5NSA1LjI3MTE4IDUuMDE4NDkgNS42NzU5NEM0LjkxMDA0IDYuMDgwNzEgNC45NjY4MiA2LjUxMTk4IDUuMTc2MzQgNi44NzQ4OEM1LjYxMTM0IDcuNjI4MzIgNi41NzYyMiA3Ljg3OTU0IDcuMzI5NjYgNy40NDQ1NFpNOS42NTcxOCA0Ljc5NTkzTDEwLjg2NzIgNC45NTE3OUMxMC45NjI4IDQuOTc3NDEgMTEuMDQwMiA1LjA3MTMzIDExLjAzODIgNS4xODc5M0wxMS4wMzg4IDYuOTg4OTNDMTEuMDQ1NSA3LjEwMDU0IDEwLjk2MTYgNy4xOTUxOCAxMC44NTUgNy4yMTA1NEw5LjY2MDAxIDcuMzgwODNMOS4yMzkxNSA4LjEzMTg4TDkuNjY5NjEgOS4yNTc0NUM5LjcwNzI5IDkuMzYyNzEgOS42NjkzNCA5LjQ3Njk5IDkuNTc0MDggOS41MzE5OUw4LjAxNTIzIDEwLjQzMkM3LjkxMTMxIDEwLjQ5MiA3Ljc5MzM3IDEwLjQ2NzcgNy43MjEwNSAxMC4zODI0TDYuOTg3NDggOS40MzE4OEw2LjEwOTMxIDkuNDMwODNMNS4zNDcwNCAxMC4zOTA1QzUuMjg5MDkgMTAuNDcwMiA1LjE3MzgzIDEwLjQ5MDUgNS4wNzE4NyAxMC40MzM5TDMuNTEyNDUgOS41MzI5M0MzLjQxMDQ5IDkuNDc2MzMgMy4zNzY0NyA5LjM1NzQxIDMuNDEwNzUgOS4yNTY3OUwzLjg2MzQ3IDguMTQwOTNMMy42MTc0OSA3Ljc3NDg4TDMuNDIzNDcgNy4zNzg4M0wyLjIzMDc1IDcuMjEyOTdDMi4xMjY0NyA3LjE5MjM1IDIuMDQwNDkgNy4xMDM0MiAyLjA0MjQ1IDYuOTg2ODJMMi4wNDE4NyA1LjE4NTgyQzIuMDQzODMgNS4wNjkyMiAyLjExOTA5IDQuOTc5NTggMi4yMTcwNCA0Ljk2OTIyTDMuNDIwNjUgNC43OTM5M0wzLjg2NzQ5IDQuMDI3ODhMMy40MTEwNSAyLjkxNzMxQzMuMzczMzcgMi44MTIwNCAzLjQxMTMxIDIuNjk3NzYgMy41MTUyMyAyLjYzNzc2TDUuMDc0MDggMS43Mzc3NkM1LjE2OTM0IDEuNjgyNzYgNS4yODcyOSAxLjcwNzA0IDUuMzU5NjEgMS43OTIzMUw2LjExOTE1IDIuNzI3ODhMNi45ODAwMSAyLjczODkzTDcuNzI0OTYgMS43ODkyMkM3Ljc5MTU2IDEuNzA0NTggNy45MTU0OCAxLjY3OTIyIDguMDA4NzkgMS43NDA4Mkw5LjU2ODIxIDIuNjQxODJDOS42NzAxNyAyLjY5ODQyIDkuNzEyODUgMi44MTIzNCA5LjY4NzIzIDIuOTA3OTdMOS4yMTcxOCA0LjAzMzgzTDkuNDYzMTYgNC4zOTk4OEw5LjY1NzE4IDQuNzk1OTNaIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-caret-down-empty-thin: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwb2x5Z29uIGNsYXNzPSJzdDEiIHBvaW50cz0iOS45LDEzLjYgMy42LDcuNCA0LjQsNi42IDkuOSwxMi4yIDE1LjQsNi43IDE2LjEsNy40ICIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-caret-down-empty: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik01LjIsNS45TDksOS43bDMuOC0zLjhsMS4yLDEuMmwtNC45LDVsLTQuOS01TDUuMiw1Ljl6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-caret-down: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik01LjIsNy41TDksMTEuMmwzLjgtMy44SDUuMnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-caret-left: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwYXRoIGQ9Ik0xMC44LDEyLjhMNy4xLDlsMy44LTMuOGwwLDcuNkgxMC44eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-caret-right: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik03LjIsNS4yTDEwLjksOWwtMy44LDMuOFY1LjJINy4yeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-caret-up-empty-thin: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwb2x5Z29uIGNsYXNzPSJzdDEiIHBvaW50cz0iMTUuNCwxMy4zIDkuOSw3LjcgNC40LDEzLjIgMy42LDEyLjUgOS45LDYuMyAxNi4xLDEyLjYgIi8+Cgk8L2c+Cjwvc3ZnPgo=);
  --jp-icon-caret-up: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwYXRoIGQ9Ik01LjIsMTAuNUw5LDYuOGwzLjgsMy44SDUuMnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-case-sensitive: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0MTQxNDEiPgogICAgPHJlY3QgeD0iMiIgeT0iMiIgd2lkdGg9IjE2IiBoZWlnaHQ9IjE2Ii8+CiAgPC9nPgogIDxnIGNsYXNzPSJqcC1pY29uLWFjY2VudDIiIGZpbGw9IiNGRkYiPgogICAgPHBhdGggZD0iTTcuNiw4aDAuOWwzLjUsOGgtMS4xTDEwLDE0SDZsLTAuOSwySDRMNy42LDh6IE04LDkuMUw2LjQsMTNoMy4yTDgsOS4xeiIvPgogICAgPHBhdGggZD0iTTE2LjYsOS44Yy0wLjIsMC4xLTAuNCwwLjEtMC43LDAuMWMtMC4yLDAtMC40LTAuMS0wLjYtMC4yYy0wLjEtMC4xLTAuMi0wLjQtMC4yLTAuNyBjLTAuMywwLjMtMC42LDAuNS0wLjksMC43Yy0wLjMsMC4xLTAuNywwLjItMS4xLDAuMmMtMC4zLDAtMC41LDAtMC43LTAuMWMtMC4yLTAuMS0wLjQtMC4yLTAuNi0wLjNjLTAuMi0wLjEtMC4zLTAuMy0wLjQtMC41IGMtMC4xLTAuMi0wLjEtMC40LTAuMS0wLjdjMC0wLjMsMC4xLTAuNiwwLjItMC44YzAuMS0wLjIsMC4zLTAuNCwwLjQtMC41QzEyLDcsMTIuMiw2LjksMTIuNSw2LjhjMC4yLTAuMSwwLjUtMC4xLDAuNy0wLjIgYzAuMy0wLjEsMC41LTAuMSwwLjctMC4xYzAuMiwwLDAuNC0wLjEsMC42LTAuMWMwLjIsMCwwLjMtMC4xLDAuNC0wLjJjMC4xLTAuMSwwLjItMC4yLDAuMi0wLjRjMC0xLTEuMS0xLTEuMy0xIGMtMC40LDAtMS40LDAtMS40LDEuMmgtMC45YzAtMC40LDAuMS0wLjcsMC4yLTFjMC4xLTAuMiwwLjMtMC40LDAuNS0wLjZjMC4yLTAuMiwwLjUtMC4zLDAuOC0wLjNDMTMuMyw0LDEzLjYsNCwxMy45LDQgYzAuMywwLDAuNSwwLDAuOCwwLjFjMC4zLDAsMC41LDAuMSwwLjcsMC4yYzAuMiwwLjEsMC40LDAuMywwLjUsMC41QzE2LDUsMTYsNS4yLDE2LDUuNnYyLjljMCwwLjIsMCwwLjQsMCwwLjUgYzAsMC4xLDAuMSwwLjIsMC4zLDAuMmMwLjEsMCwwLjIsMCwwLjMsMFY5Ljh6IE0xNS4yLDYuOWMtMS4yLDAuNi0zLjEsMC4yLTMuMSwxLjRjMCwxLjQsMy4xLDEsMy4xLTAuNVY2Ljl6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-check: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik05IDE2LjE3TDQuODMgMTJsLTEuNDIgMS40MUw5IDE5IDIxIDdsLTEuNDEtMS40MXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-circle-empty: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyIDJDNi40NyAyIDIgNi40NyAyIDEyczQuNDcgMTAgMTAgMTAgMTAtNC40NyAxMC0xMFMxNy41MyAyIDEyIDJ6bTAgMThjLTQuNDEgMC04LTMuNTktOC04czMuNTktOCA4LTggOCAzLjU5IDggOC0zLjU5IDgtOCA4eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-circle: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPGNpcmNsZSBjeD0iOSIgY3k9IjkiIHI9IjgiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-clear: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8bWFzayBpZD0iZG9udXRIb2xlIj4KICAgIDxyZWN0IHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgZmlsbD0id2hpdGUiIC8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSI4IiBmaWxsPSJibGFjayIvPgogIDwvbWFzaz4KCiAgPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxyZWN0IGhlaWdodD0iMTgiIHdpZHRoPSIyIiB4PSIxMSIgeT0iMyIgdHJhbnNmb3JtPSJyb3RhdGUoMzE1LCAxMiwgMTIpIi8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIxMCIgbWFzaz0idXJsKCNkb251dEhvbGUpIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-close: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbi1ub25lIGpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIGpwLWljb24zLWhvdmVyIiBmaWxsPSJub25lIj4KICAgIDxjaXJjbGUgY3g9IjEyIiBjeT0iMTIiIHI9IjExIi8+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIGpwLWljb24tYWNjZW50Mi1ob3ZlciIgZmlsbD0iIzYxNjE2MSI+CiAgICA8cGF0aCBkPSJNMTkgNi40MUwxNy41OSA1IDEyIDEwLjU5IDYuNDEgNSA1IDYuNDEgMTAuNTkgMTIgNSAxNy41OSA2LjQxIDE5IDEyIDEzLjQxIDE3LjU5IDE5IDE5IDE3LjU5IDEzLjQxIDEyeiIvPgogIDwvZz4KCiAgPGcgY2xhc3M9ImpwLWljb24tbm9uZSBqcC1pY29uLWJ1c3kiIGZpbGw9Im5vbmUiPgogICAgPGNpcmNsZSBjeD0iMTIiIGN5PSIxMiIgcj0iNyIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-code-check: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBzaGFwZS1yZW5kZXJpbmc9Imdlb21ldHJpY1ByZWNpc2lvbiI+CiAgICA8cGF0aCBkPSJNNi41OSwzLjQxTDIsOEw2LjU5LDEyLjZMOCwxMS4xOEw0LjgyLDhMOCw0LjgyTDYuNTksMy40MU0xMi40MSwzLjQxTDExLDQuODJMMTQuMTgsOEwxMSwxMS4xOEwxMi40MSwxMi42TDE3LDhMMTIuNDEsMy40MU0yMS41OSwxMS41OUwxMy41LDE5LjY4TDkuODMsMTZMOC40MiwxNy40MUwxMy41LDIyLjVMMjMsMTNMMjEuNTksMTEuNTlaIiAvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-code: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjIiIGhlaWdodD0iMjIiIHZpZXdCb3g9IjAgMCAyOCAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTExLjQgMTguNkw2LjggMTRMMTEuNCA5LjRMMTAgOEw0IDE0TDEwIDIwTDExLjQgMTguNlpNMTYuNiAxOC42TDIxLjIgMTRMMTYuNiA5LjRMMTggOEwyNCAxNEwxOCAyMEwxNi42IDE4LjZWMTguNloiLz4KCTwvZz4KPC9zdmc+Cg==);
  --jp-icon-collapse-all: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGgKICAgICAgICAgICAgZD0iTTggMmMxIDAgMTEgMCAxMiAwczIgMSAyIDJjMCAxIDAgMTEgMCAxMnMwIDItMiAyQzIwIDE0IDIwIDQgMjAgNFMxMCA0IDYgNGMwLTIgMS0yIDItMnoiIC8+CiAgICAgICAgPHBhdGgKICAgICAgICAgICAgZD0iTTE4IDhjMC0xLTEtMi0yLTJTNSA2IDQgNnMtMiAxLTIgMmMwIDEgMCAxMSAwIDEyczEgMiAyIDJjMSAwIDExIDAgMTIgMHMyLTEgMi0yYzAtMSAwLTExIDAtMTJ6bS0yIDB2MTJINFY4eiIgLz4KICAgICAgICA8cGF0aCBkPSJNNiAxM3YyaDh2LTJ6IiAvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-console: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwMCAyMDAiPgogIDxnIGNsYXNzPSJqcC1jb25zb2xlLWljb24tYmFja2dyb3VuZC1jb2xvciBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiMwMjg4RDEiPgogICAgPHBhdGggZD0iTTIwIDE5LjhoMTYwdjE1OS45SDIweiIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtY29uc29sZS1pY29uLWNvbG9yIGpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIiBmaWxsPSIjZmZmIj4KICAgIDxwYXRoIGQ9Ik0xMDUgMTI3LjNoNDB2MTIuOGgtNDB6TTUxLjEgNzdMNzQgOTkuOWwtMjMuMyAyMy4zIDEwLjUgMTAuNSAyMy4zLTIzLjNMOTUgOTkuOSA4NC41IDg5LjQgNjEuNiA2Ni41eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-copy: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTExLjksMUgzLjJDMi40LDEsMS43LDEuNywxLjcsMi41djEwLjJoMS41VjIuNWg4LjdWMXogTTE0LjEsMy45aC04Yy0wLjgsMC0xLjUsMC43LTEuNSwxLjV2MTAuMmMwLDAuOCwwLjcsMS41LDEuNSwxLjVoOCBjMC44LDAsMS41LTAuNywxLjUtMS41VjUuNEMxNS41LDQuNiwxNC45LDMuOSwxNC4xLDMuOXogTTE0LjEsMTUuNWgtOFY1LjRoOFYxNS41eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-copyright: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGVuYWJsZS1iYWNrZ3JvdW5kPSJuZXcgMCAwIDI0IDI0IiBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCI+CiAgPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik0xMS44OCw5LjE0YzEuMjgsMC4wNiwxLjYxLDEuMTUsMS42MywxLjY2aDEuNzljLTAuMDgtMS45OC0xLjQ5LTMuMTktMy40NS0zLjE5QzkuNjQsNy42MSw4LDksOCwxMi4xNCBjMCwxLjk0LDAuOTMsNC4yNCwzLjg0LDQuMjRjMi4yMiwwLDMuNDEtMS42NSwzLjQ0LTIuOTVoLTEuNzljLTAuMDMsMC41OS0wLjQ1LDEuMzgtMS42MywxLjQ0QzEwLjU1LDE0LjgzLDEwLDEzLjgxLDEwLDEyLjE0IEMxMCw5LjI1LDExLjI4LDkuMTYsMTEuODgsOS4xNHogTTEyLDJDNi40OCwyLDIsNi40OCwyLDEyczQuNDgsMTAsMTAsMTBzMTAtNC40OCwxMC0xMFMxNy41MiwyLDEyLDJ6IE0xMiwyMGMtNC40MSwwLTgtMy41OS04LTggczMuNTktOCw4LThzOCwzLjU5LDgsOFMxNi40MSwyMCwxMiwyMHoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-cut: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTkuNjQgNy42NGMuMjMtLjUuMzYtMS4wNS4zNi0xLjY0IDAtMi4yMS0xLjc5LTQtNC00UzIgMy43OSAyIDZzMS43OSA0IDQgNGMuNTkgMCAxLjE0LS4xMyAxLjY0LS4zNkwxMCAxMmwtMi4zNiAyLjM2QzcuMTQgMTQuMTMgNi41OSAxNCA2IDE0Yy0yLjIxIDAtNCAxLjc5LTQgNHMxLjc5IDQgNCA0IDQtMS43OSA0LTRjMC0uNTktLjEzLTEuMTQtLjM2LTEuNjRMMTIgMTRsNyA3aDN2LTFMOS42NCA3LjY0ek02IDhjLTEuMSAwLTItLjg5LTItMnMuOS0yIDItMiAyIC44OSAyIDItLjkgMi0yIDJ6bTAgMTJjLTEuMSAwLTItLjg5LTItMnMuOS0yIDItMiAyIC44OSAyIDItLjkgMi0yIDJ6bTYtNy41Yy0uMjggMC0uNS0uMjItLjUtLjVzLjIyLS41LjUtLjUuNS4yMi41LjUtLjIyLjUtLjUuNXpNMTkgM2wtNiA2IDIgMiA3LTdWM3oiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-delete: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjE2cHgiIGhlaWdodD0iMTZweCI+CiAgICA8cGF0aCBkPSJNMCAwaDI0djI0SDB6IiBmaWxsPSJub25lIiAvPgogICAgPHBhdGggY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjI2MjYyIiBkPSJNNiAxOWMwIDEuMS45IDIgMiAyaDhjMS4xIDAgMi0uOSAyLTJWN0g2djEyek0xOSA0aC0zLjVsLTEtMWgtNWwtMSAxSDV2MmgxNFY0eiIgLz4KPC9zdmc+Cg==);
  --jp-icon-download: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE5IDloLTRWM0g5djZINWw3IDcgNy03ek01IDE4djJoMTR2LTJINXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-duplicate: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGNsaXAtcnVsZT0iZXZlbm9kZCIgZD0iTTIuNzk5OTggMC44NzVIOC44OTU4MkM5LjIwMDYxIDAuODc1IDkuNDQ5OTggMS4xMzkxNCA5LjQ0OTk4IDEuNDYxOThDOS40NDk5OCAxLjc4NDgyIDkuMjAwNjEgMi4wNDg5NiA4Ljg5NTgyIDIuMDQ4OTZIMy4zNTQxNUMzLjA0OTM2IDIuMDQ4OTYgMi43OTk5OCAyLjMxMzEgMi43OTk5OCAyLjYzNTk0VjkuNjc5NjlDMi43OTk5OCAxMC4wMDI1IDIuNTUwNjEgMTAuMjY2NyAyLjI0NTgyIDEwLjI2NjdDMS45NDEwMyAxMC4yNjY3IDEuNjkxNjUgMTAuMDAyNSAxLjY5MTY1IDkuNjc5NjlWMi4wNDg5NkMxLjY5MTY1IDEuNDAzMjggMi4xOTA0IDAuODc1IDIuNzk5OTggMC44NzVaTTUuMzY2NjUgMTEuOVY0LjU1SDExLjA4MzNWMTEuOUg1LjM2NjY1Wk00LjE0MTY1IDQuMTQxNjdDNC4xNDE2NSAzLjY5MDYzIDQuNTA3MjggMy4zMjUgNC45NTgzMiAzLjMyNUgxMS40OTE3QzExLjk0MjcgMy4zMjUgMTIuMzA4MyAzLjY5MDYzIDEyLjMwODMgNC4xNDE2N1YxMi4zMDgzQzEyLjMwODMgMTIuNzU5NCAxMS45NDI3IDEzLjEyNSAxMS40OTE3IDEzLjEyNUg0Ljk1ODMyQzQuNTA3MjggMTMuMTI1IDQuMTQxNjUgMTIuNzU5NCA0LjE0MTY1IDEyLjMwODNWNC4xNDE2N1oiIGZpbGw9IiM2MTYxNjEiLz4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBkPSJNOS40MzU3NCA4LjI2NTA3SDguMzY0MzFWOS4zMzY1QzguMzY0MzEgOS40NTQzNSA4LjI2Nzg4IDkuNTUwNzggOC4xNTAwMiA5LjU1MDc4QzguMDMyMTcgOS41NTA3OCA3LjkzNTc0IDkuNDU0MzUgNy45MzU3NCA5LjMzNjVWOC4yNjUwN0g2Ljg2NDMxQzYuNzQ2NDUgOC4yNjUwNyA2LjY1MDAyIDguMTY4NjQgNi42NTAwMiA4LjA1MDc4QzYuNjUwMDIgNy45MzI5MiA2Ljc0NjQ1IDcuODM2NSA2Ljg2NDMxIDcuODM2NUg3LjkzNTc0VjYuNzY1MDdDNy45MzU3NCA2LjY0NzIxIDguMDMyMTcgNi41NTA3OCA4LjE1MDAyIDYuNTUwNzhDOC4yNjc4OCA2LjU1MDc4IDguMzY0MzEgNi42NDcyMSA4LjM2NDMxIDYuNzY1MDdWNy44MzY1SDkuNDM1NzRDOS41NTM2IDcuODM2NSA5LjY1MDAyIDcuOTMyOTIgOS42NTAwMiA4LjA1MDc4QzkuNjUwMDIgOC4xNjg2NCA5LjU1MzYgOC4yNjUwNyA5LjQzNTc0IDguMjY1MDdaIiBmaWxsPSIjNjE2MTYxIiBzdHJva2U9IiM2MTYxNjEiIHN0cm9rZS13aWR0aD0iMC41Ii8+Cjwvc3ZnPgo=);
  --jp-icon-edit: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTMgMTcuMjVWMjFoMy43NUwxNy44MSA5Ljk0bC0zLjc1LTMuNzVMMyAxNy4yNXpNMjAuNzEgNy4wNGMuMzktLjM5LjM5LTEuMDIgMC0xLjQxbC0yLjM0LTIuMzRjLS4zOS0uMzktMS4wMi0uMzktMS40MSAwbC0xLjgzIDEuODMgMy43NSAzLjc1IDEuODMtMS44M3oiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-ellipses: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPGNpcmNsZSBjeD0iNSIgY3k9IjEyIiByPSIyIi8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIyIi8+CiAgICA8Y2lyY2xlIGN4PSIxOSIgY3k9IjEyIiByPSIyIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-error: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj48Y2lyY2xlIGN4PSIxMiIgY3k9IjE5IiByPSIyIi8+PHBhdGggZD0iTTEwIDNoNHYxMmgtNHoiLz48L2c+CjxwYXRoIGZpbGw9Im5vbmUiIGQ9Ik0wIDBoMjR2MjRIMHoiLz4KPC9zdmc+Cg==);
  --jp-icon-expand-all: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGgKICAgICAgICAgICAgZD0iTTggMmMxIDAgMTEgMCAxMiAwczIgMSAyIDJjMCAxIDAgMTEgMCAxMnMwIDItMiAyQzIwIDE0IDIwIDQgMjAgNFMxMCA0IDYgNGMwLTIgMS0yIDItMnoiIC8+CiAgICAgICAgPHBhdGgKICAgICAgICAgICAgZD0iTTE4IDhjMC0xLTEtMi0yLTJTNSA2IDQgNnMtMiAxLTIgMmMwIDEgMCAxMSAwIDEyczEgMiAyIDJjMSAwIDExIDAgMTIgMHMyLTEgMi0yYzAtMSAwLTExIDAtMTJ6bS0yIDB2MTJINFY4eiIgLz4KICAgICAgICA8cGF0aCBkPSJNMTEgMTBIOXYzSDZ2MmgzdjNoMnYtM2gzdi0yaC0zeiIgLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-extension: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIwLjUgMTFIMTlWN2MwLTEuMS0uOS0yLTItMmgtNFYzLjVDMTMgMi4xMiAxMS44OCAxIDEwLjUgMVM4IDIuMTIgOCAzLjVWNUg0Yy0xLjEgMC0xLjk5LjktMS45OSAydjMuOEgzLjVjMS40OSAwIDIuNyAxLjIxIDIuNyAyLjdzLTEuMjEgMi43LTIuNyAyLjdIMlYyMGMwIDEuMS45IDIgMiAyaDMuOHYtMS41YzAtMS40OSAxLjIxLTIuNyAyLjctMi43IDEuNDkgMCAyLjcgMS4yMSAyLjcgMi43VjIySDE3YzEuMSAwIDItLjkgMi0ydi00aDEuNWMxLjM4IDAgMi41LTEuMTIgMi41LTIuNVMyMS44OCAxMSAyMC41IDExeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-fast-forward: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTQgMThsOC41LTZMNCA2djEyem05LTEydjEybDguNS02TDEzIDZ6Ii8+CiAgICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-file-upload: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTkgMTZoNnYtNmg0bC03LTctNyA3aDR6bS00IDJoMTR2Mkg1eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-file: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkuMyA4LjJsLTUuNS01LjVjLS4zLS4zLS43LS41LTEuMi0uNUgzLjljLS44LjEtMS42LjktMS42IDEuOHYxNC4xYzAgLjkuNyAxLjYgMS42IDEuNmgxNC4yYy45IDAgMS42LS43IDEuNi0xLjZWOS40Yy4xLS41LS4xLS45LS40LTEuMnptLTUuOC0zLjNsMy40IDMuNmgtMy40VjQuOXptMy45IDEyLjdINC43Yy0uMSAwLS4yIDAtLjItLjJWNC43YzAtLjIuMS0uMy4yLS4zaDcuMnY0LjRzMCAuOC4zIDEuMWMuMy4zIDEuMS4zIDEuMS4zaDQuM3Y3LjJzLS4xLjItLjIuMnoiLz4KPC9zdmc+Cg==);
  --jp-icon-filter-dot: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiNGRkYiPgogICAgPHBhdGggZD0iTTE0LDEyVjE5Ljg4QzE0LjA0LDIwLjE4IDEzLjk0LDIwLjUgMTMuNzEsMjAuNzFDMTMuMzIsMjEuMSAxMi42OSwyMS4xIDEyLjMsMjAuNzFMMTAuMjksMTguN0MxMC4wNiwxOC40NyA5Ljk2LDE4LjE2IDEwLDE3Ljg3VjEySDkuOTdMNC4yMSw0LjYyQzMuODcsNC4xOSAzLjk1LDMuNTYgNC4zOCwzLjIyQzQuNTcsMy4wOCA0Ljc4LDMgNSwzVjNIMTlWM0MxOS4yMiwzIDE5LjQzLDMuMDggMTkuNjIsMy4yMkMyMC4wNSwzLjU2IDIwLjEzLDQuMTkgMTkuNzksNC42MkwxNC4wMywxMkgxNFoiIC8+CiAgPC9nPgogIDxnIGNsYXNzPSJqcC1pY29uLWRvdCIgZmlsbD0iI0ZGRiI+CiAgICA8Y2lyY2xlIGN4PSIxOCIgY3k9IjE3IiByPSIzIj48L2NpcmNsZT4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-filter-list: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEwIDE4aDR2LTJoLTR2MnpNMyA2djJoMThWNkgzem0zIDdoMTJ2LTJINnYyeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-filter: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiNGRkYiPgogICAgPHBhdGggZD0iTTE0LDEyVjE5Ljg4QzE0LjA0LDIwLjE4IDEzLjk0LDIwLjUgMTMuNzEsMjAuNzFDMTMuMzIsMjEuMSAxMi42OSwyMS4xIDEyLjMsMjAuNzFMMTAuMjksMTguN0MxMC4wNiwxOC40NyA5Ljk2LDE4LjE2IDEwLDE3Ljg3VjEySDkuOTdMNC4yMSw0LjYyQzMuODcsNC4xOSAzLjk1LDMuNTYgNC4zOCwzLjIyQzQuNTcsMy4wOCA0Ljc4LDMgNSwzVjNIMTlWM0MxOS4yMiwzIDE5LjQzLDMuMDggMTkuNjIsMy4yMkMyMC4wNSwzLjU2IDIwLjEzLDQuMTkgMTkuNzksNC42MkwxNC4wMywxMkgxNFoiIC8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-folder-favorite: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMjRweCIgdmlld0JveD0iMCAwIDI0IDI0IiB3aWR0aD0iMjRweCIgZmlsbD0iIzAwMDAwMCI+CiAgPHBhdGggZD0iTTAgMGgyNHYyNEgwVjB6IiBmaWxsPSJub25lIi8+PHBhdGggY2xhc3M9ImpwLWljb24zIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzYxNjE2MSIgZD0iTTIwIDZoLThsLTItMkg0Yy0xLjEgMC0yIC45LTIgMnYxMmMwIDEuMS45IDIgMiAyaDE2YzEuMSAwIDItLjkgMi0yVjhjMC0xLjEtLjktMi0yLTJ6bS0yLjA2IDExTDE1IDE1LjI4IDEyLjA2IDE3bC43OC0zLjMzLTIuNTktMi4yNCAzLjQxLS4yOUwxNSA4bDEuMzQgMy4xNCAzLjQxLjI5LTIuNTkgMi4yNC43OCAzLjMzeiIvPgo8L3N2Zz4K);
  --jp-icon-folder: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTAgNEg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMThjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY4YzAtMS4xLS45LTItMi0yaC04bC0yLTJ6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-home: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMjRweCIgdmlld0JveD0iMCAwIDI0IDI0IiB3aWR0aD0iMjRweCIgZmlsbD0iIzAwMDAwMCI+CiAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPjxwYXRoIGNsYXNzPSJqcC1pY29uMyBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiIGQ9Ik0xMCAyMHYtNmg0djZoNXYtOGgzTDEyIDMgMiAxMmgzdjh6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-html5: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUxMiA1MTIiPgogIDxwYXRoIGNsYXNzPSJqcC1pY29uMCBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiMwMDAiIGQ9Ik0xMDguNCAwaDIzdjIyLjhoMjEuMlYwaDIzdjY5aC0yM1Y0NmgtMjF2MjNoLTIzLjJNMjA2IDIzaC0yMC4zVjBoNjMuN3YyM0gyMjl2NDZoLTIzbTUzLjUtNjloMjQuMWwxNC44IDI0LjNMMzEzLjIgMGgyNC4xdjY5aC0yM1YzNC44bC0xNi4xIDI0LjgtMTYuMS0yNC44VjY5aC0yMi42bTg5LjItNjloMjN2NDYuMmgzMi42VjY5aC01NS42Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI2U0NGQyNiIgZD0iTTEwNy42IDQ3MWwtMzMtMzcwLjRoMzYyLjhsLTMzIDM3MC4yTDI1NS43IDUxMiIvPgogIDxwYXRoIGNsYXNzPSJqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNmMTY1MjkiIGQ9Ik0yNTYgNDgwLjVWMTMxaDE0OC4zTDM3NiA0NDciLz4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNlYmViZWIiIGQ9Ik0xNDIgMTc2LjNoMTE0djQ1LjRoLTY0LjJsNC4yIDQ2LjVoNjB2NDUuM0gxNTQuNG0yIDIyLjhIMjAybDMuMiAzNi4zIDUwLjggMTMuNnY0Ny40bC05My4yLTI2Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIiBmaWxsPSIjZmZmIiBkPSJNMzY5LjYgMTc2LjNIMjU1Ljh2NDUuNGgxMDkuNm0tNC4xIDQ2LjVIMjU1Ljh2NDUuNGg1NmwtNS4zIDU5LTUwLjcgMTMuNnY0Ny4ybDkzLTI1LjgiLz4KPC9zdmc+Cg==);
  --jp-icon-image: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1icmFuZDQganAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNGRkYiIGQ9Ik0yLjIgMi4yaDE3LjV2MTcuNUgyLjJ6Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzNGNTFCNSIgZD0iTTIuMiAyLjJ2MTcuNWgxNy41bC4xLTE3LjVIMi4yem0xMi4xIDIuMmMxLjIgMCAyLjIgMSAyLjIgMi4ycy0xIDIuMi0yLjIgMi4yLTIuMi0xLTIuMi0yLjIgMS0yLjIgMi4yLTIuMnpNNC40IDE3LjZsMy4zLTguOCAzLjMgNi42IDIuMi0zLjIgNC40IDUuNEg0LjR6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-info: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUwLjk3OCA1MC45NzgiPgoJPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj4KCQk8cGF0aCBkPSJNNDMuNTIsNy40NThDMzguNzExLDIuNjQ4LDMyLjMwNywwLDI1LjQ4OSwwQzE4LjY3LDAsMTIuMjY2LDIuNjQ4LDcuNDU4LDcuNDU4CgkJCWMtOS45NDMsOS45NDEtOS45NDMsMjYuMTE5LDAsMzYuMDYyYzQuODA5LDQuODA5LDExLjIxMiw3LjQ1NiwxOC4wMzEsNy40NThjMCwwLDAuMDAxLDAsMC4wMDIsMAoJCQljNi44MTYsMCwxMy4yMjEtMi42NDgsMTguMDI5LTcuNDU4YzQuODA5LTQuODA5LDcuNDU3LTExLjIxMiw3LjQ1Ny0xOC4wM0M1MC45NzcsMTguNjcsNDguMzI4LDEyLjI2Niw0My41Miw3LjQ1OHoKCQkJIE00Mi4xMDYsNDIuMTA1Yy00LjQzMiw0LjQzMS0xMC4zMzIsNi44NzItMTYuNjE1LDYuODcyaC0wLjAwMmMtNi4yODUtMC4wMDEtMTIuMTg3LTIuNDQxLTE2LjYxNy02Ljg3MgoJCQljLTkuMTYyLTkuMTYzLTkuMTYyLTI0LjA3MSwwLTMzLjIzM0MxMy4zMDMsNC40NCwxOS4yMDQsMiwyNS40ODksMmM2LjI4NCwwLDEyLjE4NiwyLjQ0LDE2LjYxNyw2Ljg3MgoJCQljNC40MzEsNC40MzEsNi44NzEsMTAuMzMyLDYuODcxLDE2LjYxN0M0OC45NzcsMzEuNzcyLDQ2LjUzNiwzNy42NzUsNDIuMTA2LDQyLjEwNXoiLz4KCQk8cGF0aCBkPSJNMjMuNTc4LDMyLjIxOGMtMC4wMjMtMS43MzQsMC4xNDMtMy4wNTksMC40OTYtMy45NzJjMC4zNTMtMC45MTMsMS4xMS0xLjk5NywyLjI3Mi0zLjI1MwoJCQljMC40NjgtMC41MzYsMC45MjMtMS4wNjIsMS4zNjctMS41NzVjMC42MjYtMC43NTMsMS4xMDQtMS40NzgsMS40MzYtMi4xNzVjMC4zMzEtMC43MDcsMC40OTUtMS41NDEsMC40OTUtMi41CgkJCWMwLTEuMDk2LTAuMjYtMi4wODgtMC43NzktMi45NzljLTAuNTY1LTAuODc5LTEuNTAxLTEuMzM2LTIuODA2LTEuMzY5Yy0xLjgwMiwwLjA1Ny0yLjk4NSwwLjY2Ny0zLjU1LDEuODMyCgkJCWMtMC4zMDEsMC41MzUtMC41MDMsMS4xNDEtMC42MDcsMS44MTRjLTAuMTM5LDAuNzA3LTAuMjA3LDEuNDMyLTAuMjA3LDIuMTc0aC0yLjkzN2MtMC4wOTEtMi4yMDgsMC40MDctNC4xMTQsMS40OTMtNS43MTkKCQkJYzEuMDYyLTEuNjQsMi44NTUtMi40ODEsNS4zNzgtMi41MjdjMi4xNiwwLjAyMywzLjg3NCwwLjYwOCw1LjE0MSwxLjc1OGMxLjI3OCwxLjE2LDEuOTI5LDIuNzY0LDEuOTUsNC44MTEKCQkJYzAsMS4xNDItMC4xMzcsMi4xMTEtMC40MSwyLjkxMWMtMC4zMDksMC44NDUtMC43MzEsMS41OTMtMS4yNjgsMi4yNDNjLTAuNDkyLDAuNjUtMS4wNjgsMS4zMTgtMS43MywyLjAwMgoJCQljLTAuNjUsMC42OTctMS4zMTMsMS40NzktMS45ODcsMi4zNDZjLTAuMjM5LDAuMzc3LTAuNDI5LDAuNzc3LTAuNTY1LDEuMTk5Yy0wLjE2LDAuOTU5LTAuMjE3LDEuOTUxLTAuMTcxLDIuOTc5CgkJCUMyNi41ODksMzIuMjE4LDIzLjU3OCwzMi4yMTgsMjMuNTc4LDMyLjIxOHogTTIzLjU3OCwzOC4yMnYtMy40ODRoMy4wNzZ2My40ODRIMjMuNTc4eiIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-inspector: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaW5zcGVjdG9yLWljb24tY29sb3IganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMjAgNEg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMThjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY2YzAtMS4xLS45LTItMi0yem0tNSAxNEg0di00aDExdjR6bTAtNUg0VjloMTF2NHptNSA1aC00VjloNHY5eiIvPgo8L3N2Zz4K);
  --jp-icon-json: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtanNvbi1pY29uLWNvbG9yIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI0Y5QTgyNSI+CiAgICA8cGF0aCBkPSJNMjAuMiAxMS44Yy0xLjYgMC0xLjcuNS0xLjcgMSAwIC40LjEuOS4xIDEuMy4xLjUuMS45LjEgMS4zIDAgMS43LTEuNCAyLjMtMy41IDIuM2gtLjl2LTEuOWguNWMxLjEgMCAxLjQgMCAxLjQtLjggMC0uMyAwLS42LS4xLTEgMC0uNC0uMS0uOC0uMS0xLjIgMC0xLjMgMC0xLjggMS4zLTItMS4zLS4yLTEuMy0uNy0xLjMtMiAwLS40LjEtLjguMS0xLjIuMS0uNC4xLS43LjEtMSAwLS44LS40LS43LTEuNC0uOGgtLjVWNC4xaC45YzIuMiAwIDMuNS43IDMuNSAyLjMgMCAuNC0uMS45LS4xIDEuMy0uMS41LS4xLjktLjEgMS4zIDAgLjUuMiAxIDEuNyAxdjEuOHpNMS44IDEwLjFjMS42IDAgMS43LS41IDEuNy0xIDAtLjQtLjEtLjktLjEtMS4zLS4xLS41LS4xLS45LS4xLTEuMyAwLTEuNiAxLjQtMi4zIDMuNS0yLjNoLjl2MS45aC0uNWMtMSAwLTEuNCAwLTEuNC44IDAgLjMgMCAuNi4xIDEgMCAuMi4xLjYuMSAxIDAgMS4zIDAgMS44LTEuMyAyQzYgMTEuMiA2IDExLjcgNiAxM2MwIC40LS4xLjgtLjEgMS4yLS4xLjMtLjEuNy0uMSAxIDAgLjguMy44IDEuNC44aC41djEuOWgtLjljLTIuMSAwLTMuNS0uNi0zLjUtMi4zIDAtLjQuMS0uOS4xLTEuMy4xLS41LjEtLjkuMS0xLjMgMC0uNS0uMi0xLTEuNy0xdi0xLjl6Ii8+CiAgICA8Y2lyY2xlIGN4PSIxMSIgY3k9IjEzLjgiIHI9IjIuMSIvPgogICAgPGNpcmNsZSBjeD0iMTEiIGN5PSI4LjIiIHI9IjIuMSIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-julia: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDMyNSAzMDAiPgogIDxnIGNsYXNzPSJqcC1icmFuZDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjY2IzYzMzIj4KICAgIDxwYXRoIGQ9Ik0gMTUwLjg5ODQzOCAyMjUgQyAxNTAuODk4NDM4IDI2Ni40MjE4NzUgMTE3LjMyMDMxMiAzMDAgNzUuODk4NDM4IDMwMCBDIDM0LjQ3NjU2MiAzMDAgMC44OTg0MzggMjY2LjQyMTg3NSAwLjg5ODQzOCAyMjUgQyAwLjg5ODQzOCAxODMuNTc4MTI1IDM0LjQ3NjU2MiAxNTAgNzUuODk4NDM4IDE1MCBDIDExNy4zMjAzMTIgMTUwIDE1MC44OTg0MzggMTgzLjU3ODEyNSAxNTAuODk4NDM4IDIyNSIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzM4OTgyNiI+CiAgICA8cGF0aCBkPSJNIDIzNy41IDc1IEMgMjM3LjUgMTE2LjQyMTg3NSAyMDMuOTIxODc1IDE1MCAxNjIuNSAxNTAgQyAxMjEuMDc4MTI1IDE1MCA4Ny41IDExNi40MjE4NzUgODcuNSA3NSBDIDg3LjUgMzMuNTc4MTI1IDEyMS4wNzgxMjUgMCAxNjIuNSAwIEMgMjAzLjkyMTg3NSAwIDIzNy41IDMzLjU3ODEyNSAyMzcuNSA3NSIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzk1NThiMiI+CiAgICA8cGF0aCBkPSJNIDMyNC4xMDE1NjIgMjI1IEMgMzI0LjEwMTU2MiAyNjYuNDIxODc1IDI5MC41MjM0MzggMzAwIDI0OS4xMDE1NjIgMzAwIEMgMjA3LjY3OTY4OCAzMDAgMTc0LjEwMTU2MiAyNjYuNDIxODc1IDE3NC4xMDE1NjIgMjI1IEMgMTc0LjEwMTU2MiAxODMuNTc4MTI1IDIwNy42Nzk2ODggMTUwIDI0OS4xMDE1NjIgMTUwIEMgMjkwLjUyMzQzOCAxNTAgMzI0LjEwMTU2MiAxODMuNTc4MTI1IDMyNC4xMDE1NjIgMjI1Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-jupyter-favicon: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTUyIiBoZWlnaHQ9IjE2NSIgdmlld0JveD0iMCAwIDE1MiAxNjUiIHZlcnNpb249IjEuMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgPGcgY2xhc3M9ImpwLWp1cHl0ZXItaWNvbi1jb2xvciIgZmlsbD0iI0YzNzcyNiI+CiAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgwLjA3ODk0NywgMTEwLjU4MjkyNykiIGQ9Ik03NS45NDIyODQyLDI5LjU4MDQ1NjEgQzQzLjMwMjM5NDcsMjkuNTgwNDU2MSAxNC43OTY3ODMyLDE3LjY1MzQ2MzQgMCwwIEM1LjUxMDgzMjExLDE1Ljg0MDY4MjkgMTUuNzgxNTM4OSwyOS41NjY3NzMyIDI5LjM5MDQ5NDcsMzkuMjc4NDE3MSBDNDIuOTk5Nyw0OC45ODk4NTM3IDU5LjI3MzcsNTQuMjA2NzgwNSA3NS45NjA1Nzg5LDU0LjIwNjc4MDUgQzkyLjY0NzQ1NzksNTQuMjA2NzgwNSAxMDguOTIxNDU4LDQ4Ljk4OTg1MzcgMTIyLjUzMDY2MywzOS4yNzg0MTcxIEMxMzYuMTM5NDUzLDI5LjU2Njc3MzIgMTQ2LjQxMDI4NCwxNS44NDA2ODI5IDE1MS45MjExNTgsMCBDMTM3LjA4Nzg2OCwxNy42NTM0NjM0IDEwOC41ODI1ODksMjkuNTgwNDU2MSA3NS45NDIyODQyLDI5LjU4MDQ1NjEgTDc1Ljk0MjI4NDIsMjkuNTgwNDU2MSBaIiAvPgogICAgPHBhdGggdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC4wMzczNjgsIDAuNzA0ODc4KSIgZD0iTTc1Ljk3ODQ1NzksMjQuNjI2NDA3MyBDMTA4LjYxODc2MywyNC42MjY0MDczIDEzNy4xMjQ0NTgsMzYuNTUzNDQxNSAxNTEuOTIxMTU4LDU0LjIwNjc4MDUgQzE0Ni40MTAyODQsMzguMzY2MjIyIDEzNi4xMzk0NTMsMjQuNjQwMTMxNyAxMjIuNTMwNjYzLDE0LjkyODQ4NzggQzEwOC45MjE0NTgsNS4yMTY4NDM5IDkyLjY0NzQ1NzksMCA3NS45NjA1Nzg5LDAgQzU5LjI3MzcsMCA0Mi45OTk3LDUuMjE2ODQzOSAyOS4zOTA0OTQ3LDE0LjkyODQ4NzggQzE1Ljc4MTUzODksMjQuNjQwMTMxNyA1LjUxMDgzMjExLDM4LjM2NjIyMiAwLDU0LjIwNjc4MDUgQzE0LjgzMzA4MTYsMzYuNTg5OTI5MyA0My4zMzg1Njg0LDI0LjYyNjQwNzMgNzUuOTc4NDU3OSwyNC42MjY0MDczIEw3NS45Nzg0NTc5LDI0LjYyNjQwNzMgWiIgLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-jupyter: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMzkiIGhlaWdodD0iNTEiIHZpZXdCb3g9IjAgMCAzOSA1MSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgtMTYzOCAtMjI4MSkiPgogICAgIDxnIGNsYXNzPSJqcC1qdXB5dGVyLWljb24tY29sb3IiIGZpbGw9IiNGMzc3MjYiPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM5Ljc0IDIzMTEuOTgpIiBkPSJNIDE4LjI2NDYgNy4xMzQxMUMgMTAuNDE0NSA3LjEzNDExIDMuNTU4NzIgNC4yNTc2IDAgMEMgMS4zMjUzOSAzLjgyMDQgMy43OTU1NiA3LjEzMDgxIDcuMDY4NiA5LjQ3MzAzQyAxMC4zNDE3IDExLjgxNTIgMTQuMjU1NyAxMy4wNzM0IDE4LjI2OSAxMy4wNzM0QyAyMi4yODIzIDEzLjA3MzQgMjYuMTk2MyAxMS44MTUyIDI5LjQ2OTQgOS40NzMwM0MgMzIuNzQyNCA3LjEzMDgxIDM1LjIxMjYgMy44MjA0IDM2LjUzOCAwQyAzMi45NzA1IDQuMjU3NiAyNi4xMTQ4IDcuMTM0MTEgMTguMjY0NiA3LjEzNDExWiIvPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM5LjczIDIyODUuNDgpIiBkPSJNIDE4LjI3MzMgNS45MzkzMUMgMjYuMTIzNSA1LjkzOTMxIDMyLjk3OTMgOC44MTU4MyAzNi41MzggMTMuMDczNEMgMzUuMjEyNiA5LjI1MzAzIDMyLjc0MjQgNS45NDI2MiAyOS40Njk0IDMuNjAwNEMgMjYuMTk2MyAxLjI1ODE4IDIyLjI4MjMgMCAxOC4yNjkgMEMgMTQuMjU1NyAwIDEwLjM0MTcgMS4yNTgxOCA3LjA2ODYgMy42MDA0QyAzLjc5NTU2IDUuOTQyNjIgMS4zMjUzOSA5LjI1MzAzIDAgMTMuMDczNEMgMy41Njc0NSA4LjgyNDYzIDEwLjQyMzIgNS45MzkzMSAxOC4yNzMzIDUuOTM5MzFaIi8+CiAgICA8L2c+CiAgICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjY5LjMgMjI4MS4zMSkiIGQ9Ik0gNS44OTM1MyAyLjg0NEMgNS45MTg4OSAzLjQzMTY1IDUuNzcwODUgNC4wMTM2NyA1LjQ2ODE1IDQuNTE2NDVDIDUuMTY1NDUgNS4wMTkyMiA0LjcyMTY4IDUuNDIwMTUgNC4xOTI5OSA1LjY2ODUxQyAzLjY2NDMgNS45MTY4OCAzLjA3NDQ0IDYuMDAxNTEgMi40OTgwNSA1LjkxMTcxQyAxLjkyMTY2IDUuODIxOSAxLjM4NDYzIDUuNTYxNyAwLjk1NDg5OCA1LjE2NDAxQyAwLjUyNTE3IDQuNzY2MzMgMC4yMjIwNTYgNC4yNDkwMyAwLjA4MzkwMzcgMy42Nzc1N0MgLTAuMDU0MjQ4MyAzLjEwNjExIC0wLjAyMTIzIDIuNTA2MTcgMC4xNzg3ODEgMS45NTM2NEMgMC4zNzg3OTMgMS40MDExIDAuNzM2ODA5IDAuOTIwODE3IDEuMjA3NTQgMC41NzM1MzhDIDEuNjc4MjYgMC4yMjYyNTkgMi4yNDA1NSAwLjAyNzU5MTkgMi44MjMyNiAwLjAwMjY3MjI5QyAzLjYwMzg5IC0wLjAzMDcxMTUgNC4zNjU3MyAwLjI0OTc4OSA0Ljk0MTQyIDAuNzgyNTUxQyA1LjUxNzExIDEuMzE1MzEgNS44NTk1NiAyLjA1Njc2IDUuODkzNTMgMi44NDRaIi8+CiAgICAgIDxwYXRoIHRyYW5zZm9ybT0idHJhbnNsYXRlKDE2MzkuOCAyMzIzLjgxKSIgZD0iTSA3LjQyNzg5IDMuNTgzMzhDIDcuNDYwMDggNC4zMjQzIDcuMjczNTUgNS4wNTgxOSA2Ljg5MTkzIDUuNjkyMTNDIDYuNTEwMzEgNi4zMjYwNyA1Ljk1MDc1IDYuODMxNTYgNS4yODQxMSA3LjE0NDZDIDQuNjE3NDcgNy40NTc2MyAzLjg3MzcxIDcuNTY0MTQgMy4xNDcwMiA3LjQ1MDYzQyAyLjQyMDMyIDcuMzM3MTIgMS43NDMzNiA3LjAwODcgMS4yMDE4NCA2LjUwNjk1QyAwLjY2MDMyOCA2LjAwNTIgMC4yNzg2MSA1LjM1MjY4IDAuMTA1MDE3IDQuNjMyMDJDIC0wLjA2ODU3NTcgMy45MTEzNSAtMC4wMjYyMzYxIDMuMTU0OTQgMC4yMjY2NzUgMi40NTg1NkMgMC40Nzk1ODcgMS43NjIxNyAwLjkzMTY5NyAxLjE1NzEzIDEuNTI1NzYgMC43MjAwMzNDIDIuMTE5ODMgMC4yODI5MzUgMi44MjkxNCAwLjAzMzQzOTUgMy41NjM4OSAwLjAwMzEzMzQ0QyA0LjU0NjY3IC0wLjAzNzQwMzMgNS41MDUyOSAwLjMxNjcwNiA2LjIyOTYxIDAuOTg3ODM1QyA2Ljk1MzkzIDEuNjU4OTYgNy4zODQ4NCAyLjU5MjM1IDcuNDI3ODkgMy41ODMzOEwgNy40Mjc4OSAzLjU4MzM4WiIvPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM4LjM2IDIyODYuMDYpIiBkPSJNIDIuMjc0NzEgNC4zOTYyOUMgMS44NDM2MyA0LjQxNTA4IDEuNDE2NzEgNC4zMDQ0NSAxLjA0Nzk5IDQuMDc4NDNDIDAuNjc5MjY4IDMuODUyNCAwLjM4NTMyOCAzLjUyMTE0IDAuMjAzMzcxIDMuMTI2NTZDIDAuMDIxNDEzNiAyLjczMTk4IC0wLjA0MDM3OTggMi4yOTE4MyAwLjAyNTgxMTYgMS44NjE4MUMgMC4wOTIwMDMxIDEuNDMxOCAwLjI4MzIwNCAxLjAzMTI2IDAuNTc1MjEzIDAuNzEwODgzQyAwLjg2NzIyMiAwLjM5MDUxIDEuMjQ2OTEgMC4xNjQ3MDggMS42NjYyMiAwLjA2MjA1OTJDIDIuMDg1NTMgLTAuMDQwNTg5NyAyLjUyNTYxIC0wLjAxNTQ3MTQgMi45MzA3NiAwLjEzNDIzNUMgMy4zMzU5MSAwLjI4Mzk0MSAzLjY4NzkyIDAuNTUxNTA1IDMuOTQyMjIgMC45MDMwNkMgNC4xOTY1MiAxLjI1NDYyIDQuMzQxNjkgMS42NzQzNiA0LjM1OTM1IDIuMTA5MTZDIDQuMzgyOTkgMi42OTEwNyA0LjE3Njc4IDMuMjU4NjkgMy43ODU5NyAzLjY4NzQ2QyAzLjM5NTE2IDQuMTE2MjQgMi44NTE2NiA0LjM3MTE2IDIuMjc0NzEgNC4zOTYyOUwgMi4yNzQ3MSA0LjM5NjI5WiIvPgogICAgPC9nPgogIDwvZz4+Cjwvc3ZnPgo=);
  --jp-icon-jupyterlab-wordmark: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyMDAiIHZpZXdCb3g9IjAgMCAxODYwLjggNDc1Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0RTRFNEUiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDQ4MC4xMzY0MDEsIDY0LjI3MTQ5MykiPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC4wMDAwMDAsIDU4Ljg3NTU2NikiPgogICAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgwLjA4NzYwMywgMC4xNDAyOTQpIj4KICAgICAgICA8cGF0aCBkPSJNLTQyNi45LDE2OS44YzAsNDguNy0zLjcsNjQuNy0xMy42LDc2LjRjLTEwLjgsMTAtMjUsMTUuNS0zOS43LDE1LjVsMy43LDI5IGMyMi44LDAuMyw0NC44LTcuOSw2MS45LTIzLjFjMTcuOC0xOC41LDI0LTQ0LjEsMjQtODMuM1YwSC00Mjd2MTcwLjFMLTQyNi45LDE2OS44TC00MjYuOSwxNjkuOHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMTU1LjA0NTI5NiwgNTYuODM3MTA0KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEuNTYyNDUzLCAxLjc5OTg0MikiPgogICAgICAgIDxwYXRoIGQ9Ik0tMzEyLDE0OGMwLDIxLDAsMzkuNSwxLjcsNTUuNGgtMzEuOGwtMi4xLTMzLjNoLTAuOGMtNi43LDExLjYtMTYuNCwyMS4zLTI4LDI3LjkgYy0xMS42LDYuNi0yNC44LDEwLTM4LjIsOS44Yy0zMS40LDAtNjktMTcuNy02OS04OVYwaDM2LjR2MTEyLjdjMCwzOC43LDExLjYsNjQuNyw0NC42LDY0LjdjMTAuMy0wLjIsMjAuNC0zLjUsMjguOS05LjQgYzguNS01LjksMTUuMS0xNC4zLDE4LjktMjMuOWMyLjItNi4xLDMuMy0xMi41LDMuMy0xOC45VjAuMmgzNi40VjE0OEgtMzEyTC0zMTIsMTQ4eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgzOTAuMDEzMzIyLCA1My40Nzk2MzgpIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMS43MDY0NTgsIDAuMjMxNDI1KSI+CiAgICAgICAgPHBhdGggZD0iTS00NzguNiw3MS40YzAtMjYtMC44LTQ3LTEuNy02Ni43aDMyLjdsMS43LDM0LjhoMC44YzcuMS0xMi41LDE3LjUtMjIuOCwzMC4xLTI5LjcgYzEyLjUtNywyNi43LTEwLjMsNDEtOS44YzQ4LjMsMCw4NC43LDQxLjcsODQuNywxMDMuM2MwLDczLjEtNDMuNywxMDkuMi05MSwxMDkuMmMtMTIuMSwwLjUtMjQuMi0yLjItMzUtNy44IGMtMTAuOC01LjYtMTkuOS0xMy45LTI2LjYtMjQuMmgtMC44VjI5MWgtMzZ2LTIyMEwtNDc4LjYsNzEuNEwtNDc4LjYsNzEuNHogTS00NDIuNiwxMjUuNmMwLjEsNS4xLDAuNiwxMC4xLDEuNywxNS4xIGMzLDEyLjMsOS45LDIzLjMsMTkuOCwzMS4xYzkuOSw3LjgsMjIuMSwxMi4xLDM0LjcsMTIuMWMzOC41LDAsNjAuNy0zMS45LDYwLjctNzguNWMwLTQwLjctMjEuMS03NS42LTU5LjUtNzUuNiBjLTEyLjksMC40LTI1LjMsNS4xLTM1LjMsMTMuNGMtOS45LDguMy0xNi45LDE5LjctMTkuNiwzMi40Yy0xLjUsNC45LTIuMywxMC0yLjUsMTUuMVYxMjUuNkwtNDQyLjYsMTI1LjZMLTQ0Mi42LDEyNS42eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSg2MDYuNzQwNzI2LCA1Ni44MzcxMDQpIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC43NTEyMjYsIDEuOTg5Mjk5KSI+CiAgICAgICAgPHBhdGggZD0iTS00NDAuOCwwbDQzLjcsMTIwLjFjNC41LDEzLjQsOS41LDI5LjQsMTIuOCw0MS43aDAuOGMzLjctMTIuMiw3LjktMjcuNywxMi44LTQyLjQgbDM5LjctMTE5LjJoMzguNUwtMzQ2LjksMTQ1Yy0yNiw2OS43LTQzLjcsMTA1LjQtNjguNiwxMjcuMmMtMTIuNSwxMS43LTI3LjksMjAtNDQuNiwyMy45bC05LjEtMzEuMSBjMTEuNy0zLjksMjIuNS0xMC4xLDMxLjgtMTguMWMxMy4yLTExLjEsMjMuNy0yNS4yLDMwLjYtNDEuMmMxLjUtMi44LDIuNS01LjcsMi45LTguOGMtMC4zLTMuMy0xLjItNi42LTIuNS05LjdMLTQ4MC4yLDAuMSBoMzkuN0wtNDQwLjgsMEwtNDQwLjgsMHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoODIyLjc0ODEwNCwgMC4wMDAwMDApIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMS40NjQwNTAsIDAuMzc4OTE0KSI+CiAgICAgICAgPHBhdGggZD0iTS00MTMuNywwdjU4LjNoNTJ2MjguMmgtNTJWMTk2YzAsMjUsNywzOS41LDI3LjMsMzkuNWM3LjEsMC4xLDE0LjItMC43LDIxLjEtMi41IGwxLjcsMjcuN2MtMTAuMywzLjctMjEuMyw1LjQtMzIuMiw1Yy03LjMsMC40LTE0LjYtMC43LTIxLjMtMy40Yy02LjgtMi43LTEyLjktNi44LTE3LjktMTIuMWMtMTAuMy0xMC45LTE0LjEtMjktMTQuMS01Mi45IFY4Ni41aC0zMVY1OC4zaDMxVjkuNkwtNDEzLjcsMEwtNDEzLjcsMHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOTc0LjQzMzI4NiwgNTMuNDc5NjM4KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDAuOTkwMDM0LCAwLjYxMDMzOSkiPgogICAgICAgIDxwYXRoIGQ9Ik0tNDQ1LjgsMTEzYzAuOCw1MCwzMi4yLDcwLjYsNjguNiw3MC42YzE5LDAuNiwzNy45LTMsNTUuMy0xMC41bDYuMiwyNi40IGMtMjAuOSw4LjktNDMuNSwxMy4xLTY2LjIsMTIuNmMtNjEuNSwwLTk4LjMtNDEuMi05OC4zLTEwMi41Qy00ODAuMiw0OC4yLTQ0NC43LDAtMzg2LjUsMGM2NS4yLDAsODIuNyw1OC4zLDgyLjcsOTUuNyBjLTAuMSw1LjgtMC41LDExLjUtMS4yLDE3LjJoLTE0MC42SC00NDUuOEwtNDQ1LjgsMTEzeiBNLTMzOS4yLDg2LjZjMC40LTIzLjUtOS41LTYwLjEtNTAuNC02MC4xIGMtMzYuOCwwLTUyLjgsMzQuNC01NS43LDYwLjFILTMzOS4yTC0zMzkuMiw4Ni42TC0zMzkuMiw4Ni42eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxMjAxLjk2MTA1OCwgNTMuNDc5NjM4KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEuMTc5NjQwLCAwLjcwNTA2OCkiPgogICAgICAgIDxwYXRoIGQ9Ik0tNDc4LjYsNjhjMC0yMy45LTAuNC00NC41LTEuNy02My40aDMxLjhsMS4yLDM5LjloMS43YzkuMS0yNy4zLDMxLTQ0LjUsNTUuMy00NC41IGMzLjUtMC4xLDcsMC40LDEwLjMsMS4ydjM0LjhjLTQuMS0wLjktOC4yLTEuMy0xMi40LTEuMmMtMjUuNiwwLTQzLjcsMTkuNy00OC43LDQ3LjRjLTEsNS43LTEuNiwxMS41LTEuNywxNy4ydjEwOC4zaC0zNlY2OCBMLTQ3OC42LDY4eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMCIgZmlsbD0iI0YzNzcyNiI+CiAgICA8cGF0aCBkPSJNMTM1Mi4zLDMyNi4yaDM3VjI4aC0zN1YzMjYuMnogTTE2MDQuOCwzMjYuMmMtMi41LTEzLjktMy40LTMxLjEtMy40LTQ4Ljd2LTc2IGMwLTQwLjctMTUuMS04My4xLTc3LjMtODMuMWMtMjUuNiwwLTUwLDcuMS02Ni44LDE4LjFsOC40LDI0LjRjMTQuMy05LjIsMzQtMTUuMSw1My0xNS4xYzQxLjYsMCw0Ni4yLDMwLjIsNDYuMiw0N3Y0LjIgYy03OC42LTAuNC0xMjIuMywyNi41LTEyMi4zLDc1LjZjMCwyOS40LDIxLDU4LjQsNjIuMiw1OC40YzI5LDAsNTAuOS0xNC4zLDYyLjItMzAuMmgxLjNsMi45LDI1LjZIMTYwNC44eiBNMTU2NS43LDI1Ny43IGMwLDMuOC0wLjgsOC0yLjEsMTEuOGMtNS45LDE3LjItMjIuNywzNC00OS4yLDM0Yy0xOC45LDAtMzQuOS0xMS4zLTM0LjktMzUuM2MwLTM5LjUsNDUuOC00Ni42LDg2LjItNDUuOFYyNTcuN3ogTTE2OTguNSwzMjYuMiBsMS43LTMzLjZoMS4zYzE1LjEsMjYuOSwzOC43LDM4LjIsNjguMSwzOC4yYzQ1LjQsMCw5MS4yLTM2LjEsOTEuMi0xMDguOGMwLjQtNjEuNy0zNS4zLTEwMy43LTg1LjctMTAzLjcgYy0zMi44LDAtNTYuMywxNC43LTY5LjMsMzcuNGgtMC44VjI4aC0zNi42djI0NS43YzAsMTguMS0wLjgsMzguNi0xLjcsNTIuNUgxNjk4LjV6IE0xNzA0LjgsMjA4LjJjMC01LjksMS4zLTEwLjksMi4xLTE1LjEgYzcuNi0yOC4xLDMxLjEtNDUuNCw1Ni4zLTQ1LjRjMzkuNSwwLDYwLjUsMzQuOSw2MC41LDc1LjZjMCw0Ni42LTIzLjEsNzguMS02MS44LDc4LjFjLTI2LjksMC00OC4zLTE3LjYtNTUuNS00My4zIGMtMC44LTQuMi0xLjctOC44LTEuNy0xMy40VjIwOC4yeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-kernel: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgZmlsbD0iIzYxNjE2MSIgZD0iTTE1IDlIOXY2aDZWOXptLTIgNGgtMnYtMmgydjJ6bTgtMlY5aC0yVjdjMC0xLjEtLjktMi0yLTJoLTJWM2gtMnYyaC0yVjNIOXYySDdjLTEuMSAwLTIgLjktMiAydjJIM3YyaDJ2MkgzdjJoMnYyYzAgMS4xLjkgMiAyIDJoMnYyaDJ2LTJoMnYyaDJ2LTJoMmMxLjEgMCAyLS45IDItMnYtMmgydi0yaC0ydi0yaDJ6bS00IDZIN1Y3aDEwdjEweiIvPgo8L3N2Zz4K);
  --jp-icon-keyboard: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMjAgNUg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMTdjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY3YzAtMS4xLS45LTItMi0yem0tOSAzaDJ2MmgtMlY4em0wIDNoMnYyaC0ydi0yek04IDhoMnYySDhWOHptMCAzaDJ2Mkg4di0yem0tMSAySDV2LTJoMnYyem0wLTNINVY4aDJ2MnptOSA3SDh2LTJoOHYyem0wLTRoLTJ2LTJoMnYyem0wLTNoLTJWOGgydjJ6bTMgM2gtMnYtMmgydjJ6bTAtM2gtMlY4aDJ2MnoiLz4KPC9zdmc+Cg==);
  --jp-icon-launch: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMzIgMzIiIHdpZHRoPSIzMiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik0yNiwyOEg2YTIuMDAyNywyLjAwMjcsMCwwLDEtMi0yVjZBMi4wMDI3LDIuMDAyNywwLDAsMSw2LDRIMTZWNkg2VjI2SDI2VjE2aDJWMjZBMi4wMDI3LDIuMDAyNywwLDAsMSwyNiwyOFoiLz4KICAgIDxwb2x5Z29uIHBvaW50cz0iMjAgMiAyMCA0IDI2LjU4NiA0IDE4IDEyLjU4NiAxOS40MTQgMTQgMjggNS40MTQgMjggMTIgMzAgMTIgMzAgMiAyMCAyIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-launcher: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkgMTlINVY1aDdWM0g1YTIgMiAwIDAwLTIgMnYxNGEyIDIgMCAwMDIgMmgxNGMxLjEgMCAyLS45IDItMnYtN2gtMnY3ek0xNCAzdjJoMy41OWwtOS44MyA5LjgzIDEuNDEgMS40MUwxOSA2LjQxVjEwaDJWM2gtN3oiLz4KPC9zdmc+Cg==);
  --jp-icon-line-form: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGZpbGw9IndoaXRlIiBkPSJNNS44OCA0LjEyTDEzLjc2IDEybC03Ljg4IDcuODhMOCAyMmwxMC0xMEw4IDJ6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-link: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTMuOSAxMmMwLTEuNzEgMS4zOS0zLjEgMy4xLTMuMWg0VjdIN2MtMi43NiAwLTUgMi4yNC01IDVzMi4yNCA1IDUgNWg0di0xLjlIN2MtMS43MSAwLTMuMS0xLjM5LTMuMS0zLjF6TTggMTNoOHYtMkg4djJ6bTktNmgtNHYxLjloNGMxLjcxIDAgMy4xIDEuMzkgMy4xIDMuMXMtMS4zOSAzLjEtMy4xIDMuMWgtNFYxN2g0YzIuNzYgMCA1LTIuMjQgNS01cy0yLjI0LTUtNS01eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-list: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiIGQ9Ik0xOSA1djE0SDVWNWgxNG0xLjEtMkgzLjljLS41IDAtLjkuNC0uOS45djE2LjJjMCAuNC40LjkuOS45aDE2LjJjLjQgMCAuOS0uNS45LS45VjMuOWMwLS41LS41LS45LS45LS45ek0xMSA3aDZ2MmgtNlY3em0wIDRoNnYyaC02di0yem0wIDRoNnYyaC02ek03IDdoMnYySDd6bTAgNGgydjJIN3ptMCA0aDJ2Mkg3eiIvPgo8L3N2Zz4K);
  --jp-icon-markdown: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjN0IxRkEyIiBkPSJNNSAxNC45aDEybC02LjEgNnptOS40LTYuOGMwLTEuMy0uMS0yLjktLjEtNC41LS40IDEuNC0uOSAyLjktMS4zIDQuM2wtMS4zIDQuM2gtMkw4LjUgNy45Yy0uNC0xLjMtLjctMi45LTEtNC4zLS4xIDEuNi0uMSAzLjItLjIgNC42TDcgMTIuNEg0LjhsLjctMTFoMy4zTDEwIDVjLjQgMS4yLjcgMi43IDEgMy45LjMtMS4yLjctMi42IDEtMy45bDEuMi0zLjdoMy4zbC42IDExaC0yLjRsLS4zLTQuMnoiLz4KPC9zdmc+Cg==);
  --jp-icon-move-down: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBkPSJNMTIuNDcxIDcuNTI4OTlDMTIuNzYzMiA3LjIzNjg0IDEyLjc2MzIgNi43NjMxNiAxMi40NzEgNi40NzEwMVY2LjQ3MTAxQzEyLjE3OSA2LjE3OTA1IDExLjcwNTcgNi4xNzg4NCAxMS40MTM1IDYuNDcwNTRMNy43NSAxMC4xMjc1VjEuNzVDNy43NSAxLjMzNTc5IDcuNDE0MjEgMSA3IDFWMUM2LjU4NTc5IDEgNi4yNSAxLjMzNTc5IDYuMjUgMS43NVYxMC4xMjc1TDIuNTk3MjYgNi40NjgyMkMyLjMwMzM4IDYuMTczODEgMS44MjY0MSA2LjE3MzU5IDEuNTMyMjYgNi40Njc3NFY2LjQ2Nzc0QzEuMjM4MyA2Ljc2MTcgMS4yMzgzIDcuMjM4MyAxLjUzMjI2IDcuNTMyMjZMNi4yOTI4OSAxMi4yOTI5QzYuNjgzNDIgMTIuNjgzNCA3LjMxNjU4IDEyLjY4MzQgNy43MDcxMSAxMi4yOTI5TDEyLjQ3MSA3LjUyODk5WiIgZmlsbD0iIzYxNjE2MSIvPgo8L3N2Zz4K);
  --jp-icon-move-up: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBkPSJNMS41Mjg5OSA2LjQ3MTAxQzEuMjM2ODQgNi43NjMxNiAxLjIzNjg0IDcuMjM2ODQgMS41Mjg5OSA3LjUyODk5VjcuNTI4OTlDMS44MjA5NSA3LjgyMDk1IDIuMjk0MjYgNy44MjExNiAyLjU4NjQ5IDcuNTI5NDZMNi4yNSAzLjg3MjVWMTIuMjVDNi4yNSAxMi42NjQyIDYuNTg1NzkgMTMgNyAxM1YxM0M3LjQxNDIxIDEzIDcuNzUgMTIuNjY0MiA3Ljc1IDEyLjI1VjMuODcyNUwxMS40MDI3IDcuNTMxNzhDMTEuNjk2NiA3LjgyNjE5IDEyLjE3MzYgNy44MjY0MSAxMi40Njc3IDcuNTMyMjZWNy41MzIyNkMxMi43NjE3IDcuMjM4MyAxMi43NjE3IDYuNzYxNyAxMi40Njc3IDYuNDY3NzRMNy43MDcxMSAxLjcwNzExQzcuMzE2NTggMS4zMTY1OCA2LjY4MzQyIDEuMzE2NTggNi4yOTI4OSAxLjcwNzExTDEuNTI4OTkgNi40NzEwMVoiIGZpbGw9IiM2MTYxNjEiLz4KPC9zdmc+Cg==);
  --jp-icon-new-folder: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIwIDZoLThsLTItMkg0Yy0xLjExIDAtMS45OS44OS0xLjk5IDJMMiAxOGMwIDEuMTEuODkgMiAyIDJoMTZjMS4xMSAwIDItLjg5IDItMlY4YzAtMS4xMS0uODktMi0yLTJ6bS0xIDhoLTN2M2gtMnYtM2gtM3YtMmgzVjloMnYzaDN2MnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-not-trusted: url(data:image/svg+xml;base64,PHN2ZyBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI1IDI1Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDMgMykiIGQ9Ik0xLjg2MDk0IDExLjQ0MDlDMC44MjY0NDggOC43NzAyNyAwLjg2Mzc3OSA2LjA1NzY0IDEuMjQ5MDcgNC4xOTkzMkMyLjQ4MjA2IDMuOTMzNDcgNC4wODA2OCAzLjQwMzQ3IDUuNjAxMDIgMi44NDQ5QzcuMjM1NDkgMi4yNDQ0IDguODU2NjYgMS41ODE1IDkuOTg3NiAxLjA5NTM5QzExLjA1OTcgMS41ODM0MSAxMi42MDk0IDIuMjQ0NCAxNC4yMTggMi44NDMzOUMxNS43NTAzIDMuNDEzOTQgMTcuMzk5NSAzLjk1MjU4IDE4Ljc1MzkgNC4yMTM4NUMxOS4xMzY0IDYuMDcxNzcgMTkuMTcwOSA4Ljc3NzIyIDE4LjEzOSAxMS40NDA5QzE3LjAzMDMgMTQuMzAzMiAxNC42NjY4IDE3LjE4NDQgOS45OTk5OSAxOC45MzU0QzUuMzMzMTkgMTcuMTg0NCAyLjk2OTY4IDE0LjMwMzIgMS44NjA5NCAxMS40NDA5WiIvPgogICAgPHBhdGggY2xhc3M9ImpwLWljb24yIiBzdHJva2U9IiMzMzMzMzMiIHN0cm9rZS13aWR0aD0iMiIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOS4zMTU5MiA5LjMyMDMxKSIgZD0iTTcuMzY4NDIgMEwwIDcuMzY0NzkiLz4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDkuMzE1OTIgMTYuNjgzNikgc2NhbGUoMSAtMSkiIGQ9Ik03LjM2ODQyIDBMMCA3LjM2NDc5Ii8+Cjwvc3ZnPgo=);
  --jp-icon-notebook: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtbm90ZWJvb2staWNvbi1jb2xvciBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNFRjZDMDAiPgogICAgPHBhdGggZD0iTTE4LjcgMy4zdjE1LjRIMy4zVjMuM2gxNS40bTEuNS0xLjVIMS44djE4LjNoMTguM2wuMS0xOC4zeiIvPgogICAgPHBhdGggZD0iTTE2LjUgMTYuNWwtNS40LTQuMy01LjYgNC4zdi0xMWgxMXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-numbering: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjIiIGhlaWdodD0iMjIiIHZpZXdCb3g9IjAgMCAyOCAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTQgMTlINlYxOS41SDVWMjAuNUg2VjIxSDRWMjJIN1YxOEg0VjE5Wk01IDEwSDZWNkg0VjdINVYxMFpNNCAxM0g1LjhMNCAxNS4xVjE2SDdWMTVINS4yTDcgMTIuOVYxMkg0VjEzWk05IDdWOUgyM1Y3SDlaTTkgMjFIMjNWMTlIOVYyMVpNOSAxNUgyM1YxM0g5VjE1WiIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-offline-bolt: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjE2Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyIDIuMDJjLTUuNTEgMC05Ljk4IDQuNDctOS45OCA5Ljk4czQuNDcgOS45OCA5Ljk4IDkuOTggOS45OC00LjQ3IDkuOTgtOS45OFMxNy41MSAyLjAyIDEyIDIuMDJ6TTExLjQ4IDIwdi02LjI2SDhMMTMgNHY2LjI2aDMuMzVMMTEuNDggMjB6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-palette: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE4IDEzVjIwSDRWNkg5LjAyQzkuMDcgNS4yOSA5LjI0IDQuNjIgOS41IDRINEMyLjkgNCAyIDQuOSAyIDZWMjBDMiAyMS4xIDIuOSAyMiA0IDIySDE4QzE5LjEgMjIgMjAgMjEuMSAyMCAyMFYxNUwxOCAxM1pNMTkuMyA4Ljg5QzE5Ljc0IDguMTkgMjAgNy4zOCAyMCA2LjVDMjAgNC4wMSAxNy45OSAyIDE1LjUgMkMxMy4wMSAyIDExIDQuMDEgMTEgNi41QzExIDguOTkgMTMuMDEgMTEgMTUuNDkgMTFDMTYuMzcgMTEgMTcuMTkgMTAuNzQgMTcuODggMTAuM0wyMSAxMy40MkwyMi40MiAxMkwxOS4zIDguODlaTTE1LjUgOUMxNC4xMiA5IDEzIDcuODggMTMgNi41QzEzIDUuMTIgMTQuMTIgNCAxNS41IDRDMTYuODggNCAxOCA1LjEyIDE4IDYuNUMxOCA3Ljg4IDE2Ljg4IDkgMTUuNSA5WiIvPgogICAgPHBhdGggZmlsbC1ydWxlPSJldmVub2RkIiBjbGlwLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik00IDZIOS4wMTg5NEM5LjAwNjM5IDYuMTY1MDIgOSA2LjMzMTc2IDkgNi41QzkgOC44MTU3NyAxMC4yMTEgMTAuODQ4NyAxMi4wMzQzIDEySDlWMTRIMTZWMTIuOTgxMUMxNi41NzAzIDEyLjkzNzcgMTcuMTIgMTIuODIwNyAxNy42Mzk2IDEyLjYzOTZMMTggMTNWMjBINFY2Wk04IDhINlYxMEg4VjhaTTYgMTJIOFYxNEg2VjEyWk04IDE2SDZWMThIOFYxNlpNOSAxNkgxNlYxOEg5VjE2WiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-paste: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTE5IDJoLTQuMThDMTQuNC44NCAxMy4zIDAgMTIgMGMtMS4zIDAtMi40Ljg0LTIuODIgMkg1Yy0xLjEgMC0yIC45LTIgMnYxNmMwIDEuMS45IDIgMiAyaDE0YzEuMSAwIDItLjkgMi0yVjRjMC0xLjEtLjktMi0yLTJ6bS03IDBjLjU1IDAgMSAuNDUgMSAxcy0uNDUgMS0xIDEtMS0uNDUtMS0xIC40NS0xIDEtMXptNyAxOEg1VjRoMnYzaDEwVjRoMnYxNnoiLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-pdf: url(data:image/svg+xml;base64,PHN2ZwogICB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyMiAyMiIgd2lkdGg9IjE2Ij4KICAgIDxwYXRoIHRyYW5zZm9ybT0icm90YXRlKDQ1KSIgY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI0ZGMkEyQSIKICAgICAgIGQ9Im0gMjIuMzQ0MzY5LC0zLjAxNjM2NDIgaCA1LjYzODYwNCB2IDEuNTc5MjQzMyBoIC0zLjU0OTIyNyB2IDEuNTA4NjkyOTkgaCAzLjMzNzU3NiBWIDEuNjUwODE1NCBoIC0zLjMzNzU3NiB2IDMuNDM1MjYxMyBoIC0yLjA4OTM3NyB6IG0gLTcuMTM2NDQ0LDEuNTc5MjQzMyB2IDQuOTQzOTU0MyBoIDAuNzQ4OTIgcSAxLjI4MDc2MSwwIDEuOTUzNzAzLC0wLjYzNDk1MzUgMC42NzgzNjksLTAuNjM0OTUzNSAwLjY3ODM2OSwtMS44NDUxNjQxIDAsLTEuMjA0NzgzNTUgLTAuNjcyOTQyLC0xLjgzNDMxMDExIC0wLjY3Mjk0MiwtMC42Mjk1MjY1OSAtMS45NTkxMywtMC42Mjk1MjY1OSB6IG0gLTIuMDg5Mzc3LC0xLjU3OTI0MzMgaCAyLjIwMzM0MyBxIDEuODQ1MTY0LDAgMi43NDYwMzksMC4yNjU5MjA3IDAuOTA2MzAxLDAuMjYwNDkzNyAxLjU1MjEwOCwwLjg5MDAyMDMgMC41Njk4MywwLjU0ODEyMjMgMC44NDY2MDUsMS4yNjQ0ODAwNiAwLjI3Njc3NCwwLjcxNjM1NzgxIDAuMjc2Nzc0LDEuNjIyNjU4OTQgMCwwLjkxNzE1NTEgLTAuMjc2Nzc0LDEuNjM4OTM5OSAtMC4yNzY3NzUsMC43MTYzNTc4IC0wLjg0NjYwNSwxLjI2NDQ4IC0wLjY1MTIzNCwwLjYyOTUyNjYgLTEuNTYyOTYyLDAuODk1NDQ3MyAtMC45MTE3MjgsMC4yNjA0OTM3IC0yLjczNTE4NSwwLjI2MDQ5MzcgaCAtMi4yMDMzNDMgeiBtIC04LjE0NTg1NjUsMCBoIDMuNDY3ODIzIHEgMS41NDY2ODE2LDAgMi4zNzE1Nzg1LDAuNjg5MjIzIDAuODMwMzI0LDAuNjgzNzk2MSAwLjgzMDMyNCwxLjk1MzcwMzE0IDAsMS4yNzUzMzM5NyAtMC44MzAzMjQsMS45NjQ1NTcwNiBRIDkuOTg3MTk2MSwyLjI3NDkxNSA4LjQ0MDUxNDUsMi4yNzQ5MTUgSCA3LjA2MjA2ODQgViA1LjA4NjA3NjcgSCA0Ljk3MjY5MTUgWiBtIDIuMDg5Mzc2OSwxLjUxNDExOTkgdiAyLjI2MzAzOTQzIGggMS4xNTU5NDEgcSAwLjYwNzgxODgsMCAwLjkzODg2MjksLTAuMjkzMDU1NDcgMC4zMzEwNDQxLC0wLjI5ODQ4MjQxIDAuMzMxMDQ0MSwtMC44NDExNzc3MiAwLC0wLjU0MjY5NTMxIC0wLjMzMTA0NDEsLTAuODM1NzUwNzQgLTAuMzMxMDQ0MSwtMC4yOTMwNTU1IC0wLjkzODg2MjksLTAuMjkzMDU1NSB6IgovPgo8L3N2Zz4K);
  --jp-icon-python: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iLTEwIC0xMCAxMzEuMTYxMzYxNjk0MzM1OTQgMTMyLjM4ODk5OTkzODk2NDg0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMzA2OTk4IiBkPSJNIDU0LjkxODc4NSw5LjE5Mjc0MjFlLTQgQyA1MC4zMzUxMzIsMC4wMjIyMTcyNyA0NS45NTc4NDYsMC40MTMxMzY5NyA0Mi4xMDYyODUsMS4wOTQ2NjkzIDMwLjc2MDA2OSwzLjA5OTE3MzEgMjguNzAwMDM2LDcuMjk0NzcxNCAyOC43MDAwMzUsMTUuMDMyMTY5IHYgMTAuMjE4NzUgaCAyNi44MTI1IHYgMy40MDYyNSBoIC0yNi44MTI1IC0xMC4wNjI1IGMgLTcuNzkyNDU5LDAgLTE0LjYxNTc1ODgsNC42ODM3MTcgLTE2Ljc0OTk5OTgsMTMuNTkzNzUgLTIuNDYxODE5OTgsMTAuMjEyOTY2IC0yLjU3MTAxNTA4LDE2LjU4NjAyMyAwLDI3LjI1IDEuOTA1OTI4Myw3LjkzNzg1MiA2LjQ1NzU0MzIsMTMuNTkzNzQ4IDE0LjI0OTk5OTgsMTMuNTkzNzUgaCA5LjIxODc1IHYgLTEyLjI1IGMgMCwtOC44NDk5MDIgNy42NTcxNDQsLTE2LjY1NjI0OCAxNi43NSwtMTYuNjU2MjUgaCAyNi43ODEyNSBjIDcuNDU0OTUxLDAgMTMuNDA2MjUzLC02LjEzODE2NCAxMy40MDYyNSwtMTMuNjI1IHYgLTI1LjUzMTI1IGMgMCwtNy4yNjYzMzg2IC02LjEyOTk4LC0xMi43MjQ3NzcxIC0xMy40MDYyNSwtMTMuOTM3NDk5NyBDIDY0LjI4MTU0OCwwLjMyNzk0Mzk3IDU5LjUwMjQzOCwtMC4wMjAzNzkwMyA1NC45MTg3ODUsOS4xOTI3NDIxZS00IFogbSAtMTQuNSw4LjIxODc1MDEyNTc5IGMgMi43Njk1NDcsMCA1LjAzMTI1LDIuMjk4NjQ1NiA1LjAzMTI1LDUuMTI0OTk5NiAtMmUtNiwyLjgxNjMzNiAtMi4yNjE3MDMsNS4wOTM3NSAtNS4wMzEyNSw1LjA5Mzc1IC0yLjc3OTQ3NiwtMWUtNiAtNS4wMzEyNSwtMi4yNzc0MTUgLTUuMDMxMjUsLTUuMDkzNzUgLTEwZS03LC0yLjgyNjM1MyAyLjI1MTc3NCwtNS4xMjQ5OTk2IDUuMDMxMjUsLTUuMTI0OTk5NiB6Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI2ZmZDQzYiIgZD0ibSA4NS42Mzc1MzUsMjguNjU3MTY5IHYgMTEuOTA2MjUgYyAwLDkuMjMwNzU1IC03LjgyNTg5NSwxNi45OTk5OTkgLTE2Ljc1LDE3IGggLTI2Ljc4MTI1IGMgLTcuMzM1ODMzLDAgLTEzLjQwNjI0OSw2LjI3ODQ4MyAtMTMuNDA2MjUsMTMuNjI1IHYgMjUuNTMxMjQ3IGMgMCw3LjI2NjM0NCA2LjMxODU4OCwxMS41NDAzMjQgMTMuNDA2MjUsMTMuNjI1MDA0IDguNDg3MzMxLDIuNDk1NjEgMTYuNjI2MjM3LDIuOTQ2NjMgMjYuNzgxMjUsMCA2Ljc1MDE1NSwtMS45NTQzOSAxMy40MDYyNTMsLTUuODg3NjEgMTMuNDA2MjUsLTEzLjYyNTAwNCBWIDg2LjUwMDkxOSBoIC0yNi43ODEyNSB2IC0zLjQwNjI1IGggMjYuNzgxMjUgMTMuNDA2MjU0IGMgNy43OTI0NjEsMCAxMC42OTYyNTEsLTUuNDM1NDA4IDEzLjQwNjI0MSwtMTMuNTkzNzUgMi43OTkzMywtOC4zOTg4ODYgMi42ODAyMiwtMTYuNDc1Nzc2IDAsLTI3LjI1IC0xLjkyNTc4LC03Ljc1NzQ0MSAtNS42MDM4NywtMTMuNTkzNzUgLTEzLjQwNjI0MSwtMTMuNTkzNzUgeiBtIC0xNS4wNjI1LDY0LjY1NjI1IGMgMi43Nzk0NzgsM2UtNiA1LjAzMTI1LDIuMjc3NDE3IDUuMDMxMjUsNS4wOTM3NDcgLTJlLTYsMi44MjYzNTQgLTIuMjUxNzc1LDUuMTI1MDA0IC01LjAzMTI1LDUuMTI1MDA0IC0yLjc2OTU1LDAgLTUuMDMxMjUsLTIuMjk4NjUgLTUuMDMxMjUsLTUuMTI1MDA0IDJlLTYsLTIuODE2MzMgMi4yNjE2OTcsLTUuMDkzNzQ3IDUuMDMxMjUsLTUuMDkzNzQ3IHoiLz4KPC9zdmc+Cg==);
  --jp-icon-r-kernel: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMjE5NkYzIiBkPSJNNC40IDIuNWMxLjItLjEgMi45LS4zIDQuOS0uMyAyLjUgMCA0LjEuNCA1LjIgMS4zIDEgLjcgMS41IDEuOSAxLjUgMy41IDAgMi0xLjQgMy41LTIuOSA0LjEgMS4yLjQgMS43IDEuNiAyLjIgMyAuNiAxLjkgMSAzLjkgMS4zIDQuNmgtMy44Yy0uMy0uNC0uOC0xLjctMS4yLTMuN3MtMS4yLTIuNi0yLjYtMi42aC0uOXY2LjRINC40VjIuNXptMy43IDYuOWgxLjRjMS45IDAgMi45LS45IDIuOS0yLjNzLTEtMi4zLTIuOC0yLjNjLS43IDAtMS4zIDAtMS42LjJ2NC41aC4xdi0uMXoiLz4KPC9zdmc+Cg==);
  --jp-icon-react: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMTUwIDE1MCA1NDEuOSAyOTUuMyI+CiAgPGcgY2xhc3M9ImpwLWljb24tYnJhbmQyIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzYxREFGQiI+CiAgICA8cGF0aCBkPSJNNjY2LjMgMjk2LjVjMC0zMi41LTQwLjctNjMuMy0xMDMuMS04Mi40IDE0LjQtNjMuNiA4LTExNC4yLTIwLjItMTMwLjQtNi41LTMuOC0xNC4xLTUuNi0yMi40LTUuNnYyMi4zYzQuNiAwIDguMy45IDExLjQgMi42IDEzLjYgNy44IDE5LjUgMzcuNSAxNC45IDc1LjctMS4xIDkuNC0yLjkgMTkuMy01LjEgMjkuNC0xOS42LTQuOC00MS04LjUtNjMuNS0xMC45LTEzLjUtMTguNS0yNy41LTM1LjMtNDEuNi01MCAzMi42LTMwLjMgNjMuMi00Ni45IDg0LTQ2LjlWNzhjLTI3LjUgMC02My41IDE5LjYtOTkuOSA1My42LTM2LjQtMzMuOC03Mi40LTUzLjItOTkuOS01My4ydjIyLjNjMjAuNyAwIDUxLjQgMTYuNSA4NCA0Ni42LTE0IDE0LjctMjggMzEuNC00MS4zIDQ5LjktMjIuNiAyLjQtNDQgNi4xLTYzLjYgMTEtMi4zLTEwLTQtMTkuNy01LjItMjktNC43LTM4LjIgMS4xLTY3LjkgMTQuNi03NS44IDMtMS44IDYuOS0yLjYgMTEuNS0yLjZWNzguNWMtOC40IDAtMTYgMS44LTIyLjYgNS42LTI4LjEgMTYuMi0zNC40IDY2LjctMTkuOSAxMzAuMS02Mi4yIDE5LjItMTAyLjcgNDkuOS0xMDIuNyA4Mi4zIDAgMzIuNSA0MC43IDYzLjMgMTAzLjEgODIuNC0xNC40IDYzLjYtOCAxMTQuMiAyMC4yIDEzMC40IDYuNSAzLjggMTQuMSA1LjYgMjIuNSA1LjYgMjcuNSAwIDYzLjUtMTkuNiA5OS45LTUzLjYgMzYuNCAzMy44IDcyLjQgNTMuMiA5OS45IDUzLjIgOC40IDAgMTYtMS44IDIyLjYtNS42IDI4LjEtMTYuMiAzNC40LTY2LjcgMTkuOS0xMzAuMSA2Mi0xOS4xIDEwMi41LTQ5LjkgMTAyLjUtODIuM3ptLTEzMC4yLTY2LjdjLTMuNyAxMi45LTguMyAyNi4yLTEzLjUgMzkuNS00LjEtOC04LjQtMTYtMTMuMS0yNC00LjYtOC05LjUtMTUuOC0xNC40LTIzLjQgMTQuMiAyLjEgMjcuOSA0LjcgNDEgNy45em0tNDUuOCAxMDYuNWMtNy44IDEzLjUtMTUuOCAyNi4zLTI0LjEgMzguMi0xNC45IDEuMy0zMCAyLTQ1LjIgMi0xNS4xIDAtMzAuMi0uNy00NS0xLjktOC4zLTExLjktMTYuNC0yNC42LTI0LjItMzgtNy42LTEzLjEtMTQuNS0yNi40LTIwLjgtMzkuOCA2LjItMTMuNCAxMy4yLTI2LjggMjAuNy0zOS45IDcuOC0xMy41IDE1LjgtMjYuMyAyNC4xLTM4LjIgMTQuOS0xLjMgMzAtMiA0NS4yLTIgMTUuMSAwIDMwLjIuNyA0NSAxLjkgOC4zIDExLjkgMTYuNCAyNC42IDI0LjIgMzggNy42IDEzLjEgMTQuNSAyNi40IDIwLjggMzkuOC02LjMgMTMuNC0xMy4yIDI2LjgtMjAuNyAzOS45em0zMi4zLTEzYzUuNCAxMy40IDEwIDI2LjggMTMuOCAzOS44LTEzLjEgMy4yLTI2LjkgNS45LTQxLjIgOCA0LjktNy43IDkuOC0xNS42IDE0LjQtMjMuNyA0LjYtOCA4LjktMTYuMSAxMy0yNC4xek00MjEuMiA0MzBjLTkuMy05LjYtMTguNi0yMC4zLTI3LjgtMzIgOSAuNCAxOC4yLjcgMjcuNS43IDkuNCAwIDE4LjctLjIgMjcuOC0uNy05IDExLjctMTguMyAyMi40LTI3LjUgMzJ6bS03NC40LTU4LjljLTE0LjItMi4xLTI3LjktNC43LTQxLTcuOSAzLjctMTIuOSA4LjMtMjYuMiAxMy41LTM5LjUgNC4xIDggOC40IDE2IDEzLjEgMjQgNC43IDggOS41IDE1LjggMTQuNCAyMy40ek00MjAuNyAxNjNjOS4zIDkuNiAxOC42IDIwLjMgMjcuOCAzMi05LS40LTE4LjItLjctMjcuNS0uNy05LjQgMC0xOC43LjItMjcuOC43IDktMTEuNyAxOC4zLTIyLjQgMjcuNS0zMnptLTc0IDU4LjljLTQuOSA3LjctOS44IDE1LjYtMTQuNCAyMy43LTQuNiA4LTguOSAxNi0xMyAyNC01LjQtMTMuNC0xMC0yNi44LTEzLjgtMzkuOCAxMy4xLTMuMSAyNi45LTUuOCA0MS4yLTcuOXptLTkwLjUgMTI1LjJjLTM1LjQtMTUuMS01OC4zLTM0LjktNTguMy01MC42IDAtMTUuNyAyMi45LTM1LjYgNTguMy01MC42IDguNi0zLjcgMTgtNyAyNy43LTEwLjEgNS43IDE5LjYgMTMuMiA0MCAyMi41IDYwLjktOS4yIDIwLjgtMTYuNiA0MS4xLTIyLjIgNjAuNi05LjktMy4xLTE5LjMtNi41LTI4LTEwLjJ6TTMxMCA0OTBjLTEzLjYtNy44LTE5LjUtMzcuNS0xNC45LTc1LjcgMS4xLTkuNCAyLjktMTkuMyA1LjEtMjkuNCAxOS42IDQuOCA0MSA4LjUgNjMuNSAxMC45IDEzLjUgMTguNSAyNy41IDM1LjMgNDEuNiA1MC0zMi42IDMwLjMtNjMuMiA0Ni45LTg0IDQ2LjktNC41LS4xLTguMy0xLTExLjMtMi43em0yMzcuMi03Ni4yYzQuNyAzOC4yLTEuMSA2Ny45LTE0LjYgNzUuOC0zIDEuOC02LjkgMi42LTExLjUgMi42LTIwLjcgMC01MS40LTE2LjUtODQtNDYuNiAxNC0xNC43IDI4LTMxLjQgNDEuMy00OS45IDIyLjYtMi40IDQ0LTYuMSA2My42LTExIDIuMyAxMC4xIDQuMSAxOS44IDUuMiAyOS4xem0zOC41LTY2LjdjLTguNiAzLjctMTggNy0yNy43IDEwLjEtNS43LTE5LjYtMTMuMi00MC0yMi41LTYwLjkgOS4yLTIwLjggMTYuNi00MS4xIDIyLjItNjAuNiA5LjkgMy4xIDE5LjMgNi41IDI4LjEgMTAuMiAzNS40IDE1LjEgNTguMyAzNC45IDU4LjMgNTAuNi0uMSAxNS43LTIzIDM1LjYtNTguNCA1MC42ek0zMjAuOCA3OC40eiIvPgogICAgPGNpcmNsZSBjeD0iNDIwLjkiIGN5PSIyOTYuNSIgcj0iNDUuNyIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-redo: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjE2Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgICA8cGF0aCBkPSJNMCAwaDI0djI0SDB6IiBmaWxsPSJub25lIi8+PHBhdGggZD0iTTE4LjQgMTAuNkMxNi41NSA4Ljk5IDE0LjE1IDggMTEuNSA4Yy00LjY1IDAtOC41OCAzLjAzLTkuOTYgNy4yMkwzLjkgMTZjMS4wNS0zLjE5IDQuMDUtNS41IDcuNi01LjUgMS45NSAwIDMuNzMuNzIgNS4xMiAxLjg4TDEzIDE2aDlWN2wtMy42IDMuNnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-refresh: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTkgMTMuNWMtMi40OSAwLTQuNS0yLjAxLTQuNS00LjVTNi41MSA0LjUgOSA0LjVjMS4yNCAwIDIuMzYuNTIgMy4xNyAxLjMzTDEwIDhoNVYzbC0xLjc2IDEuNzZDMTIuMTUgMy42OCAxMC42NiAzIDkgMyA1LjY5IDMgMy4wMSA1LjY5IDMuMDEgOVM1LjY5IDE1IDkgMTVjMi45NyAwIDUuNDMtMi4xNiA1LjktNWgtMS41MmMtLjQ2IDItMi4yNCAzLjUtNC4zOCAzLjV6Ii8+CiAgICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-regex: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0MTQxNDEiPgogICAgPHJlY3QgeD0iMiIgeT0iMiIgd2lkdGg9IjE2IiBoZWlnaHQ9IjE2Ii8+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbi1hY2NlbnQyIiBmaWxsPSIjRkZGIj4KICAgIDxjaXJjbGUgY2xhc3M9InN0MiIgY3g9IjUuNSIgY3k9IjE0LjUiIHI9IjEuNSIvPgogICAgPHJlY3QgeD0iMTIiIHk9IjQiIGNsYXNzPSJzdDIiIHdpZHRoPSIxIiBoZWlnaHQ9IjgiLz4KICAgIDxyZWN0IHg9IjguNSIgeT0iNy41IiB0cmFuc2Zvcm09Im1hdHJpeCgwLjg2NiAtMC41IDAuNSAwLjg2NiAtMi4zMjU1IDcuMzIxOSkiIGNsYXNzPSJzdDIiIHdpZHRoPSI4IiBoZWlnaHQ9IjEiLz4KICAgIDxyZWN0IHg9IjEyIiB5PSI0IiB0cmFuc2Zvcm09Im1hdHJpeCgwLjUgLTAuODY2IDAuODY2IDAuNSAtMC42Nzc5IDE0LjgyNTIpIiBjbGFzcz0ic3QyIiB3aWR0aD0iMSIgaGVpZ2h0PSI4Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-run: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTggNXYxNGwxMS03eiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-running: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUxMiA1MTIiPgogIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICA8cGF0aCBkPSJNMjU2IDhDMTE5IDggOCAxMTkgOCAyNTZzMTExIDI0OCAyNDggMjQ4IDI0OC0xMTEgMjQ4LTI0OFMzOTMgOCAyNTYgOHptOTYgMzI4YzAgOC44LTcuMiAxNi0xNiAxNkgxNzZjLTguOCAwLTE2LTcuMi0xNi0xNlYxNzZjMC04LjggNy4yLTE2IDE2LTE2aDE2MGM4LjggMCAxNiA3LjIgMTYgMTZ2MTYweiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-save: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTE3IDNINWMtMS4xMSAwLTIgLjktMiAydjE0YzAgMS4xLjg5IDIgMiAyaDE0YzEuMSAwIDItLjkgMi0yVjdsLTQtNHptLTUgMTZjLTEuNjYgMC0zLTEuMzQtMy0zczEuMzQtMyAzLTMgMyAxLjM0IDMgMy0xLjM0IDMtMyAzem0zLTEwSDVWNWgxMHY0eiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-search: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyLjEsMTAuOWgtMC43bC0wLjItMC4yYzAuOC0wLjksMS4zLTIuMiwxLjMtMy41YzAtMy0yLjQtNS40LTUuNC01LjRTMS44LDQuMiwxLjgsNy4xczIuNCw1LjQsNS40LDUuNCBjMS4zLDAsMi41LTAuNSwzLjUtMS4zbDAuMiwwLjJ2MC43bDQuMSw0LjFsMS4yLTEuMkwxMi4xLDEwLjl6IE03LjEsMTAuOWMtMi4xLDAtMy43LTEuNy0zLjctMy43czEuNy0zLjcsMy43LTMuN3MzLjcsMS43LDMuNywzLjcgUzkuMiwxMC45LDcuMSwxMC45eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-settings: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkuNDMgMTIuOThjLjA0LS4zMi4wNy0uNjQuMDctLjk4cy0uMDMtLjY2LS4wNy0uOThsMi4xMS0xLjY1Yy4xOS0uMTUuMjQtLjQyLjEyLS42NGwtMi0zLjQ2Yy0uMTItLjIyLS4zOS0uMy0uNjEtLjIybC0yLjQ5IDFjLS41Mi0uNC0xLjA4LS43My0xLjY5LS45OGwtLjM4LTIuNjVBLjQ4OC40ODggMCAwMDE0IDJoLTRjLS4yNSAwLS40Ni4xOC0uNDkuNDJsLS4zOCAyLjY1Yy0uNjEuMjUtMS4xNy41OS0xLjY5Ljk4bC0yLjQ5LTFjLS4yMy0uMDktLjQ5IDAtLjYxLjIybC0yIDMuNDZjLS4xMy4yMi0uMDcuNDkuMTIuNjRsMi4xMSAxLjY1Yy0uMDQuMzItLjA3LjY1LS4wNy45OHMuMDMuNjYuMDcuOThsLTIuMTEgMS42NWMtLjE5LjE1LS4yNC40Mi0uMTIuNjRsMiAzLjQ2Yy4xMi4yMi4zOS4zLjYxLjIybDIuNDktMWMuNTIuNCAxLjA4LjczIDEuNjkuOThsLjM4IDIuNjVjLjAzLjI0LjI0LjQyLjQ5LjQyaDRjLjI1IDAgLjQ2LS4xOC40OS0uNDJsLjM4LTIuNjVjLjYxLS4yNSAxLjE3LS41OSAxLjY5LS45OGwyLjQ5IDFjLjIzLjA5LjQ5IDAgLjYxLS4yMmwyLTMuNDZjLjEyLS4yMi4wNy0uNDktLjEyLS42NGwtMi4xMS0xLjY1ek0xMiAxNS41Yy0xLjkzIDAtMy41LTEuNTctMy41LTMuNXMxLjU3LTMuNSAzLjUtMy41IDMuNSAxLjU3IDMuNSAzLjUtMS41NyAzLjUtMy41IDMuNXoiLz4KPC9zdmc+Cg==);
  --jp-icon-share: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTYiIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTSAxOCAyIEMgMTYuMzU0OTkgMiAxNSAzLjM1NDk5MDQgMTUgNSBDIDE1IDUuMTkwOTUyOSAxNS4wMjE3OTEgNS4zNzcxMjI0IDE1LjA1NjY0MSA1LjU1ODU5MzggTCA3LjkyMTg3NSA5LjcyMDcwMzEgQyA3LjM5ODUzOTkgOS4yNzc4NTM5IDYuNzMyMDc3MSA5IDYgOSBDIDQuMzU0OTkwNCA5IDMgMTAuMzU0OTkgMyAxMiBDIDMgMTMuNjQ1MDEgNC4zNTQ5OTA0IDE1IDYgMTUgQyA2LjczMjA3NzEgMTUgNy4zOTg1Mzk5IDE0LjcyMjE0NiA3LjkyMTg3NSAxNC4yNzkyOTcgTCAxNS4wNTY2NDEgMTguNDM5NDUzIEMgMTUuMDIxNTU1IDE4LjYyMTUxNCAxNSAxOC44MDgzODYgMTUgMTkgQyAxNSAyMC42NDUwMSAxNi4zNTQ5OSAyMiAxOCAyMiBDIDE5LjY0NTAxIDIyIDIxIDIwLjY0NTAxIDIxIDE5IEMgMjEgMTcuMzU0OTkgMTkuNjQ1MDEgMTYgMTggMTYgQyAxNy4yNjc0OCAxNiAxNi42MDE1OTMgMTYuMjc5MzI4IDE2LjA3ODEyNSAxNi43MjI2NTYgTCA4Ljk0MzM1OTQgMTIuNTU4NTk0IEMgOC45NzgyMDk1IDEyLjM3NzEyMiA5IDEyLjE5MDk1MyA5IDEyIEMgOSAxMS44MDkwNDcgOC45NzgyMDk1IDExLjYyMjg3OCA4Ljk0MzM1OTQgMTEuNDQxNDA2IEwgMTYuMDc4MTI1IDcuMjc5Mjk2OSBDIDE2LjYwMTQ2IDcuNzIyMTQ2MSAxNy4yNjc5MjMgOCAxOCA4IEMgMTkuNjQ1MDEgOCAyMSA2LjY0NTAwOTYgMjEgNSBDIDIxIDMuMzU0OTkwNCAxOS42NDUwMSAyIDE4IDIgeiBNIDE4IDQgQyAxOC41NjQxMjkgNCAxOSA0LjQzNTg3MDYgMTkgNSBDIDE5IDUuNTY0MTI5NCAxOC41NjQxMjkgNiAxOCA2IEMgMTcuNDM1ODcxIDYgMTcgNS41NjQxMjk0IDE3IDUgQyAxNyA0LjQzNTg3MDYgMTcuNDM1ODcxIDQgMTggNCB6IE0gNiAxMSBDIDYuNTY0MTI5NCAxMSA3IDExLjQzNTg3MSA3IDEyIEMgNyAxMi41NjQxMjkgNi41NjQxMjk0IDEzIDYgMTMgQyA1LjQzNTg3MDYgMTMgNSAxMi41NjQxMjkgNSAxMiBDIDUgMTEuNDM1ODcxIDUuNDM1ODcwNiAxMSA2IDExIHogTSAxOCAxOCBDIDE4LjU2NDEyOSAxOCAxOSAxOC40MzU4NzEgMTkgMTkgQyAxOSAxOS41NjQxMjkgMTguNTY0MTI5IDIwIDE4IDIwIEMgMTcuNDM1ODcxIDIwIDE3IDE5LjU2NDEyOSAxNyAxOSBDIDE3IDE4LjQzNTg3MSAxNy40MzU4NzEgMTggMTggMTggeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-spreadsheet: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDEganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNENBRjUwIiBkPSJNMi4yIDIuMnYxNy42aDE3LjZWMi4ySDIuMnptMTUuNCA3LjdoLTUuNVY0LjRoNS41djUuNXpNOS45IDQuNHY1LjVINC40VjQuNGg1LjV6bS01LjUgNy43aDUuNXY1LjVINC40di01LjV6bTcuNyA1LjV2LTUuNWg1LjV2NS41aC01LjV6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-stop: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik02IDZoMTJ2MTJINnoiLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-tab: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIxIDNIM2MtMS4xIDAtMiAuOS0yIDJ2MTRjMCAxLjEuOSAyIDIgMmgxOGMxLjEgMCAyLS45IDItMlY1YzAtMS4xLS45LTItMi0yem0wIDE2SDNWNWgxMHY0aDh2MTB6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-table-rows: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik0yMSw4SDNWNGgxOFY4eiBNMjEsMTBIM3Y0aDE4VjEweiBNMjEsMTZIM3Y0aDE4VjE2eiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-tag: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjgiIGhlaWdodD0iMjgiIHZpZXdCb3g9IjAgMCA0MyAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTI4LjgzMzIgMTIuMzM0TDMyLjk5OTggMTYuNTAwN0wzNy4xNjY1IDEyLjMzNEgyOC44MzMyWiIvPgoJCTxwYXRoIGQ9Ik0xNi4yMDk1IDIxLjYxMDRDMTUuNjg3MyAyMi4xMjk5IDE0Ljg0NDMgMjIuMTI5OSAxNC4zMjQ4IDIxLjYxMDRMNi45ODI5IDE0LjcyNDVDNi41NzI0IDE0LjMzOTQgNi4wODMxMyAxMy42MDk4IDYuMDQ3ODYgMTMuMDQ4MkM1Ljk1MzQ3IDExLjUyODggNi4wMjAwMiA4LjYxOTQ0IDYuMDY2MjEgNy4wNzY5NUM2LjA4MjgxIDYuNTE0NzcgNi41NTU0OCA2LjA0MzQ3IDcuMTE4MDQgNi4wMzA1NUM5LjA4ODYzIDUuOTg0NzMgMTMuMjYzOCA1LjkzNTc5IDEzLjY1MTggNi4zMjQyNUwyMS43MzY5IDEzLjYzOUMyMi4yNTYgMTQuMTU4NSAyMS43ODUxIDE1LjQ3MjQgMjEuMjYyIDE1Ljk5NDZMMTYuMjA5NSAyMS42MTA0Wk05Ljc3NTg1IDguMjY1QzkuMzM1NTEgNy44MjU2NiA4LjYyMzUxIDcuODI1NjYgOC4xODI4IDguMjY1QzcuNzQzNDYgOC43MDU3MSA3Ljc0MzQ2IDkuNDE3MzMgOC4xODI4IDkuODU2NjdDOC42MjM4MiAxMC4yOTY0IDkuMzM1ODIgMTAuMjk2NCA5Ljc3NTg1IDkuODU2NjdDMTAuMjE1NiA5LjQxNzMzIDEwLjIxNTYgOC43MDUzMyA5Ljc3NTg1IDguMjY1WiIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-terminal: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0IiA+CiAgICA8cmVjdCBjbGFzcz0ianAtdGVybWluYWwtaWNvbi1iYWNrZ3JvdW5kLWNvbG9yIGpwLWljb24tc2VsZWN0YWJsZSIgd2lkdGg9IjIwIiBoZWlnaHQ9IjIwIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSgyIDIpIiBmaWxsPSIjMzMzMzMzIi8+CiAgICA8cGF0aCBjbGFzcz0ianAtdGVybWluYWwtaWNvbi1jb2xvciBqcC1pY29uLXNlbGVjdGFibGUtaW52ZXJzZSIgZD0iTTUuMDU2NjQgOC43NjE3MkM1LjA1NjY0IDguNTk3NjYgNS4wMzEyNSA4LjQ1MzEyIDQuOTgwNDcgOC4zMjgxMkM0LjkzMzU5IDguMTk5MjIgNC44NTU0NyA4LjA4MjAzIDQuNzQ2MDkgNy45NzY1NkM0LjY0MDYyIDcuODcxMDkgNC41IDcuNzc1MzkgNC4zMjQyMiA3LjY4OTQ1QzQuMTUyMzQgNy41OTk2MSAzLjk0MzM2IDcuNTExNzIgMy42OTcyNyA3LjQyNTc4QzMuMzAyNzMgNy4yODUxNiAyLjk0MzM2IDcuMTM2NzIgMi42MTkxNCA2Ljk4MDQ3QzIuMjk0OTIgNi44MjQyMiAyLjAxNzU4IDYuNjQyNTggMS43ODcxMSA2LjQzNTU1QzEuNTYwNTUgNi4yMjg1MiAxLjM4NDc3IDUuOTg4MjggMS4yNTk3NyA1LjcxNDg0QzEuMTM0NzcgNS40Mzc1IDEuMDcyMjcgNS4xMDkzOCAxLjA3MjI3IDQuNzMwNDdDMS4wNzIyNyA0LjM5ODQ0IDEuMTI4OTEgNC4wOTU3IDEuMjQyMTkgMy44MjIyN0MxLjM1NTQ3IDMuNTQ0OTIgMS41MTU2MiAzLjMwNDY5IDEuNzIyNjYgMy4xMDE1NkMxLjkyOTY5IDIuODk4NDQgMi4xNzk2OSAyLjczNDM3IDIuNDcyNjYgMi42MDkzOEMyLjc2NTYyIDIuNDg0MzggMy4wOTE4IDIuNDA0MyAzLjQ1MTE3IDIuMzY5MTRWMS4xMDkzOEg0LjM4ODY3VjIuMzgwODZDNC43NDAyMyAyLjQyNzczIDUuMDU2NjQgMi41MjM0NCA1LjMzNzg5IDIuNjY3OTdDNS42MTkxNCAyLjgxMjUgNS44NTc0MiAzLjAwMTk1IDYuMDUyNzMgMy4yMzYzM0M2LjI1MTk1IDMuNDY2OCA2LjQwNDMgMy43NDAyMyA2LjUwOTc3IDQuMDU2NjRDNi42MTkxNCA0LjM2OTE0IDYuNjczODMgNC43MjA3IDYuNjczODMgNS4xMTEzM0g1LjA0NDkyQzUuMDQ0OTIgNC42Mzg2NyA0LjkzNzUgNC4yODEyNSA0LjcyMjY2IDQuMDM5MDZDNC41MDc4MSAzLjc5Mjk3IDQuMjE2OCAzLjY2OTkyIDMuODQ5NjEgMy42Njk5MkMzLjY1MDM5IDMuNjY5OTIgMy40NzY1NiAzLjY5NzI3IDMuMzI4MTIgMy43NTE5NUMzLjE4MzU5IDMuODAyNzMgMy4wNjQ0NSAzLjg3Njk1IDIuOTcwNyAzLjk3NDYxQzIuODc2OTUgNC4wNjgzNiAyLjgwNjY0IDQuMTc5NjkgMi43NTk3NyA0LjMwODU5QzIuNzE2OCA0LjQzNzUgMi42OTUzMSA0LjU3ODEyIDIuNjk1MzEgNC43MzA0N0MyLjY5NTMxIDQuODgyODEgMi43MTY4IDUuMDE5NTMgMi43NTk3NyA1LjE0MDYyQzIuODA2NjQgNS4yNTc4MSAyLjg4MjgxIDUuMzY3MTkgMi45ODgyOCA1LjQ2ODc1QzMuMDk3NjYgNS41NzAzMSAzLjI0MDIzIDUuNjY3OTcgMy40MTYwMiA1Ljc2MTcyQzMuNTkxOCA1Ljg1MTU2IDMuODEwNTUgNS45NDMzNiA0LjA3MjI3IDYuMDM3MTFDNC40NjY4IDYuMTg1NTUgNC44MjQyMiA2LjMzOTg0IDUuMTQ0NTMgNi41QzUuNDY0ODQgNi42NTYyNSA1LjczODI4IDYuODM5ODQgNS45NjQ4NCA3LjA1MDc4QzYuMTk1MzEgNy4yNTc4MSA2LjM3MTA5IDcuNSA2LjQ5MjE5IDcuNzc3MzRDNi42MTcxOSA4LjA1MDc4IDYuNjc5NjkgOC4zNzUgNi42Nzk2OSA4Ljc1QzYuNjc5NjkgOS4wOTM3NSA2LjYyMzA1IDkuNDA0MyA2LjUwOTc3IDkuNjgxNjRDNi4zOTY0OCA5Ljk1NTA4IDYuMjM0MzggMTAuMTkxNCA2LjAyMzQ0IDEwLjM5MDZDNS44MTI1IDEwLjU4OTggNS41NTg1OSAxMC43NSA1LjI2MTcyIDEwLjg3MTFDNC45NjQ4NCAxMC45ODgzIDQuNjMyODEgMTEuMDY0NSA0LjI2NTYyIDExLjA5OTZWMTIuMjQ4SDMuMzMzOThWMTEuMDk5NkMzLjAwMTk1IDExLjA2ODQgMi42Nzk2OSAxMC45OTYxIDIuMzY3MTkgMTAuODgyOEMyLjA1NDY5IDEwLjc2NTYgMS43NzczNCAxMC41OTc3IDEuNTM1MTYgMTAuMzc4OUMxLjI5Njg4IDEwLjE2MDIgMS4xMDU0NyA5Ljg4NDc3IDAuOTYwOTM4IDkuNTUyNzNDMC44MTY0MDYgOS4yMTY4IDAuNzQ0MTQxIDguODE0NDUgMC43NDQxNDEgOC4zNDU3SDIuMzc4OTFDMi4zNzg5MSA4LjYyNjk1IDIuNDE5OTIgOC44NjMyOCAyLjUwMTk1IDkuMDU0NjlDMi41ODM5OCA5LjI0MjE5IDIuNjg5NDUgOS4zOTI1OCAyLjgxODM2IDkuNTA1ODZDMi45NTExNyA5LjYxNTIzIDMuMTAxNTYgOS42OTMzNiAzLjI2OTUzIDkuNzQwMjNDMy40Mzc1IDkuNzg3MTEgMy42MDkzOCA5LjgxMDU1IDMuNzg1MTYgOS44MTA1NUM0LjIwMzEyIDkuODEwNTUgNC41MTk1MyA5LjcxMjg5IDQuNzM0MzggOS41MTc1OEM0Ljk0OTIyIDkuMzIyMjcgNS4wNTY2NCA5LjA3MDMxIDUuMDU2NjQgOC43NjE3MlpNMTMuNDE4IDEyLjI3MTVIOC4wNzQyMlYxMUgxMy40MThWMTIuMjcxNVoiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDMuOTUyNjQgNikiIGZpbGw9IndoaXRlIi8+Cjwvc3ZnPgo=);
  --jp-icon-text-editor: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtdGV4dC1lZGl0b3ItaWNvbi1jb2xvciBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiIGQ9Ik0xNSAxNUgzdjJoMTJ2LTJ6bTAtOEgzdjJoMTJWN3pNMyAxM2gxOHYtMkgzdjJ6bTAgOGgxOHYtMkgzdjJ6TTMgM3YyaDE4VjNIM3oiLz4KPC9zdmc+Cg==);
  --jp-icon-toc: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik03LDVIMjFWN0g3VjVNNywxM1YxMUgyMVYxM0g3TTQsNC41QTEuNSwxLjUgMCAwLDEgNS41LDZBMS41LDEuNSAwIDAsMSA0LDcuNUExLjUsMS41IDAgMCwxIDIuNSw2QTEuNSwxLjUgMCAwLDEgNCw0LjVNNCwxMC41QTEuNSwxLjUgMCAwLDEgNS41LDEyQTEuNSwxLjUgMCAwLDEgNCwxMy41QTEuNSwxLjUgMCAwLDEgMi41LDEyQTEuNSwxLjUgMCAwLDEgNCwxMC41TTcsMTlWMTdIMjFWMTlIN000LDE2LjVBMS41LDEuNSAwIDAsMSA1LjUsMThBMS41LDEuNSAwIDAsMSA0LDE5LjVBMS41LDEuNSAwIDAsMSAyLjUsMThBMS41LDEuNSAwIDAsMSA0LDE2LjVaIiAvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-tree-view: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik0yMiAxMVYzaC03djNIOVYzSDJ2OGg3VjhoMnYxMGg0djNoN3YtOGgtN3YzaC0yVjhoMnYzeiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-trusted: url(data:image/svg+xml;base64,PHN2ZyBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI1Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDIgMykiIGQ9Ik0xLjg2MDk0IDExLjQ0MDlDMC44MjY0NDggOC43NzAyNyAwLjg2Mzc3OSA2LjA1NzY0IDEuMjQ5MDcgNC4xOTkzMkMyLjQ4MjA2IDMuOTMzNDcgNC4wODA2OCAzLjQwMzQ3IDUuNjAxMDIgMi44NDQ5QzcuMjM1NDkgMi4yNDQ0IDguODU2NjYgMS41ODE1IDkuOTg3NiAxLjA5NTM5QzExLjA1OTcgMS41ODM0MSAxMi42MDk0IDIuMjQ0NCAxNC4yMTggMi44NDMzOUMxNS43NTAzIDMuNDEzOTQgMTcuMzk5NSAzLjk1MjU4IDE4Ljc1MzkgNC4yMTM4NUMxOS4xMzY0IDYuMDcxNzcgMTkuMTcwOSA4Ljc3NzIyIDE4LjEzOSAxMS40NDA5QzE3LjAzMDMgMTQuMzAzMiAxNC42NjY4IDE3LjE4NDQgOS45OTk5OSAxOC45MzU0QzUuMzMzMiAxNy4xODQ0IDIuOTY5NjggMTQuMzAzMiAxLjg2MDk0IDExLjQ0MDlaIi8+CiAgICA8cGF0aCBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiMzMzMzMzMiIHN0cm9rZT0iIzMzMzMzMyIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOCA5Ljg2NzE5KSIgZD0iTTIuODYwMTUgNC44NjUzNUwwLjcyNjU0OSAyLjk5OTU5TDAgMy42MzA0NUwyLjg2MDE1IDYuMTMxNTdMOCAwLjYzMDg3Mkw3LjI3ODU3IDBMMi44NjAxNSA0Ljg2NTM1WiIvPgo8L3N2Zz4K);
  --jp-icon-undo: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyLjUgOGMtMi42NSAwLTUuMDUuOTktNi45IDIuNkwyIDd2OWg5bC0zLjYyLTMuNjJjMS4zOS0xLjE2IDMuMTYtMS44OCA1LjEyLTEuODggMy41NCAwIDYuNTUgMi4zMSA3LjYgNS41bDIuMzctLjc4QzIxLjA4IDExLjAzIDE3LjE1IDggMTIuNSA4eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-user: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTYiIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE2IDdhNCA0IDAgMTEtOCAwIDQgNCAwIDAxOCAwek0xMiAxNGE3IDcgMCAwMC03IDdoMTRhNyA3IDAgMDAtNy03eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-users: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZlcnNpb249IjEuMSIgdmlld0JveD0iMCAwIDM2IDI0IiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgogPGcgY2xhc3M9ImpwLWljb24zIiB0cmFuc2Zvcm09Im1hdHJpeCgxLjczMjcgMCAwIDEuNzMyNyAtMy42MjgyIC4wOTk1NzcpIiBmaWxsPSIjNjE2MTYxIj4KICA8cGF0aCB0cmFuc2Zvcm09Im1hdHJpeCgxLjUsMCwwLDEuNSwwLC02KSIgZD0ibTEyLjE4NiA3LjUwOThjLTEuMDUzNSAwLTEuOTc1NyAwLjU2NjUtMi40Nzg1IDEuNDEwMiAwLjc1MDYxIDAuMzEyNzcgMS4zOTc0IDAuODI2NDggMS44NzMgMS40NzI3aDMuNDg2M2MwLTEuNTkyLTEuMjg4OS0yLjg4MjgtMi44ODA5LTIuODgyOHoiLz4KICA8cGF0aCBkPSJtMjAuNDY1IDIuMzg5NWEyLjE4ODUgMi4xODg1IDAgMCAxLTIuMTg4NCAyLjE4ODUgMi4xODg1IDIuMTg4NSAwIDAgMS0yLjE4ODUtMi4xODg1IDIuMTg4NSAyLjE4ODUgMCAwIDEgMi4xODg1LTIuMTg4NSAyLjE4ODUgMi4xODg1IDAgMCAxIDIuMTg4NCAyLjE4ODV6Ii8+CiAgPHBhdGggdHJhbnNmb3JtPSJtYXRyaXgoMS41LDAsMCwxLjUsMCwtNikiIGQ9Im0zLjU4OTggOC40MjE5Yy0xLjExMjYgMC0yLjAxMzcgMC45MDExMS0yLjAxMzcgMi4wMTM3aDIuODE0NWMwLjI2Nzk3LTAuMzczMDkgMC41OTA3LTAuNzA0MzUgMC45NTg5OC0wLjk3ODUyLTAuMzQ0MzMtMC42MTY4OC0xLjAwMzEtMS4wMzUyLTEuNzU5OC0xLjAzNTJ6Ii8+CiAgPHBhdGggZD0ibTYuOTE1NCA0LjYyM2ExLjUyOTQgMS41Mjk0IDAgMCAxLTEuNTI5NCAxLjUyOTQgMS41Mjk0IDEuNTI5NCAwIDAgMS0xLjUyOTQtMS41Mjk0IDEuNTI5NCAxLjUyOTQgMCAwIDEgMS41Mjk0LTEuNTI5NCAxLjUyOTQgMS41Mjk0IDAgMCAxIDEuNTI5NCAxLjUyOTR6Ii8+CiAgPHBhdGggZD0ibTYuMTM1IDEzLjUzNWMwLTMuMjM5MiAyLjYyNTktNS44NjUgNS44NjUtNS44NjUgMy4yMzkyIDAgNS44NjUgMi42MjU5IDUuODY1IDUuODY1eiIvPgogIDxjaXJjbGUgY3g9IjEyIiBjeT0iMy43Njg1IiByPSIyLjk2ODUiLz4KIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-vega: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbjEganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMjEyMTIxIj4KICAgIDxwYXRoIGQ9Ik0xMC42IDUuNGwyLjItMy4ySDIuMnY3LjNsNC02LjZ6Ii8+CiAgICA8cGF0aCBkPSJNMTUuOCAyLjJsLTQuNCA2LjZMNyA2LjNsLTQuOCA4djUuNWgxNy42VjIuMmgtNHptLTcgMTUuNEg1LjV2LTQuNGgzLjN2NC40em00LjQgMEg5LjhWOS44aDMuNHY3Ljh6bTQuNCAwaC0zLjRWNi41aDMuNHYxMS4xeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-word: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KIDxnIGNsYXNzPSJqcC1pY29uMiIgZmlsbD0iIzQxNDE0MSI+CiAgPHJlY3QgeD0iMiIgeT0iMiIgd2lkdGg9IjE2IiBoZWlnaHQ9IjE2Ii8+CiA8L2c+CiA8ZyBjbGFzcz0ianAtaWNvbi1hY2NlbnQyIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSguNDMgLjA0MDEpIiBmaWxsPSIjZmZmIj4KICA8cGF0aCBkPSJtNC4xNCA4Ljc2cTAuMDY4Mi0xLjg5IDIuNDItMS44OSAxLjE2IDAgMS42OCAwLjQyIDAuNTY3IDAuNDEgMC41NjcgMS4xNnYzLjQ3cTAgMC40NjIgMC41MTQgMC40NjIgMC4xMDMgMCAwLjItMC4wMjMxdjAuNzE0cS0wLjM5OSAwLjEwMy0wLjY1MSAwLjEwMy0wLjQ1MiAwLTAuNjkzLTAuMjItMC4yMzEtMC4yLTAuMjg0LTAuNjYyLTAuOTU2IDAuODcyLTIgMC44NzItMC45MDMgMC0xLjQ3LTAuNDcyLTAuNTI1LTAuNDcyLTAuNTI1LTEuMjYgMC0wLjI2MiAwLjA0NTItMC40NzIgMC4wNTY3LTAuMjIgMC4xMTYtMC4zNzggMC4wNjgyLTAuMTY4IDAuMjMxLTAuMzA0IDAuMTU4LTAuMTQ3IDAuMjYyLTAuMjQyIDAuMTE2LTAuMDkxNCAwLjM2OC0wLjE2OCAwLjI2Mi0wLjA5MTQgMC4zOTktMC4xMjYgMC4xMzYtMC4wNDUyIDAuNDcyLTAuMTAzIDAuMzM2LTAuMDU3OCAwLjUwNC0wLjA3OTggMC4xNTgtMC4wMjMxIDAuNTY3LTAuMDc5OCAwLjU1Ni0wLjA2ODIgMC43NzctMC4yMjEgMC4yMi0wLjE1MiAwLjIyLTAuNDQxdi0wLjI1MnEwLTAuNDMtMC4zNTctMC42NjItMC4zMzYtMC4yMzEtMC45NzYtMC4yMzEtMC42NjIgMC0wLjk5OCAwLjI2Mi0wLjMzNiAwLjI1Mi0wLjM5OSAwLjc5OHptMS44OSAzLjY4cTAuNzg4IDAgMS4yNi0wLjQxIDAuNTA0LTAuNDIgMC41MDQtMC45MDN2LTEuMDVxLTAuMjg0IDAuMTM2LTAuODYxIDAuMjMxLTAuNTY3IDAuMDkxNC0wLjk4NyAwLjE1OC0wLjQyIDAuMDY4Mi0wLjc2NiAwLjMyNi0wLjMzNiAwLjI1Mi0wLjMzNiAwLjcwNHQwLjMwNCAwLjcwNCAwLjg2MSAwLjI1MnoiIHN0cm9rZS13aWR0aD0iMS4wNSIvPgogIDxwYXRoIGQ9Im0xMCA0LjU2aDAuOTQ1djMuMTVxMC42NTEtMC45NzYgMS44OS0wLjk3NiAxLjE2IDAgMS44OSAwLjg0IDAuNjgyIDAuODQgMC42ODIgMi4zMSAwIDEuNDctMC43MDQgMi40Mi0wLjcwNCAwLjg4Mi0xLjg5IDAuODgyLTEuMjYgMC0xLjg5LTEuMDJ2MC43NjZoLTAuODV6bTIuNjIgMy4wNHEtMC43NDYgMC0xLjE2IDAuNjQtMC40NTIgMC42My0wLjQ1MiAxLjY4IDAgMS4wNSAwLjQ1MiAxLjY4dDEuMTYgMC42M3EwLjc3NyAwIDEuMjYtMC42MyAwLjQ5NC0wLjY0IDAuNDk0LTEuNjggMC0xLjA1LTAuNDcyLTEuNjgtMC40NjItMC42NC0xLjI2LTAuNjR6IiBzdHJva2Utd2lkdGg9IjEuMDUiLz4KICA8cGF0aCBkPSJtMi43MyAxNS44IDEzLjYgMC4wMDgxYzAuMDA2OSAwIDAtMi42IDAtMi42IDAtMC4wMDc4LTEuMTUgMC0xLjE1IDAtMC4wMDY5IDAtMC4wMDgzIDEuNS0wLjAwODMgMS41LTJlLTMgLTAuMDAxNC0xMS4zLTAuMDAxNC0xMS4zLTAuMDAxNGwtMC4wMDU5Mi0xLjVjMC0wLjAwNzgtMS4xNyAwLjAwMTMtMS4xNyAwLjAwMTN6IiBzdHJva2Utd2lkdGg9Ii45NzUiLz4KIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-yaml: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi1jb250cmFzdDIganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjRDgxQjYwIj4KICAgIDxwYXRoIGQ9Ik03LjIgMTguNnYtNS40TDMgNS42aDMuM2wxLjQgMy4xYy4zLjkuNiAxLjYgMSAyLjUuMy0uOC42LTEuNiAxLTIuNWwxLjQtMy4xaDMuNGwtNC40IDcuNnY1LjVsLTIuOS0uMXoiLz4KICAgIDxjaXJjbGUgY2xhc3M9InN0MCIgY3g9IjE3LjYiIGN5PSIxNi41IiByPSIyLjEiLz4KICAgIDxjaXJjbGUgY2xhc3M9InN0MCIgY3g9IjE3LjYiIGN5PSIxMSIgcj0iMi4xIi8+CiAgPC9nPgo8L3N2Zz4K);
}

/* Icon CSS class declarations */

.jp-AddAboveIcon {
  background-image: var(--jp-icon-add-above);
}

.jp-AddBelowIcon {
  background-image: var(--jp-icon-add-below);
}

.jp-AddIcon {
  background-image: var(--jp-icon-add);
}

.jp-BellIcon {
  background-image: var(--jp-icon-bell);
}

.jp-BugDotIcon {
  background-image: var(--jp-icon-bug-dot);
}

.jp-BugIcon {
  background-image: var(--jp-icon-bug);
}

.jp-BuildIcon {
  background-image: var(--jp-icon-build);
}

.jp-CaretDownEmptyIcon {
  background-image: var(--jp-icon-caret-down-empty);
}

.jp-CaretDownEmptyThinIcon {
  background-image: var(--jp-icon-caret-down-empty-thin);
}

.jp-CaretDownIcon {
  background-image: var(--jp-icon-caret-down);
}

.jp-CaretLeftIcon {
  background-image: var(--jp-icon-caret-left);
}

.jp-CaretRightIcon {
  background-image: var(--jp-icon-caret-right);
}

.jp-CaretUpEmptyThinIcon {
  background-image: var(--jp-icon-caret-up-empty-thin);
}

.jp-CaretUpIcon {
  background-image: var(--jp-icon-caret-up);
}

.jp-CaseSensitiveIcon {
  background-image: var(--jp-icon-case-sensitive);
}

.jp-CheckIcon {
  background-image: var(--jp-icon-check);
}

.jp-CircleEmptyIcon {
  background-image: var(--jp-icon-circle-empty);
}

.jp-CircleIcon {
  background-image: var(--jp-icon-circle);
}

.jp-ClearIcon {
  background-image: var(--jp-icon-clear);
}

.jp-CloseIcon {
  background-image: var(--jp-icon-close);
}

.jp-CodeCheckIcon {
  background-image: var(--jp-icon-code-check);
}

.jp-CodeIcon {
  background-image: var(--jp-icon-code);
}

.jp-CollapseAllIcon {
  background-image: var(--jp-icon-collapse-all);
}

.jp-ConsoleIcon {
  background-image: var(--jp-icon-console);
}

.jp-CopyIcon {
  background-image: var(--jp-icon-copy);
}

.jp-CopyrightIcon {
  background-image: var(--jp-icon-copyright);
}

.jp-CutIcon {
  background-image: var(--jp-icon-cut);
}

.jp-DeleteIcon {
  background-image: var(--jp-icon-delete);
}

.jp-DownloadIcon {
  background-image: var(--jp-icon-download);
}

.jp-DuplicateIcon {
  background-image: var(--jp-icon-duplicate);
}

.jp-EditIcon {
  background-image: var(--jp-icon-edit);
}

.jp-EllipsesIcon {
  background-image: var(--jp-icon-ellipses);
}

.jp-ErrorIcon {
  background-image: var(--jp-icon-error);
}

.jp-ExpandAllIcon {
  background-image: var(--jp-icon-expand-all);
}

.jp-ExtensionIcon {
  background-image: var(--jp-icon-extension);
}

.jp-FastForwardIcon {
  background-image: var(--jp-icon-fast-forward);
}

.jp-FileIcon {
  background-image: var(--jp-icon-file);
}

.jp-FileUploadIcon {
  background-image: var(--jp-icon-file-upload);
}

.jp-FilterDotIcon {
  background-image: var(--jp-icon-filter-dot);
}

.jp-FilterIcon {
  background-image: var(--jp-icon-filter);
}

.jp-FilterListIcon {
  background-image: var(--jp-icon-filter-list);
}

.jp-FolderFavoriteIcon {
  background-image: var(--jp-icon-folder-favorite);
}

.jp-FolderIcon {
  background-image: var(--jp-icon-folder);
}

.jp-HomeIcon {
  background-image: var(--jp-icon-home);
}

.jp-Html5Icon {
  background-image: var(--jp-icon-html5);
}

.jp-ImageIcon {
  background-image: var(--jp-icon-image);
}

.jp-InfoIcon {
  background-image: var(--jp-icon-info);
}

.jp-InspectorIcon {
  background-image: var(--jp-icon-inspector);
}

.jp-JsonIcon {
  background-image: var(--jp-icon-json);
}

.jp-JuliaIcon {
  background-image: var(--jp-icon-julia);
}

.jp-JupyterFaviconIcon {
  background-image: var(--jp-icon-jupyter-favicon);
}

.jp-JupyterIcon {
  background-image: var(--jp-icon-jupyter);
}

.jp-JupyterlabWordmarkIcon {
  background-image: var(--jp-icon-jupyterlab-wordmark);
}

.jp-KernelIcon {
  background-image: var(--jp-icon-kernel);
}

.jp-KeyboardIcon {
  background-image: var(--jp-icon-keyboard);
}

.jp-LaunchIcon {
  background-image: var(--jp-icon-launch);
}

.jp-LauncherIcon {
  background-image: var(--jp-icon-launcher);
}

.jp-LineFormIcon {
  background-image: var(--jp-icon-line-form);
}

.jp-LinkIcon {
  background-image: var(--jp-icon-link);
}

.jp-ListIcon {
  background-image: var(--jp-icon-list);
}

.jp-MarkdownIcon {
  background-image: var(--jp-icon-markdown);
}

.jp-MoveDownIcon {
  background-image: var(--jp-icon-move-down);
}

.jp-MoveUpIcon {
  background-image: var(--jp-icon-move-up);
}

.jp-NewFolderIcon {
  background-image: var(--jp-icon-new-folder);
}

.jp-NotTrustedIcon {
  background-image: var(--jp-icon-not-trusted);
}

.jp-NotebookIcon {
  background-image: var(--jp-icon-notebook);
}

.jp-NumberingIcon {
  background-image: var(--jp-icon-numbering);
}

.jp-OfflineBoltIcon {
  background-image: var(--jp-icon-offline-bolt);
}

.jp-PaletteIcon {
  background-image: var(--jp-icon-palette);
}

.jp-PasteIcon {
  background-image: var(--jp-icon-paste);
}

.jp-PdfIcon {
  background-image: var(--jp-icon-pdf);
}

.jp-PythonIcon {
  background-image: var(--jp-icon-python);
}

.jp-RKernelIcon {
  background-image: var(--jp-icon-r-kernel);
}

.jp-ReactIcon {
  background-image: var(--jp-icon-react);
}

.jp-RedoIcon {
  background-image: var(--jp-icon-redo);
}

.jp-RefreshIcon {
  background-image: var(--jp-icon-refresh);
}

.jp-RegexIcon {
  background-image: var(--jp-icon-regex);
}

.jp-RunIcon {
  background-image: var(--jp-icon-run);
}

.jp-RunningIcon {
  background-image: var(--jp-icon-running);
}

.jp-SaveIcon {
  background-image: var(--jp-icon-save);
}

.jp-SearchIcon {
  background-image: var(--jp-icon-search);
}

.jp-SettingsIcon {
  background-image: var(--jp-icon-settings);
}

.jp-ShareIcon {
  background-image: var(--jp-icon-share);
}

.jp-SpreadsheetIcon {
  background-image: var(--jp-icon-spreadsheet);
}

.jp-StopIcon {
  background-image: var(--jp-icon-stop);
}

.jp-TabIcon {
  background-image: var(--jp-icon-tab);
}

.jp-TableRowsIcon {
  background-image: var(--jp-icon-table-rows);
}

.jp-TagIcon {
  background-image: var(--jp-icon-tag);
}

.jp-TerminalIcon {
  background-image: var(--jp-icon-terminal);
}

.jp-TextEditorIcon {
  background-image: var(--jp-icon-text-editor);
}

.jp-TocIcon {
  background-image: var(--jp-icon-toc);
}

.jp-TreeViewIcon {
  background-image: var(--jp-icon-tree-view);
}

.jp-TrustedIcon {
  background-image: var(--jp-icon-trusted);
}

.jp-UndoIcon {
  background-image: var(--jp-icon-undo);
}

.jp-UserIcon {
  background-image: var(--jp-icon-user);
}

.jp-UsersIcon {
  background-image: var(--jp-icon-users);
}

.jp-VegaIcon {
  background-image: var(--jp-icon-vega);
}

.jp-WordIcon {
  background-image: var(--jp-icon-word);
}

.jp-YamlIcon {
  background-image: var(--jp-icon-yaml);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/**
 * (DEPRECATED) Support for consuming icons as CSS background images
 */

.jp-Icon,
.jp-MaterialIcon {
  background-position: center;
  background-repeat: no-repeat;
  background-size: 16px;
  min-width: 16px;
  min-height: 16px;
}

.jp-Icon-cover {
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}

/**
 * (DEPRECATED) Support for specific CSS icon sizes
 */

.jp-Icon-16 {
  background-size: 16px;
  min-width: 16px;
  min-height: 16px;
}

.jp-Icon-18 {
  background-size: 18px;
  min-width: 18px;
  min-height: 18px;
}

.jp-Icon-20 {
  background-size: 20px;
  min-width: 20px;
  min-height: 20px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.lm-TabBar .lm-TabBar-addButton {
  align-items: center;
  display: flex;
  padding: 4px;
  padding-bottom: 5px;
  margin-right: 1px;
  background-color: var(--jp-layout-color2);
}

.lm-TabBar .lm-TabBar-addButton:hover {
  background-color: var(--jp-layout-color1);
}

.lm-DockPanel-tabBar .lm-TabBar-tab {
  width: var(--jp-private-horizontal-tab-width);
}

.lm-DockPanel-tabBar .lm-TabBar-content {
  flex: unset;
}

.lm-DockPanel-tabBar[data-orientation='horizontal'] {
  flex: 1 1 auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/**
 * Support for icons as inline SVG HTMLElements
 */

/* recolor the primary elements of an icon */
.jp-icon0[fill] {
  fill: var(--jp-inverse-layout-color0);
}

.jp-icon1[fill] {
  fill: var(--jp-inverse-layout-color1);
}

.jp-icon2[fill] {
  fill: var(--jp-inverse-layout-color2);
}

.jp-icon3[fill] {
  fill: var(--jp-inverse-layout-color3);
}

.jp-icon4[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon0[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}

.jp-icon1[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}

.jp-icon2[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}

.jp-icon3[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}

.jp-icon4[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}

/* recolor the accent elements of an icon */
.jp-icon-accent0[fill] {
  fill: var(--jp-layout-color0);
}

.jp-icon-accent1[fill] {
  fill: var(--jp-layout-color1);
}

.jp-icon-accent2[fill] {
  fill: var(--jp-layout-color2);
}

.jp-icon-accent3[fill] {
  fill: var(--jp-layout-color3);
}

.jp-icon-accent4[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-accent0[stroke] {
  stroke: var(--jp-layout-color0);
}

.jp-icon-accent1[stroke] {
  stroke: var(--jp-layout-color1);
}

.jp-icon-accent2[stroke] {
  stroke: var(--jp-layout-color2);
}

.jp-icon-accent3[stroke] {
  stroke: var(--jp-layout-color3);
}

.jp-icon-accent4[stroke] {
  stroke: var(--jp-layout-color4);
}

/* set the color of an icon to transparent */
.jp-icon-none[fill] {
  fill: none;
}

.jp-icon-none[stroke] {
  stroke: none;
}

/* brand icon colors. Same for light and dark */
.jp-icon-brand0[fill] {
  fill: var(--jp-brand-color0);
}

.jp-icon-brand1[fill] {
  fill: var(--jp-brand-color1);
}

.jp-icon-brand2[fill] {
  fill: var(--jp-brand-color2);
}

.jp-icon-brand3[fill] {
  fill: var(--jp-brand-color3);
}

.jp-icon-brand4[fill] {
  fill: var(--jp-brand-color4);
}

.jp-icon-brand0[stroke] {
  stroke: var(--jp-brand-color0);
}

.jp-icon-brand1[stroke] {
  stroke: var(--jp-brand-color1);
}

.jp-icon-brand2[stroke] {
  stroke: var(--jp-brand-color2);
}

.jp-icon-brand3[stroke] {
  stroke: var(--jp-brand-color3);
}

.jp-icon-brand4[stroke] {
  stroke: var(--jp-brand-color4);
}

/* warn icon colors. Same for light and dark */
.jp-icon-warn0[fill] {
  fill: var(--jp-warn-color0);
}

.jp-icon-warn1[fill] {
  fill: var(--jp-warn-color1);
}

.jp-icon-warn2[fill] {
  fill: var(--jp-warn-color2);
}

.jp-icon-warn3[fill] {
  fill: var(--jp-warn-color3);
}

.jp-icon-warn0[stroke] {
  stroke: var(--jp-warn-color0);
}

.jp-icon-warn1[stroke] {
  stroke: var(--jp-warn-color1);
}

.jp-icon-warn2[stroke] {
  stroke: var(--jp-warn-color2);
}

.jp-icon-warn3[stroke] {
  stroke: var(--jp-warn-color3);
}

/* icon colors that contrast well with each other and most backgrounds */
.jp-icon-contrast0[fill] {
  fill: var(--jp-icon-contrast-color0);
}

.jp-icon-contrast1[fill] {
  fill: var(--jp-icon-contrast-color1);
}

.jp-icon-contrast2[fill] {
  fill: var(--jp-icon-contrast-color2);
}

.jp-icon-contrast3[fill] {
  fill: var(--jp-icon-contrast-color3);
}

.jp-icon-contrast0[stroke] {
  stroke: var(--jp-icon-contrast-color0);
}

.jp-icon-contrast1[stroke] {
  stroke: var(--jp-icon-contrast-color1);
}

.jp-icon-contrast2[stroke] {
  stroke: var(--jp-icon-contrast-color2);
}

.jp-icon-contrast3[stroke] {
  stroke: var(--jp-icon-contrast-color3);
}

.jp-icon-dot[fill] {
  fill: var(--jp-warn-color0);
}

.jp-jupyter-icon-color[fill] {
  fill: var(--jp-jupyter-icon-color, var(--jp-warn-color0));
}

.jp-notebook-icon-color[fill] {
  fill: var(--jp-notebook-icon-color, var(--jp-warn-color0));
}

.jp-json-icon-color[fill] {
  fill: var(--jp-json-icon-color, var(--jp-warn-color1));
}

.jp-console-icon-color[fill] {
  fill: var(--jp-console-icon-color, white);
}

.jp-console-icon-background-color[fill] {
  fill: var(--jp-console-icon-background-color, var(--jp-brand-color1));
}

.jp-terminal-icon-color[fill] {
  fill: var(--jp-terminal-icon-color, var(--jp-layout-color2));
}

.jp-terminal-icon-background-color[fill] {
  fill: var(
    --jp-terminal-icon-background-color,
    var(--jp-inverse-layout-color2)
  );
}

.jp-text-editor-icon-color[fill] {
  fill: var(--jp-text-editor-icon-color, var(--jp-inverse-layout-color3));
}

.jp-inspector-icon-color[fill] {
  fill: var(--jp-inspector-icon-color, var(--jp-inverse-layout-color3));
}

/* CSS for icons in selected filebrowser listing items */
.jp-DirListing-item.jp-mod-selected .jp-icon-selectable[fill] {
  fill: #fff;
}

.jp-DirListing-item.jp-mod-selected .jp-icon-selectable-inverse[fill] {
  fill: var(--jp-brand-color1);
}

/* stylelint-disable selector-max-class, selector-max-compound-selectors */

/**
* TODO: come up with non css-hack solution for showing the busy icon on top
*  of the close icon
* CSS for complex behavior of close icon of tabs in the main area tabbar
*/
.lm-DockPanel-tabBar
  .lm-TabBar-tab.lm-mod-closable.jp-mod-dirty
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon3[fill] {
  fill: none;
}

.lm-DockPanel-tabBar
  .lm-TabBar-tab.lm-mod-closable.jp-mod-dirty
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon-busy[fill] {
  fill: var(--jp-inverse-layout-color3);
}

/* stylelint-enable selector-max-class, selector-max-compound-selectors */

/* CSS for icons in status bar */
#jp-main-statusbar .jp-mod-selected .jp-icon-selectable[fill] {
  fill: #fff;
}

#jp-main-statusbar .jp-mod-selected .jp-icon-selectable-inverse[fill] {
  fill: var(--jp-brand-color1);
}

/* special handling for splash icon CSS. While the theme CSS reloads during
   splash, the splash icon can loose theming. To prevent that, we set a
   default for its color variable */
:root {
  --jp-warn-color0: var(--md-orange-700);
}

/* not sure what to do with this one, used in filebrowser listing */
.jp-DragIcon {
  margin-right: 4px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/**
 * Support for alt colors for icons as inline SVG HTMLElements
 */

/* alt recolor the primary elements of an icon */
.jp-icon-alt .jp-icon0[fill] {
  fill: var(--jp-layout-color0);
}

.jp-icon-alt .jp-icon1[fill] {
  fill: var(--jp-layout-color1);
}

.jp-icon-alt .jp-icon2[fill] {
  fill: var(--jp-layout-color2);
}

.jp-icon-alt .jp-icon3[fill] {
  fill: var(--jp-layout-color3);
}

.jp-icon-alt .jp-icon4[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-alt .jp-icon0[stroke] {
  stroke: var(--jp-layout-color0);
}

.jp-icon-alt .jp-icon1[stroke] {
  stroke: var(--jp-layout-color1);
}

.jp-icon-alt .jp-icon2[stroke] {
  stroke: var(--jp-layout-color2);
}

.jp-icon-alt .jp-icon3[stroke] {
  stroke: var(--jp-layout-color3);
}

.jp-icon-alt .jp-icon4[stroke] {
  stroke: var(--jp-layout-color4);
}

/* alt recolor the accent elements of an icon */
.jp-icon-alt .jp-icon-accent0[fill] {
  fill: var(--jp-inverse-layout-color0);
}

.jp-icon-alt .jp-icon-accent1[fill] {
  fill: var(--jp-inverse-layout-color1);
}

.jp-icon-alt .jp-icon-accent2[fill] {
  fill: var(--jp-inverse-layout-color2);
}

.jp-icon-alt .jp-icon-accent3[fill] {
  fill: var(--jp-inverse-layout-color3);
}

.jp-icon-alt .jp-icon-accent4[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon-alt .jp-icon-accent0[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}

.jp-icon-alt .jp-icon-accent1[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}

.jp-icon-alt .jp-icon-accent2[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}

.jp-icon-alt .jp-icon-accent3[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}

.jp-icon-alt .jp-icon-accent4[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-icon-hoverShow:not(:hover) .jp-icon-hoverShow-content {
  display: none !important;
}

/**
 * Support for hover colors for icons as inline SVG HTMLElements
 */

/**
 * regular colors
 */

/* recolor the primary elements of an icon */
.jp-icon-hover :hover .jp-icon0-hover[fill] {
  fill: var(--jp-inverse-layout-color0);
}

.jp-icon-hover :hover .jp-icon1-hover[fill] {
  fill: var(--jp-inverse-layout-color1);
}

.jp-icon-hover :hover .jp-icon2-hover[fill] {
  fill: var(--jp-inverse-layout-color2);
}

.jp-icon-hover :hover .jp-icon3-hover[fill] {
  fill: var(--jp-inverse-layout-color3);
}

.jp-icon-hover :hover .jp-icon4-hover[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon-hover :hover .jp-icon0-hover[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}

.jp-icon-hover :hover .jp-icon1-hover[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}

.jp-icon-hover :hover .jp-icon2-hover[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}

.jp-icon-hover :hover .jp-icon3-hover[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}

.jp-icon-hover :hover .jp-icon4-hover[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}

/* recolor the accent elements of an icon */
.jp-icon-hover :hover .jp-icon-accent0-hover[fill] {
  fill: var(--jp-layout-color0);
}

.jp-icon-hover :hover .jp-icon-accent1-hover[fill] {
  fill: var(--jp-layout-color1);
}

.jp-icon-hover :hover .jp-icon-accent2-hover[fill] {
  fill: var(--jp-layout-color2);
}

.jp-icon-hover :hover .jp-icon-accent3-hover[fill] {
  fill: var(--jp-layout-color3);
}

.jp-icon-hover :hover .jp-icon-accent4-hover[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-hover :hover .jp-icon-accent0-hover[stroke] {
  stroke: var(--jp-layout-color0);
}

.jp-icon-hover :hover .jp-icon-accent1-hover[stroke] {
  stroke: var(--jp-layout-color1);
}

.jp-icon-hover :hover .jp-icon-accent2-hover[stroke] {
  stroke: var(--jp-layout-color2);
}

.jp-icon-hover :hover .jp-icon-accent3-hover[stroke] {
  stroke: var(--jp-layout-color3);
}

.jp-icon-hover :hover .jp-icon-accent4-hover[stroke] {
  stroke: var(--jp-layout-color4);
}

/* set the color of an icon to transparent */
.jp-icon-hover :hover .jp-icon-none-hover[fill] {
  fill: none;
}

.jp-icon-hover :hover .jp-icon-none-hover[stroke] {
  stroke: none;
}

/**
 * inverse colors
 */

/* inverse recolor the primary elements of an icon */
.jp-icon-hover.jp-icon-alt :hover .jp-icon0-hover[fill] {
  fill: var(--jp-layout-color0);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon1-hover[fill] {
  fill: var(--jp-layout-color1);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon2-hover[fill] {
  fill: var(--jp-layout-color2);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon3-hover[fill] {
  fill: var(--jp-layout-color3);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon4-hover[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon0-hover[stroke] {
  stroke: var(--jp-layout-color0);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon1-hover[stroke] {
  stroke: var(--jp-layout-color1);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon2-hover[stroke] {
  stroke: var(--jp-layout-color2);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon3-hover[stroke] {
  stroke: var(--jp-layout-color3);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon4-hover[stroke] {
  stroke: var(--jp-layout-color4);
}

/* inverse recolor the accent elements of an icon */
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent0-hover[fill] {
  fill: var(--jp-inverse-layout-color0);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent1-hover[fill] {
  fill: var(--jp-inverse-layout-color1);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent2-hover[fill] {
  fill: var(--jp-inverse-layout-color2);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent3-hover[fill] {
  fill: var(--jp-inverse-layout-color3);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent4-hover[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent0-hover[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent1-hover[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent2-hover[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent3-hover[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent4-hover[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-IFrame {
  width: 100%;
  height: 100%;
}

.jp-IFrame > iframe {
  border: none;
}

/*
When drag events occur, `lm-mod-override-cursor` is added to the body.
Because iframes steal all cursor events, the following two rules are necessary
to suppress pointer events while resize drags are occurring. There may be a
better solution to this problem.
*/
body.lm-mod-override-cursor .jp-IFrame {
  position: relative;
}

body.lm-mod-override-cursor .jp-IFrame::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: transparent;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-HoverBox {
  position: fixed;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-FormGroup-content fieldset {
  border: none;
  padding: 0;
  min-width: 0;
  width: 100%;
}

/* stylelint-disable selector-max-type */

.jp-FormGroup-content fieldset .jp-inputFieldWrapper input,
.jp-FormGroup-content fieldset .jp-inputFieldWrapper select,
.jp-FormGroup-content fieldset .jp-inputFieldWrapper textarea {
  font-size: var(--jp-content-font-size2);
  border-color: var(--jp-input-border-color);
  border-style: solid;
  border-radius: var(--jp-border-radius);
  border-width: 1px;
  padding: 6px 8px;
  background: none;
  color: var(--jp-ui-font-color0);
  height: inherit;
}

.jp-FormGroup-content fieldset input[type='checkbox'] {
  position: relative;
  top: 2px;
  margin-left: 0;
}

.jp-FormGroup-content button.jp-mod-styled {
  cursor: pointer;
}

.jp-FormGroup-content .checkbox label {
  cursor: pointer;
  font-size: var(--jp-content-font-size1);
}

.jp-FormGroup-content .jp-root > fieldset > legend {
  display: none;
}

.jp-FormGroup-content .jp-root > fieldset > p {
  display: none;
}

/** copy of `input.jp-mod-styled:focus` style */
.jp-FormGroup-content fieldset input:focus,
.jp-FormGroup-content fieldset select:focus {
  -moz-outline-radius: unset;
  outline: var(--jp-border-width) solid var(--md-blue-500);
  outline-offset: -1px;
  box-shadow: inset 0 0 4px var(--md-blue-300);
}

.jp-FormGroup-content fieldset input:hover:not(:focus),
.jp-FormGroup-content fieldset select:hover:not(:focus) {
  background-color: var(--jp-border-color2);
}

/* stylelint-enable selector-max-type */

.jp-FormGroup-content .checkbox .field-description {
  /* Disable default description field for checkbox:
   because other widgets do not have description fields,
   we add descriptions to each widget on the field level.
  */
  display: none;
}

.jp-FormGroup-content #root__description {
  display: none;
}

.jp-FormGroup-content .jp-modifiedIndicator {
  width: 5px;
  background-color: var(--jp-brand-color2);
  margin-top: 0;
  margin-left: calc(var(--jp-private-settingeditor-modifier-indent) * -1);
  flex-shrink: 0;
}

.jp-FormGroup-content .jp-modifiedIndicator.jp-errorIndicator {
  background-color: var(--jp-error-color0);
  margin-right: 0.5em;
}

/* RJSF ARRAY style */

.jp-arrayFieldWrapper legend {
  font-size: var(--jp-content-font-size2);
  color: var(--jp-ui-font-color0);
  flex-basis: 100%;
  padding: 4px 0;
  font-weight: var(--jp-content-heading-font-weight);
  border-bottom: 1px solid var(--jp-border-color2);
}

.jp-arrayFieldWrapper .field-description {
  padding: 4px 0;
  white-space: pre-wrap;
}

.jp-arrayFieldWrapper .array-item {
  width: 100%;
  border: 1px solid var(--jp-border-color2);
  border-radius: 4px;
  margin: 4px;
}

.jp-ArrayOperations {
  display: flex;
  margin-left: 8px;
}

.jp-ArrayOperationsButton {
  margin: 2px;
}

.jp-ArrayOperationsButton .jp-icon3[fill] {
  fill: var(--jp-ui-font-color0);
}

button.jp-ArrayOperationsButton.jp-mod-styled:disabled {
  cursor: not-allowed;
  opacity: 0.5;
}

/* RJSF form validation error */

.jp-FormGroup-content .validationErrors {
  color: var(--jp-error-color0);
}

/* Hide panel level error as duplicated the field level error */
.jp-FormGroup-content .panel.errors {
  display: none;
}

/* RJSF normal content (settings-editor) */

.jp-FormGroup-contentNormal {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}

.jp-FormGroup-contentNormal .jp-FormGroup-contentItem {
  margin-left: 7px;
  color: var(--jp-ui-font-color0);
}

.jp-FormGroup-contentNormal .jp-FormGroup-description {
  flex-basis: 100%;
  padding: 4px 7px;
}

.jp-FormGroup-contentNormal .jp-FormGroup-default {
  flex-basis: 100%;
  padding: 4px 7px;
}

.jp-FormGroup-contentNormal .jp-FormGroup-fieldLabel {
  font-size: var(--jp-content-font-size1);
  font-weight: normal;
  min-width: 120px;
}

.jp-FormGroup-contentNormal fieldset:not(:first-child) {
  margin-left: 7px;
}

.jp-FormGroup-contentNormal .field-array-of-string .array-item {
  /* Display `jp-ArrayOperations` buttons side-by-side with content except
    for small screens where flex-wrap will place them one below the other.
  */
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}

.jp-FormGroup-contentNormal .jp-objectFieldWrapper .form-group {
  padding: 2px 8px 2px var(--jp-private-settingeditor-modifier-indent);
  margin-top: 2px;
}

/* RJSF compact content (metadata-form) */

.jp-FormGroup-content.jp-FormGroup-contentCompact {
  width: 100%;
}

.jp-FormGroup-contentCompact .form-group {
  display: flex;
  padding: 0.5em 0.2em 0.5em 0;
}

.jp-FormGroup-contentCompact
  .jp-FormGroup-compactTitle
  .jp-FormGroup-description {
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color2);
}

.jp-FormGroup-contentCompact .jp-FormGroup-fieldLabel {
  padding-bottom: 0.3em;
}

.jp-FormGroup-contentCompact .jp-inputFieldWrapper .form-control {
  width: 100%;
  box-sizing: border-box;
}

.jp-FormGroup-contentCompact .jp-arrayFieldWrapper .jp-FormGroup-compactTitle {
  padding-bottom: 7px;
}

.jp-FormGroup-contentCompact
  .jp-objectFieldWrapper
  .jp-objectFieldWrapper
  .form-group {
  padding: 2px 8px 2px var(--jp-private-settingeditor-modifier-indent);
  margin-top: 2px;
}

.jp-FormGroup-contentCompact ul.error-detail {
  margin-block-start: 0.5em;
  margin-block-end: 0.5em;
  padding-inline-start: 1em;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-SidePanel {
  display: flex;
  flex-direction: column;
  min-width: var(--jp-sidebar-min-width);
  overflow-y: auto;
  color: var(--jp-ui-font-color1);
  background: var(--jp-layout-color1);
  font-size: var(--jp-ui-font-size1);
}

.jp-SidePanel-header {
  flex: 0 0 auto;
  display: flex;
  border-bottom: var(--jp-border-width) solid var(--jp-border-color2);
  font-size: var(--jp-ui-font-size0);
  font-weight: 600;
  letter-spacing: 1px;
  margin: 0;
  padding: 2px;
  text-transform: uppercase;
}

.jp-SidePanel-toolbar {
  flex: 0 0 auto;
}

.jp-SidePanel-content {
  flex: 1 1 auto;
}

.jp-SidePanel-toolbar,
.jp-AccordionPanel-toolbar {
  height: var(--jp-private-toolbar-height);
}

.jp-SidePanel-toolbar.jp-Toolbar-micro {
  display: none;
}

.lm-AccordionPanel .jp-AccordionPanel-title {
  box-sizing: border-box;
  line-height: 25px;
  margin: 0;
  display: flex;
  align-items: center;
  background: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  box-shadow: var(--jp-toolbar-box-shadow);
  font-size: var(--jp-ui-font-size0);
}

.jp-AccordionPanel-title {
  cursor: pointer;
  user-select: none;
  -moz-user-select: none;
  -webkit-user-select: none;
  text-transform: uppercase;
}

.lm-AccordionPanel[data-orientation='horizontal'] > .jp-AccordionPanel-title {
  /* Title is rotated for horizontal accordion panel using CSS */
  display: block;
  transform-origin: top left;
  transform: rotate(-90deg) translate(-100%);
}

.jp-AccordionPanel-title .lm-AccordionPanel-titleLabel {
  user-select: none;
  text-overflow: ellipsis;
  white-space: nowrap;
  overflow: hidden;
}

.jp-AccordionPanel-title .lm-AccordionPanel-titleCollapser {
  transform: rotate(-90deg);
  margin: auto 0;
  height: 16px;
}

.jp-AccordionPanel-title.lm-mod-expanded .lm-AccordionPanel-titleCollapser {
  transform: rotate(0deg);
}

.lm-AccordionPanel .jp-AccordionPanel-toolbar {
  background: none;
  box-shadow: none;
  border: none;
  margin-left: auto;
}

.lm-AccordionPanel .lm-SplitPanel-handle:hover {
  background: var(--jp-layout-color3);
}

.jp-text-truncated {
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Spinner {
  position: absolute;
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 10;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background: var(--jp-layout-color0);
  outline: none;
}

.jp-SpinnerContent {
  font-size: 10px;
  margin: 50px auto;
  text-indent: -9999em;
  width: 3em;
  height: 3em;
  border-radius: 50%;
  background: var(--jp-brand-color3);
  background: linear-gradient(
    to right,
    #f37626 10%,
    rgba(255, 255, 255, 0) 42%
  );
  position: relative;
  animation: load3 1s infinite linear, fadeIn 1s;
}

.jp-SpinnerContent::before {
  width: 50%;
  height: 50%;
  background: #f37626;
  border-radius: 100% 0 0;
  position: absolute;
  top: 0;
  left: 0;
  content: '';
}

.jp-SpinnerContent::after {
  background: var(--jp-layout-color0);
  width: 75%;
  height: 75%;
  border-radius: 50%;
  content: '';
  margin: auto;
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
}

@keyframes fadeIn {
  0% {
    opacity: 0;
  }

  100% {
    opacity: 1;
  }
}

@keyframes load3 {
  0% {
    transform: rotate(0deg);
  }

  100% {
    transform: rotate(360deg);
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

button.jp-mod-styled {
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color0);
  border: none;
  box-sizing: border-box;
  text-align: center;
  line-height: 32px;
  height: 32px;
  padding: 0 12px;
  letter-spacing: 0.8px;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
}

input.jp-mod-styled {
  background: var(--jp-input-background);
  height: 28px;
  box-sizing: border-box;
  border: var(--jp-border-width) solid var(--jp-border-color1);
  padding-left: 7px;
  padding-right: 7px;
  font-size: var(--jp-ui-font-size2);
  color: var(--jp-ui-font-color0);
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
}

input[type='checkbox'].jp-mod-styled {
  appearance: checkbox;
  -webkit-appearance: checkbox;
  -moz-appearance: checkbox;
  height: auto;
}

input.jp-mod-styled:focus {
  border: var(--jp-border-width) solid var(--md-blue-500);
  box-shadow: inset 0 0 4px var(--md-blue-300);
}

.jp-select-wrapper {
  display: flex;
  position: relative;
  flex-direction: column;
  padding: 1px;
  background-color: var(--jp-layout-color1);
  box-sizing: border-box;
  margin-bottom: 12px;
}

.jp-select-wrapper:not(.multiple) {
  height: 28px;
}

.jp-select-wrapper.jp-mod-focused select.jp-mod-styled {
  border: var(--jp-border-width) solid var(--jp-input-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
  background-color: var(--jp-input-active-background);
}

select.jp-mod-styled:hover {
  cursor: pointer;
  color: var(--jp-ui-font-color0);
  background-color: var(--jp-input-hover-background);
  box-shadow: inset 0 0 1px rgba(0, 0, 0, 0.5);
}

select.jp-mod-styled {
  flex: 1 1 auto;
  width: 100%;
  font-size: var(--jp-ui-font-size2);
  background: var(--jp-input-background);
  color: var(--jp-ui-font-color0);
  padding: 0 25px 0 8px;
  border: var(--jp-border-width) solid var(--jp-input-border-color);
  border-radius: 0;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
}

select.jp-mod-styled:not([multiple]) {
  height: 32px;
}

select.jp-mod-styled[multiple] {
  max-height: 200px;
  overflow-y: auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-switch {
  display: flex;
  align-items: center;
  padding-left: 4px;
  padding-right: 4px;
  font-size: var(--jp-ui-font-size1);
  background-color: transparent;
  color: var(--jp-ui-font-color1);
  border: none;
  height: 20px;
}

.jp-switch:hover {
  background-color: var(--jp-layout-color2);
}

.jp-switch-label {
  margin-right: 5px;
  font-family: var(--jp-ui-font-family);
}

.jp-switch-track {
  cursor: pointer;
  background-color: var(--jp-switch-color, var(--jp-border-color1));
  -webkit-transition: 0.4s;
  transition: 0.4s;
  border-radius: 34px;
  height: 16px;
  width: 35px;
  position: relative;
}

.jp-switch-track::before {
  content: '';
  position: absolute;
  height: 10px;
  width: 10px;
  margin: 3px;
  left: 0;
  background-color: var(--jp-ui-inverse-font-color1);
  -webkit-transition: 0.4s;
  transition: 0.4s;
  border-radius: 50%;
}

.jp-switch[aria-checked='true'] .jp-switch-track {
  background-color: var(--jp-switch-true-position-color, var(--jp-warn-color0));
}

.jp-switch[aria-checked='true'] .jp-switch-track::before {
  /* track width (35) - margins (3 + 3) - thumb width (10) */
  left: 19px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

:root {
  --jp-private-toolbar-height: calc(
    28px + var(--jp-border-width)
  ); /* leave 28px for content */
}

.jp-Toolbar {
  color: var(--jp-ui-font-color1);
  flex: 0 0 auto;
  display: flex;
  flex-direction: row;
  border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  box-shadow: var(--jp-toolbar-box-shadow);
  background: var(--jp-toolbar-background);
  min-height: var(--jp-toolbar-micro-height);
  padding: 2px;
  z-index: 8;
  overflow-x: hidden;
}

/* Toolbar items */

.jp-Toolbar > .jp-Toolbar-item.jp-Toolbar-spacer {
  flex-grow: 1;
  flex-shrink: 1;
}

.jp-Toolbar-item.jp-Toolbar-kernelStatus {
  display: inline-block;
  width: 32px;
  background-repeat: no-repeat;
  background-position: center;
  background-size: 16px;
}

.jp-Toolbar > .jp-Toolbar-item {
  flex: 0 0 auto;
  display: flex;
  padding-left: 1px;
  padding-right: 1px;
  font-size: var(--jp-ui-font-size1);
  line-height: var(--jp-private-toolbar-height);
  height: 100%;
}

/* Toolbar buttons */

/* This is the div we use to wrap the react component into a Widget */
div.jp-ToolbarButton {
  color: transparent;
  border: none;
  box-sizing: border-box;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
  padding: 0;
  margin: 0;
}

button.jp-ToolbarButtonComponent {
  background: var(--jp-layout-color1);
  border: none;
  box-sizing: border-box;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
  padding: 0 6px;
  margin: 0;
  height: 24px;
  border-radius: var(--jp-border-radius);
  display: flex;
  align-items: center;
  text-align: center;
  font-size: 14px;
  min-width: unset;
  min-height: unset;
}

button.jp-ToolbarButtonComponent:disabled {
  opacity: 0.4;
}

button.jp-ToolbarButtonComponent > span {
  padding: 0;
  flex: 0 0 auto;
}

button.jp-ToolbarButtonComponent .jp-ToolbarButtonComponent-label {
  font-size: var(--jp-ui-font-size1);
  line-height: 100%;
  padding-left: 2px;
  color: var(--jp-ui-font-color1);
  font-family: var(--jp-ui-font-family);
}

#jp-main-dock-panel[data-mode='single-document']
  .jp-MainAreaWidget
  > .jp-Toolbar.jp-Toolbar-micro {
  padding: 0;
  min-height: 0;
}

#jp-main-dock-panel[data-mode='single-document']
  .jp-MainAreaWidget
  > .jp-Toolbar {
  border: none;
  box-shadow: none;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-WindowedPanel-outer {
  position: relative;
  overflow-y: auto;
}

.jp-WindowedPanel-inner {
  position: relative;
}

.jp-WindowedPanel-window {
  position: absolute;
  left: 0;
  right: 0;
  overflow: visible;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* Sibling imports */

body {
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
}

/* Disable native link decoration styles everywhere outside of dialog boxes */
a {
  text-decoration: unset;
  color: unset;
}

a:hover {
  text-decoration: unset;
  color: unset;
}

/* Accessibility for links inside dialog box text */
.jp-Dialog-content a {
  text-decoration: revert;
  color: var(--jp-content-link-color);
}

.jp-Dialog-content a:hover {
  text-decoration: revert;
}

/* Styles for ui-components */
.jp-Button {
  color: var(--jp-ui-font-color2);
  border-radius: var(--jp-border-radius);
  padding: 0 12px;
  font-size: var(--jp-ui-font-size1);

  /* Copy from blueprint 3 */
  display: inline-flex;
  flex-direction: row;
  border: none;
  cursor: pointer;
  align-items: center;
  justify-content: center;
  text-align: left;
  vertical-align: middle;
  min-height: 30px;
  min-width: 30px;
}

.jp-Button:disabled {
  cursor: not-allowed;
}

.jp-Button:empty {
  padding: 0 !important;
}

.jp-Button.jp-mod-small {
  min-height: 24px;
  min-width: 24px;
  font-size: 12px;
  padding: 0 7px;
}

/* Use our own theme for hover styles */
.jp-Button.jp-mod-minimal:hover {
  background-color: var(--jp-layout-color2);
}

.jp-Button.jp-mod-minimal {
  background: none;
}

.jp-InputGroup {
  display: block;
  position: relative;
}

.jp-InputGroup input {
  box-sizing: border-box;
  border: none;
  border-radius: 0;
  background-color: transparent;
  color: var(--jp-ui-font-color0);
  box-shadow: inset 0 0 0 var(--jp-border-width) var(--jp-input-border-color);
  padding-bottom: 0;
  padding-top: 0;
  padding-left: 10px;
  padding-right: 28px;
  position: relative;
  width: 100%;
  -webkit-appearance: none;
  -moz-appearance: none;
  appearance: none;
  font-size: 14px;
  font-weight: 400;
  height: 30px;
  line-height: 30px;
  outline: none;
  vertical-align: middle;
}

.jp-InputGroup input:focus {
  box-shadow: inset 0 0 0 var(--jp-border-width)
      var(--jp-input-active-box-shadow-color),
    inset 0 0 0 3px var(--jp-input-active-box-shadow-color);
}

.jp-InputGroup input:disabled {
  cursor: not-allowed;
  resize: block;
  background-color: var(--jp-layout-color2);
  color: var(--jp-ui-font-color2);
}

.jp-InputGroup input:disabled ~ span {
  cursor: not-allowed;
  color: var(--jp-ui-font-color2);
}

.jp-InputGroup input::placeholder,
input::placeholder {
  color: var(--jp-ui-font-color2);
}

.jp-InputGroupAction {
  position: absolute;
  bottom: 1px;
  right: 0;
  padding: 6px;
}

.jp-HTMLSelect.jp-DefaultStyle select {
  background-color: initial;
  border: none;
  border-radius: 0;
  box-shadow: none;
  color: var(--jp-ui-font-color0);
  display: block;
  font-size: var(--jp-ui-font-size1);
  font-family: var(--jp-ui-font-family);
  height: 24px;
  line-height: 14px;
  padding: 0 25px 0 10px;
  text-align: left;
  -moz-appearance: none;
  -webkit-appearance: none;
}

.jp-HTMLSelect.jp-DefaultStyle select:disabled {
  background-color: var(--jp-layout-color2);
  color: var(--jp-ui-font-color2);
  cursor: not-allowed;
  resize: block;
}

.jp-HTMLSelect.jp-DefaultStyle select:disabled ~ span {
  cursor: not-allowed;
}

/* Use our own theme for hover and option styles */
/* stylelint-disable-next-line selector-max-type */
.jp-HTMLSelect.jp-DefaultStyle select:hover,
.jp-HTMLSelect.jp-DefaultStyle select > option {
  background-color: var(--jp-layout-color2);
  color: var(--jp-ui-font-color0);
}

select {
  box-sizing: border-box;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Styles
|----------------------------------------------------------------------------*/

.jp-StatusBar-Widget {
  display: flex;
  align-items: center;
  background: var(--jp-layout-color2);
  min-height: var(--jp-statusbar-height);
  justify-content: space-between;
  padding: 0 10px;
}

.jp-StatusBar-Left {
  display: flex;
  align-items: center;
  flex-direction: row;
}

.jp-StatusBar-Middle {
  display: flex;
  align-items: center;
}

.jp-StatusBar-Right {
  display: flex;
  align-items: center;
  flex-direction: row-reverse;
}

.jp-StatusBar-Item {
  max-height: var(--jp-statusbar-height);
  margin: 0 2px;
  height: var(--jp-statusbar-height);
  white-space: nowrap;
  text-overflow: ellipsis;
  color: var(--jp-ui-font-color1);
  padding: 0 6px;
}

.jp-mod-highlighted:hover {
  background-color: var(--jp-layout-color3);
}

.jp-mod-clicked {
  background-color: var(--jp-brand-color1);
}

.jp-mod-clicked:hover {
  background-color: var(--jp-brand-color0);
}

.jp-mod-clicked .jp-StatusBar-TextItem {
  color: var(--jp-ui-inverse-font-color1);
}

.jp-StatusBar-HoverItem {
  box-shadow: '0px 4px 4px rgba(0, 0, 0, 0.25)';
}

.jp-StatusBar-TextItem {
  font-size: var(--jp-ui-font-size1);
  font-family: var(--jp-ui-font-family);
  line-height: 24px;
  color: var(--jp-ui-font-color1);
}

.jp-StatusBar-GroupItem {
  display: flex;
  align-items: center;
  flex-direction: row;
}

.jp-Statusbar-ProgressCircle svg {
  display: block;
  margin: 0 auto;
  width: 16px;
  height: 24px;
  align-self: normal;
}

.jp-Statusbar-ProgressCircle path {
  fill: var(--jp-inverse-layout-color3);
}

.jp-Statusbar-ProgressBar-progress-bar {
  height: 10px;
  width: 100px;
  border: solid 0.25px var(--jp-brand-color2);
  border-radius: 3px;
  overflow: hidden;
  align-self: center;
}

.jp-Statusbar-ProgressBar-progress-bar > div {
  background-color: var(--jp-brand-color2);
  background-image: linear-gradient(
    -45deg,
    rgba(255, 255, 255, 0.2) 25%,
    transparent 25%,
    transparent 50%,
    rgba(255, 255, 255, 0.2) 50%,
    rgba(255, 255, 255, 0.2) 75%,
    transparent 75%,
    transparent
  );
  background-size: 40px 40px;
  float: left;
  width: 0%;
  height: 100%;
  font-size: 12px;
  line-height: 14px;
  color: #fff;
  text-align: center;
  animation: jp-Statusbar-ExecutionTime-progress-bar 2s linear infinite;
}

.jp-Statusbar-ProgressBar-progress-bar p {
  color: var(--jp-ui-font-color1);
  font-family: var(--jp-ui-font-family);
  font-size: var(--jp-ui-font-size1);
  line-height: 10px;
  width: 100px;
}

@keyframes jp-Statusbar-ExecutionTime-progress-bar {
  0% {
    background-position: 0 0;
  }

  100% {
    background-position: 40px 40px;
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------*/

:root {
  --jp-private-commandpalette-search-height: 28px;
}

/*-----------------------------------------------------------------------------
| Overall styles
|----------------------------------------------------------------------------*/

.lm-CommandPalette {
  padding-bottom: 0;
  color: var(--jp-ui-font-color1);
  background: var(--jp-layout-color1);

  /* This is needed so that all font sizing of children done in ems is
   * relative to this base size */
  font-size: var(--jp-ui-font-size1);
}

/*-----------------------------------------------------------------------------
| Modal variant
|----------------------------------------------------------------------------*/

.jp-ModalCommandPalette {
  position: absolute;
  z-index: 10000;
  top: 38px;
  left: 30%;
  margin: 0;
  padding: 4px;
  width: 40%;
  box-shadow: var(--jp-elevation-z4);
  border-radius: 4px;
  background: var(--jp-layout-color0);
}

.jp-ModalCommandPalette .lm-CommandPalette {
  max-height: 40vh;
}

.jp-ModalCommandPalette .lm-CommandPalette .lm-close-icon::after {
  display: none;
}

.jp-ModalCommandPalette .lm-CommandPalette .lm-CommandPalette-header {
  display: none;
}

.jp-ModalCommandPalette .lm-CommandPalette .lm-CommandPalette-item {
  margin-left: 4px;
  margin-right: 4px;
}

.jp-ModalCommandPalette
  .lm-CommandPalette
  .lm-CommandPalette-item.lm-mod-disabled {
  display: none;
}

/*-----------------------------------------------------------------------------
| Search
|----------------------------------------------------------------------------*/

.lm-CommandPalette-search {
  padding: 4px;
  background-color: var(--jp-layout-color1);
  z-index: 2;
}

.lm-CommandPalette-wrapper {
  overflow: overlay;
  padding: 0 9px;
  background-color: var(--jp-input-active-background);
  height: 30px;
  box-shadow: inset 0 0 0 var(--jp-border-width) var(--jp-input-border-color);
}

.lm-CommandPalette.lm-mod-focused .lm-CommandPalette-wrapper {
  box-shadow: inset 0 0 0 1px var(--jp-input-active-box-shadow-color),
    inset 0 0 0 3px var(--jp-input-active-box-shadow-color);
}

.jp-SearchIconGroup {
  color: white;
  background-color: var(--jp-brand-color1);
  position: absolute;
  top: 4px;
  right: 4px;
  padding: 5px 5px 1px;
}

.jp-SearchIconGroup svg {
  height: 20px;
  width: 20px;
}

.jp-SearchIconGroup .jp-icon3[fill] {
  fill: var(--jp-layout-color0);
}

.lm-CommandPalette-input {
  background: transparent;
  width: calc(100% - 18px);
  float: left;
  border: none;
  outline: none;
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color0);
  line-height: var(--jp-private-commandpalette-search-height);
}

.lm-CommandPalette-input::-webkit-input-placeholder,
.lm-CommandPalette-input::-moz-placeholder,
.lm-CommandPalette-input:-ms-input-placeholder {
  color: var(--jp-ui-font-color2);
  font-size: var(--jp-ui-font-size1);
}

/*-----------------------------------------------------------------------------
| Results
|----------------------------------------------------------------------------*/

.lm-CommandPalette-header:first-child {
  margin-top: 0;
}

.lm-CommandPalette-header {
  border-bottom: solid var(--jp-border-width) var(--jp-border-color2);
  color: var(--jp-ui-font-color1);
  cursor: pointer;
  display: flex;
  font-size: var(--jp-ui-font-size0);
  font-weight: 600;
  letter-spacing: 1px;
  margin-top: 8px;
  padding: 8px 0 8px 12px;
  text-transform: uppercase;
}

.lm-CommandPalette-header.lm-mod-active {
  background: var(--jp-layout-color2);
}

.lm-CommandPalette-header > mark {
  background-color: transparent;
  font-weight: bold;
  color: var(--jp-ui-font-color1);
}

.lm-CommandPalette-item {
  padding: 4px 12px 4px 4px;
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
  font-weight: 400;
  display: flex;
}

.lm-CommandPalette-item.lm-mod-disabled {
  color: var(--jp-ui-font-color2);
}

.lm-CommandPalette-item.lm-mod-active {
  color: var(--jp-ui-inverse-font-color1);
  background: var(--jp-brand-color1);
}

.lm-CommandPalette-item.lm-mod-active .lm-CommandPalette-itemLabel > mark {
  color: var(--jp-ui-inverse-font-color0);
}

.lm-CommandPalette-item.lm-mod-active .jp-icon-selectable[fill] {
  fill: var(--jp-layout-color0);
}

.lm-CommandPalette-item.lm-mod-active:hover:not(.lm-mod-disabled) {
  color: var(--jp-ui-inverse-font-color1);
  background: var(--jp-brand-color1);
}

.lm-CommandPalette-item:hover:not(.lm-mod-active):not(.lm-mod-disabled) {
  background: var(--jp-layout-color2);
}

.lm-CommandPalette-itemContent {
  overflow: hidden;
}

.lm-CommandPalette-itemLabel > mark {
  color: var(--jp-ui-font-color0);
  background-color: transparent;
  font-weight: bold;
}

.lm-CommandPalette-item.lm-mod-disabled mark {
  color: var(--jp-ui-font-color2);
}

.lm-CommandPalette-item .lm-CommandPalette-itemIcon {
  margin: 0 4px 0 0;
  position: relative;
  width: 16px;
  top: 2px;
  flex: 0 0 auto;
}

.lm-CommandPalette-item.lm-mod-disabled .lm-CommandPalette-itemIcon {
  opacity: 0.6;
}

.lm-CommandPalette-item .lm-CommandPalette-itemShortcut {
  flex: 0 0 auto;
}

.lm-CommandPalette-itemCaption {
  display: none;
}

.lm-CommandPalette-content {
  background-color: var(--jp-layout-color1);
}

.lm-CommandPalette-content:empty::after {
  content: 'No results';
  margin: auto;
  margin-top: 20px;
  width: 100px;
  display: block;
  font-size: var(--jp-ui-font-size2);
  font-family: var(--jp-ui-font-family);
  font-weight: lighter;
}

.lm-CommandPalette-emptyMessage {
  text-align: center;
  margin-top: 24px;
  line-height: 1.32;
  padding: 0 8px;
  color: var(--jp-content-font-color3);
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Dialog {
  position: absolute;
  z-index: 10000;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  top: 0;
  left: 0;
  margin: 0;
  padding: 0;
  width: 100%;
  height: 100%;
  background: var(--jp-dialog-background);
}

.jp-Dialog-content {
  display: flex;
  flex-direction: column;
  margin-left: auto;
  margin-right: auto;
  background: var(--jp-layout-color1);
  padding: 24px 24px 12px;
  min-width: 300px;
  min-height: 150px;
  max-width: 1000px;
  max-height: 500px;
  box-sizing: border-box;
  box-shadow: var(--jp-elevation-z20);
  word-wrap: break-word;
  border-radius: var(--jp-border-radius);

  /* This is needed so that all font sizing of children done in ems is
   * relative to this base size */
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color1);
  resize: both;
}

.jp-Dialog-content.jp-Dialog-content-small {
  max-width: 500px;
}

.jp-Dialog-button {
  overflow: visible;
}

button.jp-Dialog-button:focus {
  outline: 1px solid var(--jp-brand-color1);
  outline-offset: 4px;
  -moz-outline-radius: 0;
}

button.jp-Dialog-button:focus::-moz-focus-inner {
  border: 0;
}

button.jp-Dialog-button.jp-mod-styled.jp-mod-accept:focus,
button.jp-Dialog-button.jp-mod-styled.jp-mod-warn:focus,
button.jp-Dialog-button.jp-mod-styled.jp-mod-reject:focus {
  outline-offset: 4px;
  -moz-outline-radius: 0;
}

button.jp-Dialog-button.jp-mod-styled.jp-mod-accept:focus {
  outline: 1px solid var(--jp-accept-color-normal, var(--jp-brand-color1));
}

button.jp-Dialog-button.jp-mod-styled.jp-mod-warn:focus {
  outline: 1px solid var(--jp-warn-color-normal, var(--jp-error-color1));
}

button.jp-Dialog-button.jp-mod-styled.jp-mod-reject:focus {
  outline: 1px solid var(--jp-reject-color-normal, var(--md-grey-600));
}

button.jp-Dialog-close-button {
  padding: 0;
  height: 100%;
  min-width: unset;
  min-height: unset;
}

.jp-Dialog-header {
  display: flex;
  justify-content: space-between;
  flex: 0 0 auto;
  padding-bottom: 12px;
  font-size: var(--jp-ui-font-size3);
  font-weight: 400;
  color: var(--jp-ui-font-color1);
}

.jp-Dialog-body {
  display: flex;
  flex-direction: column;
  flex: 1 1 auto;
  font-size: var(--jp-ui-font-size1);
  background: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  overflow: auto;
}

.jp-Dialog-footer {
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  align-items: center;
  flex: 0 0 auto;
  margin-left: -12px;
  margin-right: -12px;
  padding: 12px;
}

.jp-Dialog-checkbox {
  padding-right: 5px;
}

.jp-Dialog-checkbox > input:focus-visible {
  outline: 1px solid var(--jp-input-active-border-color);
  outline-offset: 1px;
}

.jp-Dialog-spacer {
  flex: 1 1 auto;
}

.jp-Dialog-title {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.jp-Dialog-body > .jp-select-wrapper {
  width: 100%;
}

.jp-Dialog-body > button {
  padding: 0 16px;
}

.jp-Dialog-body > label {
  line-height: 1.4;
  color: var(--jp-ui-font-color0);
}

.jp-Dialog-button.jp-mod-styled:not(:last-child) {
  margin-right: 12px;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-Input-Boolean-Dialog {
  flex-direction: row-reverse;
  align-items: end;
  width: 100%;
}

.jp-Input-Boolean-Dialog > label {
  flex: 1 1 auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-MainAreaWidget > :focus {
  outline: none;
}

.jp-MainAreaWidget .jp-MainAreaWidget-error {
  padding: 6px;
}

.jp-MainAreaWidget .jp-MainAreaWidget-error > pre {
  width: auto;
  padding: 10px;
  background: var(--jp-error-color3);
  border: var(--jp-border-width) solid var(--jp-error-color1);
  border-radius: var(--jp-border-radius);
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
  white-space: pre-wrap;
  word-wrap: break-word;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/**
 * google-material-color v1.2.6
 * https://github.com/danlevan/google-material-color
 */
:root {
  --md-red-50: #ffebee;
  --md-red-100: #ffcdd2;
  --md-red-200: #ef9a9a;
  --md-red-300: #e57373;
  --md-red-400: #ef5350;
  --md-red-500: #f44336;
  --md-red-600: #e53935;
  --md-red-700: #d32f2f;
  --md-red-800: #c62828;
  --md-red-900: #b71c1c;
  --md-red-A100: #ff8a80;
  --md-red-A200: #ff5252;
  --md-red-A400: #ff1744;
  --md-red-A700: #d50000;
  --md-pink-50: #fce4ec;
  --md-pink-100: #f8bbd0;
  --md-pink-200: #f48fb1;
  --md-pink-300: #f06292;
  --md-pink-400: #ec407a;
  --md-pink-500: #e91e63;
  --md-pink-600: #d81b60;
  --md-pink-700: #c2185b;
  --md-pink-800: #ad1457;
  --md-pink-900: #880e4f;
  --md-pink-A100: #ff80ab;
  --md-pink-A200: #ff4081;
  --md-pink-A400: #f50057;
  --md-pink-A700: #c51162;
  --md-purple-50: #f3e5f5;
  --md-purple-100: #e1bee7;
  --md-purple-200: #ce93d8;
  --md-purple-300: #ba68c8;
  --md-purple-400: #ab47bc;
  --md-purple-500: #9c27b0;
  --md-purple-600: #8e24aa;
  --md-purple-700: #7b1fa2;
  --md-purple-800: #6a1b9a;
  --md-purple-900: #4a148c;
  --md-purple-A100: #ea80fc;
  --md-purple-A200: #e040fb;
  --md-purple-A400: #d500f9;
  --md-purple-A700: #a0f;
  --md-deep-purple-50: #ede7f6;
  --md-deep-purple-100: #d1c4e9;
  --md-deep-purple-200: #b39ddb;
  --md-deep-purple-300: #9575cd;
  --md-deep-purple-400: #7e57c2;
  --md-deep-purple-500: #673ab7;
  --md-deep-purple-600: #5e35b1;
  --md-deep-purple-700: #512da8;
  --md-deep-purple-800: #4527a0;
  --md-deep-purple-900: #311b92;
  --md-deep-purple-A100: #b388ff;
  --md-deep-purple-A200: #7c4dff;
  --md-deep-purple-A400: #651fff;
  --md-deep-purple-A700: #6200ea;
  --md-indigo-50: #e8eaf6;
  --md-indigo-100: #c5cae9;
  --md-indigo-200: #9fa8da;
  --md-indigo-300: #7986cb;
  --md-indigo-400: #5c6bc0;
  --md-indigo-500: #3f51b5;
  --md-indigo-600: #3949ab;
  --md-indigo-700: #303f9f;
  --md-indigo-800: #283593;
  --md-indigo-900: #1a237e;
  --md-indigo-A100: #8c9eff;
  --md-indigo-A200: #536dfe;
  --md-indigo-A400: #3d5afe;
  --md-indigo-A700: #304ffe;
  --md-blue-50: #e3f2fd;
  --md-blue-100: #bbdefb;
  --md-blue-200: #90caf9;
  --md-blue-300: #64b5f6;
  --md-blue-400: #42a5f5;
  --md-blue-500: #2196f3;
  --md-blue-600: #1e88e5;
  --md-blue-700: #1976d2;
  --md-blue-800: #1565c0;
  --md-blue-900: #0d47a1;
  --md-blue-A100: #82b1ff;
  --md-blue-A200: #448aff;
  --md-blue-A400: #2979ff;
  --md-blue-A700: #2962ff;
  --md-light-blue-50: #e1f5fe;
  --md-light-blue-100: #b3e5fc;
  --md-light-blue-200: #81d4fa;
  --md-light-blue-300: #4fc3f7;
  --md-light-blue-400: #29b6f6;
  --md-light-blue-500: #03a9f4;
  --md-light-blue-600: #039be5;
  --md-light-blue-700: #0288d1;
  --md-light-blue-800: #0277bd;
  --md-light-blue-900: #01579b;
  --md-light-blue-A100: #80d8ff;
  --md-light-blue-A200: #40c4ff;
  --md-light-blue-A400: #00b0ff;
  --md-light-blue-A700: #0091ea;
  --md-cyan-50: #e0f7fa;
  --md-cyan-100: #b2ebf2;
  --md-cyan-200: #80deea;
  --md-cyan-300: #4dd0e1;
  --md-cyan-400: #26c6da;
  --md-cyan-500: #00bcd4;
  --md-cyan-600: #00acc1;
  --md-cyan-700: #0097a7;
  --md-cyan-800: #00838f;
  --md-cyan-900: #006064;
  --md-cyan-A100: #84ffff;
  --md-cyan-A200: #18ffff;
  --md-cyan-A400: #00e5ff;
  --md-cyan-A700: #00b8d4;
  --md-teal-50: #e0f2f1;
  --md-teal-100: #b2dfdb;
  --md-teal-200: #80cbc4;
  --md-teal-300: #4db6ac;
  --md-teal-400: #26a69a;
  --md-teal-500: #009688;
  --md-teal-600: #00897b;
  --md-teal-700: #00796b;
  --md-teal-800: #00695c;
  --md-teal-900: #004d40;
  --md-teal-A100: #a7ffeb;
  --md-teal-A200: #64ffda;
  --md-teal-A400: #1de9b6;
  --md-teal-A700: #00bfa5;
  --md-green-50: #e8f5e9;
  --md-green-100: #c8e6c9;
  --md-green-200: #a5d6a7;
  --md-green-300: #81c784;
  --md-green-400: #66bb6a;
  --md-green-500: #4caf50;
  --md-green-600: #43a047;
  --md-green-700: #388e3c;
  --md-green-800: #2e7d32;
  --md-green-900: #1b5e20;
  --md-green-A100: #b9f6ca;
  --md-green-A200: #69f0ae;
  --md-green-A400: #00e676;
  --md-green-A700: #00c853;
  --md-light-green-50: #f1f8e9;
  --md-light-green-100: #dcedc8;
  --md-light-green-200: #c5e1a5;
  --md-light-green-300: #aed581;
  --md-light-green-400: #9ccc65;
  --md-light-green-500: #8bc34a;
  --md-light-green-600: #7cb342;
  --md-light-green-700: #689f38;
  --md-light-green-800: #558b2f;
  --md-light-green-900: #33691e;
  --md-light-green-A100: #ccff90;
  --md-light-green-A200: #b2ff59;
  --md-light-green-A400: #76ff03;
  --md-light-green-A700: #64dd17;
  --md-lime-50: #f9fbe7;
  --md-lime-100: #f0f4c3;
  --md-lime-200: #e6ee9c;
  --md-lime-300: #dce775;
  --md-lime-400: #d4e157;
  --md-lime-500: #cddc39;
  --md-lime-600: #c0ca33;
  --md-lime-700: #afb42b;
  --md-lime-800: #9e9d24;
  --md-lime-900: #827717;
  --md-lime-A100: #f4ff81;
  --md-lime-A200: #eeff41;
  --md-lime-A400: #c6ff00;
  --md-lime-A700: #aeea00;
  --md-yellow-50: #fffde7;
  --md-yellow-100: #fff9c4;
  --md-yellow-200: #fff59d;
  --md-yellow-300: #fff176;
  --md-yellow-400: #ffee58;
  --md-yellow-500: #ffeb3b;
  --md-yellow-600: #fdd835;
  --md-yellow-700: #fbc02d;
  --md-yellow-800: #f9a825;
  --md-yellow-900: #f57f17;
  --md-yellow-A100: #ffff8d;
  --md-yellow-A200: #ff0;
  --md-yellow-A400: #ffea00;
  --md-yellow-A700: #ffd600;
  --md-amber-50: #fff8e1;
  --md-amber-100: #ffecb3;
  --md-amber-200: #ffe082;
  --md-amber-300: #ffd54f;
  --md-amber-400: #ffca28;
  --md-amber-500: #ffc107;
  --md-amber-600: #ffb300;
  --md-amber-700: #ffa000;
  --md-amber-800: #ff8f00;
  --md-amber-900: #ff6f00;
  --md-amber-A100: #ffe57f;
  --md-amber-A200: #ffd740;
  --md-amber-A400: #ffc400;
  --md-amber-A700: #ffab00;
  --md-orange-50: #fff3e0;
  --md-orange-100: #ffe0b2;
  --md-orange-200: #ffcc80;
  --md-orange-300: #ffb74d;
  --md-orange-400: #ffa726;
  --md-orange-500: #ff9800;
  --md-orange-600: #fb8c00;
  --md-orange-700: #f57c00;
  --md-orange-800: #ef6c00;
  --md-orange-900: #e65100;
  --md-orange-A100: #ffd180;
  --md-orange-A200: #ffab40;
  --md-orange-A400: #ff9100;
  --md-orange-A700: #ff6d00;
  --md-deep-orange-50: #fbe9e7;
  --md-deep-orange-100: #ffccbc;
  --md-deep-orange-200: #ffab91;
  --md-deep-orange-300: #ff8a65;
  --md-deep-orange-400: #ff7043;
  --md-deep-orange-500: #ff5722;
  --md-deep-orange-600: #f4511e;
  --md-deep-orange-700: #e64a19;
  --md-deep-orange-800: #d84315;
  --md-deep-orange-900: #bf360c;
  --md-deep-orange-A100: #ff9e80;
  --md-deep-orange-A200: #ff6e40;
  --md-deep-orange-A400: #ff3d00;
  --md-deep-orange-A700: #dd2c00;
  --md-brown-50: #efebe9;
  --md-brown-100: #d7ccc8;
  --md-brown-200: #bcaaa4;
  --md-brown-300: #a1887f;
  --md-brown-400: #8d6e63;
  --md-brown-500: #795548;
  --md-brown-600: #6d4c41;
  --md-brown-700: #5d4037;
  --md-brown-800: #4e342e;
  --md-brown-900: #3e2723;
  --md-grey-50: #fafafa;
  --md-grey-100: #f5f5f5;
  --md-grey-200: #eee;
  --md-grey-300: #e0e0e0;
  --md-grey-400: #bdbdbd;
  --md-grey-500: #9e9e9e;
  --md-grey-600: #757575;
  --md-grey-700: #616161;
  --md-grey-800: #424242;
  --md-grey-900: #212121;
  --md-blue-grey-50: #eceff1;
  --md-blue-grey-100: #cfd8dc;
  --md-blue-grey-200: #b0bec5;
  --md-blue-grey-300: #90a4ae;
  --md-blue-grey-400: #78909c;
  --md-blue-grey-500: #607d8b;
  --md-blue-grey-600: #546e7a;
  --md-blue-grey-700: #455a64;
  --md-blue-grey-800: #37474f;
  --md-blue-grey-900: #263238;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| RenderedText
|----------------------------------------------------------------------------*/

:root {
  /* This is the padding value to fill the gaps between lines containing spans with background color. */
  --jp-private-code-span-padding: calc(
    (var(--jp-code-line-height) - 1) * var(--jp-code-font-size) / 2
  );
}

.jp-RenderedText {
  text-align: left;
  padding-left: var(--jp-code-padding);
  line-height: var(--jp-code-line-height);
  font-family: var(--jp-code-font-family);
}

.jp-RenderedText pre,
.jp-RenderedJavaScript pre,
.jp-RenderedHTMLCommon pre {
  color: var(--jp-content-font-color1);
  font-size: var(--jp-code-font-size);
  border: none;
  margin: 0;
  padding: 0;
}

.jp-RenderedText pre a:link {
  text-decoration: none;
  color: var(--jp-content-link-color);
}

.jp-RenderedText pre a:hover {
  text-decoration: underline;
  color: var(--jp-content-link-color);
}

.jp-RenderedText pre a:visited {
  text-decoration: none;
  color: var(--jp-content-link-color);
}

/* console foregrounds and backgrounds */
.jp-RenderedText pre .ansi-black-fg {
  color: #3e424d;
}

.jp-RenderedText pre .ansi-red-fg {
  color: #e75c58;
}

.jp-RenderedText pre .ansi-green-fg {
  color: #00a250;
}

.jp-RenderedText pre .ansi-yellow-fg {
  color: #ddb62b;
}

.jp-RenderedText pre .ansi-blue-fg {
  color: #208ffb;
}

.jp-RenderedText pre .ansi-magenta-fg {
  color: #d160c4;
}

.jp-RenderedText pre .ansi-cyan-fg {
  color: #60c6c8;
}

.jp-RenderedText pre .ansi-white-fg {
  color: #c5c1b4;
}

.jp-RenderedText pre .ansi-black-bg {
  background-color: #3e424d;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-red-bg {
  background-color: #e75c58;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-green-bg {
  background-color: #00a250;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-yellow-bg {
  background-color: #ddb62b;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-blue-bg {
  background-color: #208ffb;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-magenta-bg {
  background-color: #d160c4;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-cyan-bg {
  background-color: #60c6c8;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-white-bg {
  background-color: #c5c1b4;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-black-intense-fg {
  color: #282c36;
}

.jp-RenderedText pre .ansi-red-intense-fg {
  color: #b22b31;
}

.jp-RenderedText pre .ansi-green-intense-fg {
  color: #007427;
}

.jp-RenderedText pre .ansi-yellow-intense-fg {
  color: #b27d12;
}

.jp-RenderedText pre .ansi-blue-intense-fg {
  color: #0065ca;
}

.jp-RenderedText pre .ansi-magenta-intense-fg {
  color: #a03196;
}

.jp-RenderedText pre .ansi-cyan-intense-fg {
  color: #258f8f;
}

.jp-RenderedText pre .ansi-white-intense-fg {
  color: #a1a6b2;
}

.jp-RenderedText pre .ansi-black-intense-bg {
  background-color: #282c36;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-red-intense-bg {
  background-color: #b22b31;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-green-intense-bg {
  background-color: #007427;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-yellow-intense-bg {
  background-color: #b27d12;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-blue-intense-bg {
  background-color: #0065ca;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-magenta-intense-bg {
  background-color: #a03196;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-cyan-intense-bg {
  background-color: #258f8f;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-white-intense-bg {
  background-color: #a1a6b2;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-default-inverse-fg {
  color: var(--jp-ui-inverse-font-color0);
}

.jp-RenderedText pre .ansi-default-inverse-bg {
  background-color: var(--jp-inverse-layout-color0);
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-bold {
  font-weight: bold;
}

.jp-RenderedText pre .ansi-underline {
  text-decoration: underline;
}

.jp-RenderedText[data-mime-type='application/vnd.jupyter.stderr'] {
  background: var(--jp-rendermime-error-background);
  padding-top: var(--jp-code-padding);
}

/*-----------------------------------------------------------------------------
| RenderedLatex
|----------------------------------------------------------------------------*/

.jp-RenderedLatex {
  color: var(--jp-content-font-color1);
  font-size: var(--jp-content-font-size1);
  line-height: var(--jp-content-line-height);
}

/* Left-justify outputs.*/
.jp-OutputArea-output.jp-RenderedLatex {
  padding: var(--jp-code-padding);
  text-align: left;
}

/*-----------------------------------------------------------------------------
| RenderedHTML
|----------------------------------------------------------------------------*/

.jp-RenderedHTMLCommon {
  color: var(--jp-content-font-color1);
  font-family: var(--jp-content-font-family);
  font-size: var(--jp-content-font-size1);
  line-height: var(--jp-content-line-height);

  /* Give a bit more R padding on Markdown text to keep line lengths reasonable */
  padding-right: 20px;
}

.jp-RenderedHTMLCommon em {
  font-style: italic;
}

.jp-RenderedHTMLCommon strong {
  font-weight: bold;
}

.jp-RenderedHTMLCommon u {
  text-decoration: underline;
}

.jp-RenderedHTMLCommon a:link {
  text-decoration: none;
  color: var(--jp-content-link-color);
}

.jp-RenderedHTMLCommon a:hover {
  text-decoration: underline;
  color: var(--jp-content-link-color);
}

.jp-RenderedHTMLCommon a:visited {
  text-decoration: none;
  color: var(--jp-content-link-color);
}

/* Headings */

.jp-RenderedHTMLCommon h1,
.jp-RenderedHTMLCommon h2,
.jp-RenderedHTMLCommon h3,
.jp-RenderedHTMLCommon h4,
.jp-RenderedHTMLCommon h5,
.jp-RenderedHTMLCommon h6 {
  line-height: var(--jp-content-heading-line-height);
  font-weight: var(--jp-content-heading-font-weight);
  font-style: normal;
  margin: var(--jp-content-heading-margin-top) 0
    var(--jp-content-heading-margin-bottom) 0;
}

.jp-RenderedHTMLCommon h1:first-child,
.jp-RenderedHTMLCommon h2:first-child,
.jp-RenderedHTMLCommon h3:first-child,
.jp-RenderedHTMLCommon h4:first-child,
.jp-RenderedHTMLCommon h5:first-child,
.jp-RenderedHTMLCommon h6:first-child {
  margin-top: calc(0.5 * var(--jp-content-heading-margin-top));
}

.jp-RenderedHTMLCommon h1:last-child,
.jp-RenderedHTMLCommon h2:last-child,
.jp-RenderedHTMLCommon h3:last-child,
.jp-RenderedHTMLCommon h4:last-child,
.jp-RenderedHTMLCommon h5:last-child,
.jp-RenderedHTMLCommon h6:last-child {
  margin-bottom: calc(0.5 * var(--jp-content-heading-margin-bottom));
}

.jp-RenderedHTMLCommon h1 {
  font-size: var(--jp-content-font-size5);
}

.jp-RenderedHTMLCommon h2 {
  font-size: var(--jp-content-font-size4);
}

.jp-RenderedHTMLCommon h3 {
  font-size: var(--jp-content-font-size3);
}

.jp-RenderedHTMLCommon h4 {
  font-size: var(--jp-content-font-size2);
}

.jp-RenderedHTMLCommon h5 {
  font-size: var(--jp-content-font-size1);
}

.jp-RenderedHTMLCommon h6 {
  font-size: var(--jp-content-font-size0);
}

/* Lists */

/* stylelint-disable selector-max-type, selector-max-compound-selectors */

.jp-RenderedHTMLCommon ul:not(.list-inline),
.jp-RenderedHTMLCommon ol:not(.list-inline) {
  padding-left: 2em;
}

.jp-RenderedHTMLCommon ul {
  list-style: disc;
}

.jp-RenderedHTMLCommon ul ul {
  list-style: square;
}

.jp-RenderedHTMLCommon ul ul ul {
  list-style: circle;
}

.jp-RenderedHTMLCommon ol {
  list-style: decimal;
}

.jp-RenderedHTMLCommon ol ol {
  list-style: upper-alpha;
}

.jp-RenderedHTMLCommon ol ol ol {
  list-style: lower-alpha;
}

.jp-RenderedHTMLCommon ol ol ol ol {
  list-style: lower-roman;
}

.jp-RenderedHTMLCommon ol ol ol ol ol {
  list-style: decimal;
}

.jp-RenderedHTMLCommon ol,
.jp-RenderedHTMLCommon ul {
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon ul ul,
.jp-RenderedHTMLCommon ul ol,
.jp-RenderedHTMLCommon ol ul,
.jp-RenderedHTMLCommon ol ol {
  margin-bottom: 0;
}

/* stylelint-enable selector-max-type, selector-max-compound-selectors */

.jp-RenderedHTMLCommon hr {
  color: var(--jp-border-color2);
  background-color: var(--jp-border-color1);
  margin-top: 1em;
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon > pre {
  margin: 1.5em 2em;
}

.jp-RenderedHTMLCommon pre,
.jp-RenderedHTMLCommon code {
  border: 0;
  background-color: var(--jp-layout-color0);
  color: var(--jp-content-font-color1);
  font-family: var(--jp-code-font-family);
  font-size: inherit;
  line-height: var(--jp-code-line-height);
  padding: 0;
  white-space: pre-wrap;
}

.jp-RenderedHTMLCommon :not(pre) > code {
  background-color: var(--jp-layout-color2);
  padding: 1px 5px;
}

/* Tables */

.jp-RenderedHTMLCommon table {
  border-collapse: collapse;
  border-spacing: 0;
  border: none;
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
  table-layout: fixed;
  margin-left: auto;
  margin-bottom: 1em;
  margin-right: auto;
}

.jp-RenderedHTMLCommon thead {
  border-bottom: var(--jp-border-width) solid var(--jp-border-color1);
  vertical-align: bottom;
}

.jp-RenderedHTMLCommon td,
.jp-RenderedHTMLCommon th,
.jp-RenderedHTMLCommon tr {
  vertical-align: middle;
  padding: 0.5em;
  line-height: normal;
  white-space: normal;
  max-width: none;
  border: none;
}

.jp-RenderedMarkdown.jp-RenderedHTMLCommon td,
.jp-RenderedMarkdown.jp-RenderedHTMLCommon th {
  max-width: none;
}

:not(.jp-RenderedMarkdown).jp-RenderedHTMLCommon td,
:not(.jp-RenderedMarkdown).jp-RenderedHTMLCommon th,
:not(.jp-RenderedMarkdown).jp-RenderedHTMLCommon tr {
  text-align: right;
}

.jp-RenderedHTMLCommon th {
  font-weight: bold;
}

.jp-RenderedHTMLCommon tbody tr:nth-child(odd) {
  background: var(--jp-layout-color0);
}

.jp-RenderedHTMLCommon tbody tr:nth-child(even) {
  background: var(--jp-rendermime-table-row-background);
}

.jp-RenderedHTMLCommon tbody tr:hover {
  background: var(--jp-rendermime-table-row-hover-background);
}

.jp-RenderedHTMLCommon p {
  text-align: left;
  margin: 0;
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon img {
  -moz-force-broken-image-icon: 1;
}

/* Restrict to direct children as other images could be nested in other content. */
.jp-RenderedHTMLCommon > img {
  display: block;
  margin-left: 0;
  margin-right: 0;
  margin-bottom: 1em;
}

/* Change color behind transparent images if they need it... */
[data-jp-theme-light='false'] .jp-RenderedImage img.jp-needs-light-background {
  background-color: var(--jp-inverse-layout-color1);
}

[data-jp-theme-light='true'] .jp-RenderedImage img.jp-needs-dark-background {
  background-color: var(--jp-inverse-layout-color1);
}

.jp-RenderedHTMLCommon img,
.jp-RenderedImage img,
.jp-RenderedHTMLCommon svg,
.jp-RenderedSVG svg {
  max-width: 100%;
  height: auto;
}

.jp-RenderedHTMLCommon img.jp-mod-unconfined,
.jp-RenderedImage img.jp-mod-unconfined,
.jp-RenderedHTMLCommon svg.jp-mod-unconfined,
.jp-RenderedSVG svg.jp-mod-unconfined {
  max-width: none;
}

.jp-RenderedHTMLCommon .alert {
  padding: var(--jp-notebook-padding);
  border: var(--jp-border-width) solid transparent;
  border-radius: var(--jp-border-radius);
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon .alert-info {
  color: var(--jp-info-color0);
  background-color: var(--jp-info-color3);
  border-color: var(--jp-info-color2);
}

.jp-RenderedHTMLCommon .alert-info hr {
  border-color: var(--jp-info-color3);
}

.jp-RenderedHTMLCommon .alert-info > p:last-child,
.jp-RenderedHTMLCommon .alert-info > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon .alert-warning {
  color: var(--jp-warn-color0);
  background-color: var(--jp-warn-color3);
  border-color: var(--jp-warn-color2);
}

.jp-RenderedHTMLCommon .alert-warning hr {
  border-color: var(--jp-warn-color3);
}

.jp-RenderedHTMLCommon .alert-warning > p:last-child,
.jp-RenderedHTMLCommon .alert-warning > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon .alert-success {
  color: var(--jp-success-color0);
  background-color: var(--jp-success-color3);
  border-color: var(--jp-success-color2);
}

.jp-RenderedHTMLCommon .alert-success hr {
  border-color: var(--jp-success-color3);
}

.jp-RenderedHTMLCommon .alert-success > p:last-child,
.jp-RenderedHTMLCommon .alert-success > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon .alert-danger {
  color: var(--jp-error-color0);
  background-color: var(--jp-error-color3);
  border-color: var(--jp-error-color2);
}

.jp-RenderedHTMLCommon .alert-danger hr {
  border-color: var(--jp-error-color3);
}

.jp-RenderedHTMLCommon .alert-danger > p:last-child,
.jp-RenderedHTMLCommon .alert-danger > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon blockquote {
  margin: 1em 2em;
  padding: 0 1em;
  border-left: 5px solid var(--jp-border-color2);
}

a.jp-InternalAnchorLink {
  visibility: hidden;
  margin-left: 8px;
  color: var(--md-blue-800);
}

h1:hover .jp-InternalAnchorLink,
h2:hover .jp-InternalAnchorLink,
h3:hover .jp-InternalAnchorLink,
h4:hover .jp-InternalAnchorLink,
h5:hover .jp-InternalAnchorLink,
h6:hover .jp-InternalAnchorLink {
  visibility: visible;
}

.jp-RenderedHTMLCommon kbd {
  background-color: var(--jp-rendermime-table-row-background);
  border: 1px solid var(--jp-border-color0);
  border-bottom-color: var(--jp-border-color2);
  border-radius: 3px;
  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.25);
  display: inline-block;
  font-size: var(--jp-ui-font-size0);
  line-height: 1em;
  padding: 0.2em 0.5em;
}

/* Most direct children of .jp-RenderedHTMLCommon have a margin-bottom of 1.0.
 * At the bottom of cells this is a bit too much as there is also spacing
 * between cells. Going all the way to 0 gets too tight between markdown and
 * code cells.
 */
.jp-RenderedHTMLCommon > *:last-child {
  margin-bottom: 0.5em;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-cursor-backdrop {
  position: fixed;
  width: 200px;
  height: 200px;
  margin-top: -100px;
  margin-left: -100px;
  will-change: transform;
  z-index: 100;
}

.lm-mod-drag-image {
  will-change: transform;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-lineFormSearch {
  padding: 4px 12px;
  background-color: var(--jp-layout-color2);
  box-shadow: var(--jp-toolbar-box-shadow);
  z-index: 2;
  font-size: var(--jp-ui-font-size1);
}

.jp-lineFormCaption {
  font-size: var(--jp-ui-font-size0);
  line-height: var(--jp-ui-font-size1);
  margin-top: 4px;
  color: var(--jp-ui-font-color0);
}

.jp-baseLineForm {
  border: none;
  border-radius: 0;
  position: absolute;
  background-size: 16px;
  background-repeat: no-repeat;
  background-position: center;
  outline: none;
}

.jp-lineFormButtonContainer {
  top: 4px;
  right: 8px;
  height: 24px;
  padding: 0 12px;
  width: 12px;
}

.jp-lineFormButtonIcon {
  top: 0;
  right: 0;
  background-color: var(--jp-brand-color1);
  height: 100%;
  width: 100%;
  box-sizing: border-box;
  padding: 4px 6px;
}

.jp-lineFormButton {
  top: 0;
  right: 0;
  background-color: transparent;
  height: 100%;
  width: 100%;
  box-sizing: border-box;
}

.jp-lineFormWrapper {
  overflow: hidden;
  padding: 0 8px;
  border: 1px solid var(--jp-border-color0);
  background-color: var(--jp-input-active-background);
  height: 22px;
}

.jp-lineFormWrapperFocusWithin {
  border: var(--jp-border-width) solid var(--md-blue-500);
  box-shadow: inset 0 0 4px var(--md-blue-300);
}

.jp-lineFormInput {
  background: transparent;
  width: 200px;
  height: 100%;
  border: none;
  outline: none;
  color: var(--jp-ui-font-color0);
  line-height: 28px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-JSONEditor {
  display: flex;
  flex-direction: column;
  width: 100%;
}

.jp-JSONEditor-host {
  flex: 1 1 auto;
  border: var(--jp-border-width) solid var(--jp-input-border-color);
  border-radius: 0;
  background: var(--jp-layout-color0);
  min-height: 50px;
  padding: 1px;
}

.jp-JSONEditor.jp-mod-error .jp-JSONEditor-host {
  border-color: red;
  outline-color: red;
}

.jp-JSONEditor-header {
  display: flex;
  flex: 1 0 auto;
  padding: 0 0 0 12px;
}

.jp-JSONEditor-header label {
  flex: 0 0 auto;
}

.jp-JSONEditor-commitButton {
  height: 16px;
  width: 16px;
  background-size: 18px;
  background-repeat: no-repeat;
  background-position: center;
}

.jp-JSONEditor-host.jp-mod-focused {
  background-color: var(--jp-input-active-background);
  border: 1px solid var(--jp-input-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
}

.jp-Editor.jp-mod-dropTarget {
  border: var(--jp-border-width) solid var(--jp-input-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/
.jp-DocumentSearch-input {
  border: none;
  outline: none;
  color: var(--jp-ui-font-color0);
  font-size: var(--jp-ui-font-size1);
  background-color: var(--jp-layout-color0);
  font-family: var(--jp-ui-font-family);
  padding: 2px 1px;
  resize: none;
}

.jp-DocumentSearch-overlay {
  position: absolute;
  background-color: var(--jp-toolbar-background);
  border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  border-left: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  top: 0;
  right: 0;
  z-index: 7;
  min-width: 405px;
  padding: 2px;
  font-size: var(--jp-ui-font-size1);

  --jp-private-document-search-button-height: 20px;
}

.jp-DocumentSearch-overlay button {
  background-color: var(--jp-toolbar-background);
  outline: 0;
}

.jp-DocumentSearch-overlay button:hover {
  background-color: var(--jp-layout-color2);
}

.jp-DocumentSearch-overlay button:active {
  background-color: var(--jp-layout-color3);
}

.jp-DocumentSearch-overlay-row {
  display: flex;
  align-items: center;
  margin-bottom: 2px;
}

.jp-DocumentSearch-button-content {
  display: inline-block;
  cursor: pointer;
  box-sizing: border-box;
  width: 100%;
  height: 100%;
}

.jp-DocumentSearch-button-content svg {
  width: 100%;
  height: 100%;
}

.jp-DocumentSearch-input-wrapper {
  border: var(--jp-border-width) solid var(--jp-border-color0);
  display: flex;
  background-color: var(--jp-layout-color0);
  margin: 2px;
}

.jp-DocumentSearch-input-wrapper:focus-within {
  border-color: var(--jp-cell-editor-active-border-color);
}

.jp-DocumentSearch-toggle-wrapper,
.jp-DocumentSearch-button-wrapper {
  all: initial;
  overflow: hidden;
  display: inline-block;
  border: none;
  box-sizing: border-box;
}

.jp-DocumentSearch-toggle-wrapper {
  width: 14px;
  height: 14px;
}

.jp-DocumentSearch-button-wrapper {
  width: var(--jp-private-document-search-button-height);
  height: var(--jp-private-document-search-button-height);
}

.jp-DocumentSearch-toggle-wrapper:focus,
.jp-DocumentSearch-button-wrapper:focus {
  outline: var(--jp-border-width) solid
    var(--jp-cell-editor-active-border-color);
  outline-offset: -1px;
}

.jp-DocumentSearch-toggle-wrapper,
.jp-DocumentSearch-button-wrapper,
.jp-DocumentSearch-button-content:focus {
  outline: none;
}

.jp-DocumentSearch-toggle-placeholder {
  width: 5px;
}

.jp-DocumentSearch-input-button::before {
  display: block;
  padding-top: 100%;
}

.jp-DocumentSearch-input-button-off {
  opacity: var(--jp-search-toggle-off-opacity);
}

.jp-DocumentSearch-input-button-off:hover {
  opacity: var(--jp-search-toggle-hover-opacity);
}

.jp-DocumentSearch-input-button-on {
  opacity: var(--jp-search-toggle-on-opacity);
}

.jp-DocumentSearch-index-counter {
  padding-left: 10px;
  padding-right: 10px;
  user-select: none;
  min-width: 35px;
  display: inline-block;
}

.jp-DocumentSearch-up-down-wrapper {
  display: inline-block;
  padding-right: 2px;
  margin-left: auto;
  white-space: nowrap;
}

.jp-DocumentSearch-spacer {
  margin-left: auto;
}

.jp-DocumentSearch-up-down-wrapper button {
  outline: 0;
  border: none;
  width: var(--jp-private-document-search-button-height);
  height: var(--jp-private-document-search-button-height);
  vertical-align: middle;
  margin: 1px 5px 2px;
}

.jp-DocumentSearch-up-down-button:hover {
  background-color: var(--jp-layout-color2);
}

.jp-DocumentSearch-up-down-button:active {
  background-color: var(--jp-layout-color3);
}

.jp-DocumentSearch-filter-button {
  border-radius: var(--jp-border-radius);
}

.jp-DocumentSearch-filter-button:hover {
  background-color: var(--jp-layout-color2);
}

.jp-DocumentSearch-filter-button-enabled {
  background-color: var(--jp-layout-color2);
}

.jp-DocumentSearch-filter-button-enabled:hover {
  background-color: var(--jp-layout-color3);
}

.jp-DocumentSearch-search-options {
  padding: 0 8px;
  margin-left: 3px;
  width: 100%;
  display: grid;
  justify-content: start;
  grid-template-columns: 1fr 1fr;
  align-items: center;
  justify-items: stretch;
}

.jp-DocumentSearch-search-filter-disabled {
  color: var(--jp-ui-font-color2);
}

.jp-DocumentSearch-search-filter {
  display: flex;
  align-items: center;
  user-select: none;
}

.jp-DocumentSearch-regex-error {
  color: var(--jp-error-color0);
}

.jp-DocumentSearch-replace-button-wrapper {
  overflow: hidden;
  display: inline-block;
  box-sizing: border-box;
  border: var(--jp-border-width) solid var(--jp-border-color0);
  margin: auto 2px;
  padding: 1px 4px;
  height: calc(var(--jp-private-document-search-button-height) + 2px);
}

.jp-DocumentSearch-replace-button-wrapper:focus {
  border: var(--jp-border-width) solid var(--jp-cell-editor-active-border-color);
}

.jp-DocumentSearch-replace-button {
  display: inline-block;
  text-align: center;
  cursor: pointer;
  box-sizing: border-box;
  color: var(--jp-ui-font-color1);

  /* height - 2 * (padding of wrapper) */
  line-height: calc(var(--jp-private-document-search-button-height) - 2px);
  width: 100%;
  height: 100%;
}

.jp-DocumentSearch-replace-button:focus {
  outline: none;
}

.jp-DocumentSearch-replace-wrapper-class {
  margin-left: 14px;
  display: flex;
}

.jp-DocumentSearch-replace-toggle {
  border: none;
  background-color: var(--jp-toolbar-background);
  border-radius: var(--jp-border-radius);
}

.jp-DocumentSearch-replace-toggle:hover {
  background-color: var(--jp-layout-color2);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.cm-editor {
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  font-family: var(--jp-code-font-family);
  border: 0;
  border-radius: 0;
  height: auto;

  /* Changed to auto to autogrow */
}

.cm-editor pre {
  padding: 0 var(--jp-code-padding);
}

.jp-CodeMirrorEditor[data-type='inline'] .cm-dialog {
  background-color: var(--jp-layout-color0);
  color: var(--jp-content-font-color1);
}

.jp-CodeMirrorEditor {
  cursor: text;
}

/* When zoomed out 67% and 33% on a screen of 1440 width x 900 height */
@media screen and (min-width: 2138px) and (max-width: 4319px) {
  .jp-CodeMirrorEditor[data-type='inline'] .cm-cursor {
    border-left: var(--jp-code-cursor-width1) solid
      var(--jp-editor-cursor-color);
  }
}

/* When zoomed out less than 33% */
@media screen and (min-width: 4320px) {
  .jp-CodeMirrorEditor[data-type='inline'] .cm-cursor {
    border-left: var(--jp-code-cursor-width2) solid
      var(--jp-editor-cursor-color);
  }
}

.cm-editor.jp-mod-readOnly .cm-cursor {
  display: none;
}

.jp-CollaboratorCursor {
  border-left: 5px solid transparent;
  border-right: 5px solid transparent;
  border-top: none;
  border-bottom: 3px solid;
  background-clip: content-box;
  margin-left: -5px;
  margin-right: -5px;
}

.cm-searching,
.cm-searching span {
  /* `.cm-searching span`: we need to override syntax highlighting */
  background-color: var(--jp-search-unselected-match-background-color);
  color: var(--jp-search-unselected-match-color);
}

.cm-searching::selection,
.cm-searching span::selection {
  background-color: var(--jp-search-unselected-match-background-color);
  color: var(--jp-search-unselected-match-color);
}

.jp-current-match > .cm-searching,
.jp-current-match > .cm-searching span,
.cm-searching > .jp-current-match,
.cm-searching > .jp-current-match span {
  background-color: var(--jp-search-selected-match-background-color);
  color: var(--jp-search-selected-match-color);
}

.jp-current-match > .cm-searching::selection,
.cm-searching > .jp-current-match::selection,
.jp-current-match > .cm-searching span::selection {
  background-color: var(--jp-search-selected-match-background-color);
  color: var(--jp-search-selected-match-color);
}

.cm-trailingspace {
  background-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAgAAAAFCAYAAAB4ka1VAAAAsElEQVQIHQGlAFr/AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA7+r3zKmT0/+pk9P/7+r3zAAAAAAAAAAABAAAAAAAAAAA6OPzM+/q9wAAAAAA6OPzMwAAAAAAAAAAAgAAAAAAAAAAGR8NiRQaCgAZIA0AGR8NiQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAQyoYJ/SY80UAAAAASUVORK5CYII=);
  background-position: center left;
  background-repeat: repeat-x;
}

.jp-CollaboratorCursor-hover {
  position: absolute;
  z-index: 1;
  transform: translateX(-50%);
  color: white;
  border-radius: 3px;
  padding-left: 4px;
  padding-right: 4px;
  padding-top: 1px;
  padding-bottom: 1px;
  text-align: center;
  font-size: var(--jp-ui-font-size1);
  white-space: nowrap;
}

.jp-CodeMirror-ruler {
  border-left: 1px dashed var(--jp-border-color2);
}

/* Styles for shared cursors (remote cursor locations and selected ranges) */
.jp-CodeMirrorEditor .cm-ySelectionCaret {
  position: relative;
  border-left: 1px solid black;
  margin-left: -1px;
  margin-right: -1px;
  box-sizing: border-box;
}

.jp-CodeMirrorEditor .cm-ySelectionCaret > .cm-ySelectionInfo {
  white-space: nowrap;
  position: absolute;
  top: -1.15em;
  padding-bottom: 0.05em;
  left: -1px;
  font-size: 0.95em;
  font-family: var(--jp-ui-font-family);
  font-weight: bold;
  line-height: normal;
  user-select: none;
  color: white;
  padding-left: 2px;
  padding-right: 2px;
  z-index: 101;
  transition: opacity 0.3s ease-in-out;
}

.jp-CodeMirrorEditor .cm-ySelectionInfo {
  transition-delay: 0.7s;
  opacity: 0;
}

.jp-CodeMirrorEditor .cm-ySelectionCaret:hover > .cm-ySelectionInfo {
  opacity: 1;
  transition-delay: 0s;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-MimeDocument {
  outline: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------*/

:root {
  --jp-private-filebrowser-button-height: 28px;
  --jp-private-filebrowser-button-width: 48px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-FileBrowser .jp-SidePanel-content {
  display: flex;
  flex-direction: column;
}

.jp-FileBrowser-toolbar.jp-Toolbar {
  flex-wrap: wrap;
  row-gap: 12px;
  border-bottom: none;
  height: auto;
  margin: 8px 12px 0;
  box-shadow: none;
  padding: 0;
  justify-content: flex-start;
}

.jp-FileBrowser-Panel {
  flex: 1 1 auto;
  display: flex;
  flex-direction: column;
}

.jp-BreadCrumbs {
  flex: 0 0 auto;
  margin: 8px 12px;
}

.jp-BreadCrumbs-item {
  margin: 0 2px;
  padding: 0 2px;
  border-radius: var(--jp-border-radius);
  cursor: pointer;
}

.jp-BreadCrumbs-item:hover {
  background-color: var(--jp-layout-color2);
}

.jp-BreadCrumbs-item:first-child {
  margin-left: 0;
}

.jp-BreadCrumbs-item.jp-mod-dropTarget {
  background-color: var(--jp-brand-color2);
  opacity: 0.7;
}

/*-----------------------------------------------------------------------------
| Buttons
|----------------------------------------------------------------------------*/

.jp-FileBrowser-toolbar > .jp-Toolbar-item {
  flex: 0 0 auto;
  padding-left: 0;
  padding-right: 2px;
  align-items: center;
  height: unset;
}

.jp-FileBrowser-toolbar > .jp-Toolbar-item .jp-ToolbarButtonComponent {
  width: 40px;
}

/*-----------------------------------------------------------------------------
| Other styles
|----------------------------------------------------------------------------*/

.jp-FileDialog.jp-mod-conflict input {
  color: var(--jp-error-color1);
}

.jp-FileDialog .jp-new-name-title {
  margin-top: 12px;
}

.jp-LastModified-hidden {
  display: none;
}

.jp-FileSize-hidden {
  display: none;
}

.jp-FileBrowser .lm-AccordionPanel > h3:first-child {
  display: none;
}

/*-----------------------------------------------------------------------------
| DirListing
|----------------------------------------------------------------------------*/

.jp-DirListing {
  flex: 1 1 auto;
  display: flex;
  flex-direction: column;
  outline: 0;
}

.jp-DirListing-header {
  flex: 0 0 auto;
  display: flex;
  flex-direction: row;
  align-items: center;
  overflow: hidden;
  border-top: var(--jp-border-width) solid var(--jp-border-color2);
  border-bottom: var(--jp-border-width) solid var(--jp-border-color1);
  box-shadow: var(--jp-toolbar-box-shadow);
  z-index: 2;
}

.jp-DirListing-headerItem {
  padding: 4px 12px 2px;
  font-weight: 500;
}

.jp-DirListing-headerItem:hover {
  background: var(--jp-layout-color2);
}

.jp-DirListing-headerItem.jp-id-name {
  flex: 1 0 84px;
}

.jp-DirListing-headerItem.jp-id-modified {
  flex: 0 0 112px;
  border-left: var(--jp-border-width) solid var(--jp-border-color2);
  text-align: right;
}

.jp-DirListing-headerItem.jp-id-filesize {
  flex: 0 0 75px;
  border-left: var(--jp-border-width) solid var(--jp-border-color2);
  text-align: right;
}

.jp-id-narrow {
  display: none;
  flex: 0 0 5px;
  padding: 4px;
  border-left: var(--jp-border-width) solid var(--jp-border-color2);
  text-align: right;
  color: var(--jp-border-color2);
}

.jp-DirListing-narrow .jp-id-narrow {
  display: block;
}

.jp-DirListing-narrow .jp-id-modified,
.jp-DirListing-narrow .jp-DirListing-itemModified {
  display: none;
}

.jp-DirListing-headerItem.jp-mod-selected {
  font-weight: 600;
}

/* increase specificity to override bundled default */
.jp-DirListing-content {
  flex: 1 1 auto;
  margin: 0;
  padding: 0;
  list-style-type: none;
  overflow: auto;
  background-color: var(--jp-layout-color1);
}

.jp-DirListing-content mark {
  color: var(--jp-ui-font-color0);
  background-color: transparent;
  font-weight: bold;
}

.jp-DirListing-content .jp-DirListing-item.jp-mod-selected mark {
  color: var(--jp-ui-inverse-font-color0);
}

/* Style the directory listing content when a user drops a file to upload */
.jp-DirListing.jp-mod-native-drop .jp-DirListing-content {
  outline: 5px dashed rgba(128, 128, 128, 0.5);
  outline-offset: -10px;
  cursor: copy;
}

.jp-DirListing-item {
  display: flex;
  flex-direction: row;
  align-items: center;
  padding: 4px 12px;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.jp-DirListing-checkboxWrapper {
  /* Increases hit area of checkbox. */
  padding: 4px;
}

.jp-DirListing-header
  .jp-DirListing-checkboxWrapper
  + .jp-DirListing-headerItem {
  padding-left: 4px;
}

.jp-DirListing-content .jp-DirListing-checkboxWrapper {
  position: relative;
  left: -4px;
  margin: -4px 0 -4px -8px;
}

.jp-DirListing-checkboxWrapper.jp-mod-visible {
  visibility: visible;
}

/* For devices that support hovering, hide checkboxes until hovered, selected...
*/
@media (hover: hover) {
  .jp-DirListing-checkboxWrapper {
    visibility: hidden;
  }

  .jp-DirListing-item:hover .jp-DirListing-checkboxWrapper,
  .jp-DirListing-item.jp-mod-selected .jp-DirListing-checkboxWrapper {
    visibility: visible;
  }
}

.jp-DirListing-item[data-is-dot] {
  opacity: 75%;
}

.jp-DirListing-item.jp-mod-selected {
  color: var(--jp-ui-inverse-font-color1);
  background: var(--jp-brand-color1);
}

.jp-DirListing-item.jp-mod-dropTarget {
  background: var(--jp-brand-color3);
}

.jp-DirListing-item:hover:not(.jp-mod-selected) {
  background: var(--jp-layout-color2);
}

.jp-DirListing-itemIcon {
  flex: 0 0 20px;
  margin-right: 4px;
}

.jp-DirListing-itemText {
  flex: 1 0 64px;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  user-select: none;
}

.jp-DirListing-itemText:focus {
  outline-width: 2px;
  outline-color: var(--jp-inverse-layout-color1);
  outline-style: solid;
  outline-offset: 1px;
}

.jp-DirListing-item.jp-mod-selected .jp-DirListing-itemText:focus {
  outline-color: var(--jp-layout-color1);
}

.jp-DirListing-itemModified {
  flex: 0 0 125px;
  text-align: right;
}

.jp-DirListing-itemFileSize {
  flex: 0 0 90px;
  text-align: right;
}

.jp-DirListing-editor {
  flex: 1 0 64px;
  outline: none;
  border: none;
  color: var(--jp-ui-font-color1);
  background-color: var(--jp-layout-color1);
}

.jp-DirListing-item.jp-mod-running .jp-DirListing-itemIcon::before {
  color: var(--jp-success-color1);
  content: '\25CF';
  font-size: 8px;
  position: absolute;
  left: -8px;
}

.jp-DirListing-item.jp-mod-running.jp-mod-selected
  .jp-DirListing-itemIcon::before {
  color: var(--jp-ui-inverse-font-color1);
}

.jp-DirListing-item.lm-mod-drag-image,
.jp-DirListing-item.jp-mod-selected.lm-mod-drag-image {
  font-size: var(--jp-ui-font-size1);
  padding-left: 4px;
  margin-left: 4px;
  width: 160px;
  background-color: var(--jp-ui-inverse-font-color2);
  box-shadow: var(--jp-elevation-z2);
  border-radius: 0;
  color: var(--jp-ui-font-color1);
  transform: translateX(-40%) translateY(-58%);
}

.jp-Document {
  min-width: 120px;
  min-height: 120px;
  outline: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Main OutputArea
| OutputArea has a list of Outputs
|----------------------------------------------------------------------------*/

.jp-OutputArea {
  overflow-y: auto;
}

.jp-OutputArea-child {
  display: table;
  table-layout: fixed;
  width: 100%;
  overflow: hidden;
}

.jp-OutputPrompt {
  width: var(--jp-cell-prompt-width);
  color: var(--jp-cell-outprompt-font-color);
  font-family: var(--jp-cell-prompt-font-family);
  padding: var(--jp-code-padding);
  letter-spacing: var(--jp-cell-prompt-letter-spacing);
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  border: var(--jp-border-width) solid transparent;
  opacity: var(--jp-cell-prompt-opacity);

  /* Right align prompt text, don't wrap to handle large prompt numbers */
  text-align: right;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;

  /* Disable text selection */
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.jp-OutputArea-prompt {
  display: table-cell;
  vertical-align: top;
}

.jp-OutputArea-output {
  display: table-cell;
  width: 100%;
  height: auto;
  overflow: auto;
  user-select: text;
  -moz-user-select: text;
  -webkit-user-select: text;
  -ms-user-select: text;
}

.jp-OutputArea .jp-RenderedText {
  padding-left: 1ch;
}

/**
 * Prompt overlay.
 */

.jp-OutputArea-promptOverlay {
  position: absolute;
  top: 0;
  width: var(--jp-cell-prompt-width);
  height: 100%;
  opacity: 0.5;
}

.jp-OutputArea-promptOverlay:hover {
  background: var(--jp-layout-color2);
  box-shadow: inset 0 0 1px var(--jp-inverse-layout-color0);
  cursor: zoom-out;
}

.jp-mod-outputsScrolled .jp-OutputArea-promptOverlay:hover {
  cursor: zoom-in;
}

/**
 * Isolated output.
 */
.jp-OutputArea-output.jp-mod-isolated {
  width: 100%;
  display: block;
}

/*
When drag events occur, `lm-mod-override-cursor` is added to the body.
Because iframes steal all cursor events, the following two rules are necessary
to suppress pointer events while resize drags are occurring. There may be a
better solution to this problem.
*/
body.lm-mod-override-cursor .jp-OutputArea-output.jp-mod-isolated {
  position: relative;
}

body.lm-mod-override-cursor .jp-OutputArea-output.jp-mod-isolated::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: transparent;
}

/* pre */

.jp-OutputArea-output pre {
  border: none;
  margin: 0;
  padding: 0;
  overflow-x: auto;
  overflow-y: auto;
  word-break: break-all;
  word-wrap: break-word;
  white-space: pre-wrap;
}

/* tables */

.jp-OutputArea-output.jp-RenderedHTMLCommon table {
  margin-left: 0;
  margin-right: 0;
}

/* description lists */

.jp-OutputArea-output dl,
.jp-OutputArea-output dt,
.jp-OutputArea-output dd {
  display: block;
}

.jp-OutputArea-output dl {
  width: 100%;
  overflow: hidden;
  padding: 0;
  margin: 0;
}

.jp-OutputArea-output dt {
  font-weight: bold;
  float: left;
  width: 20%;
  padding: 0;
  margin: 0;
}

.jp-OutputArea-output dd {
  float: left;
  width: 80%;
  padding: 0;
  margin: 0;
}

.jp-TrimmedOutputs pre {
  background: var(--jp-layout-color3);
  font-size: calc(var(--jp-code-font-size) * 1.4);
  text-align: center;
  text-transform: uppercase;
}

/* Hide the gutter in case of
 *  - nested output areas (e.g. in the case of output widgets)
 *  - mirrored output areas
 */
.jp-OutputArea .jp-OutputArea .jp-OutputArea-prompt {
  display: none;
}

/* Hide empty lines in the output area, for instance due to cleared widgets */
.jp-OutputArea-prompt:empty {
  padding: 0;
  border: 0;
}

/*-----------------------------------------------------------------------------
| executeResult is added to any Output-result for the display of the object
| returned by a cell
|----------------------------------------------------------------------------*/

.jp-OutputArea-output.jp-OutputArea-executeResult {
  margin-left: 0;
  width: 100%;
}

/* Text output with the Out[] prompt needs a top padding to match the
 * alignment of the Out[] prompt itself.
 */
.jp-OutputArea-executeResult .jp-RenderedText.jp-OutputArea-output {
  padding-top: var(--jp-code-padding);
  border-top: var(--jp-border-width) solid transparent;
}

/*-----------------------------------------------------------------------------
| The Stdin output
|----------------------------------------------------------------------------*/

.jp-Stdin-prompt {
  color: var(--jp-content-font-color0);
  padding-right: var(--jp-code-padding);
  vertical-align: baseline;
  flex: 0 0 auto;
}

.jp-Stdin-input {
  font-family: var(--jp-code-font-family);
  font-size: inherit;
  color: inherit;
  background-color: inherit;
  width: 42%;
  min-width: 200px;

  /* make sure input baseline aligns with prompt */
  vertical-align: baseline;

  /* padding + margin = 0.5em between prompt and cursor */
  padding: 0 0.25em;
  margin: 0 0.25em;
  flex: 0 0 70%;
}

.jp-Stdin-input::placeholder {
  opacity: 0;
}

.jp-Stdin-input:focus {
  box-shadow: none;
}

.jp-Stdin-input:focus::placeholder {
  opacity: 1;
}

/*-----------------------------------------------------------------------------
| Output Area View
|----------------------------------------------------------------------------*/

.jp-LinkedOutputView .jp-OutputArea {
  height: 100%;
  display: block;
}

.jp-LinkedOutputView .jp-OutputArea-output:only-child {
  height: 100%;
}

/*-----------------------------------------------------------------------------
| Printing
|----------------------------------------------------------------------------*/

@media print {
  .jp-OutputArea-child {
    break-inside: avoid-page;
  }
}

/*-----------------------------------------------------------------------------
| Mobile
|----------------------------------------------------------------------------*/
@media only screen and (max-width: 760px) {
  .jp-OutputPrompt {
    display: table-row;
    text-align: left;
  }

  .jp-OutputArea-child .jp-OutputArea-output {
    display: table-row;
    margin-left: var(--jp-notebook-padding);
  }
}

/* Trimmed outputs warning */
.jp-TrimmedOutputs > a {
  margin: 10px;
  text-decoration: none;
  cursor: pointer;
}

.jp-TrimmedOutputs > a:hover {
  text-decoration: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Table of Contents
|----------------------------------------------------------------------------*/

:root {
  --jp-private-toc-active-width: 4px;
}

.jp-TableOfContents {
  display: flex;
  flex-direction: column;
  background: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
  height: 100%;
}

.jp-TableOfContents-placeholder {
  text-align: center;
}

.jp-TableOfContents-placeholderContent {
  color: var(--jp-content-font-color2);
  padding: 8px;
}

.jp-TableOfContents-placeholderContent > h3 {
  margin-bottom: var(--jp-content-heading-margin-bottom);
}

.jp-TableOfContents .jp-SidePanel-content {
  overflow-y: auto;
}

.jp-TableOfContents-tree {
  margin: 4px;
}

.jp-TableOfContents ol {
  list-style-type: none;
}

/* stylelint-disable-next-line selector-max-type */
.jp-TableOfContents li > ol {
  /* Align left border with triangle icon center */
  padding-left: 11px;
}

.jp-TableOfContents-content {
  /* left margin for the active heading indicator */
  margin: 0 0 0 var(--jp-private-toc-active-width);
  padding: 0;
  background-color: var(--jp-layout-color1);
}

.jp-tocItem {
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.jp-tocItem-heading {
  display: flex;
  cursor: pointer;
}

.jp-tocItem-heading:hover {
  background-color: var(--jp-layout-color2);
}

.jp-tocItem-content {
  display: block;
  padding: 4px 0;
  white-space: nowrap;
  text-overflow: ellipsis;
  overflow-x: hidden;
}

.jp-tocItem-collapser {
  height: 20px;
  margin: 2px 2px 0;
  padding: 0;
  background: none;
  border: none;
  cursor: pointer;
}

.jp-tocItem-collapser:hover {
  background-color: var(--jp-layout-color3);
}

/* Active heading indicator */

.jp-tocItem-heading::before {
  content: ' ';
  background: transparent;
  width: var(--jp-private-toc-active-width);
  height: 24px;
  position: absolute;
  left: 0;
  border-radius: var(--jp-border-radius);
}

.jp-tocItem-heading.jp-tocItem-active::before {
  background-color: var(--jp-brand-color1);
}

.jp-tocItem-heading:hover.jp-tocItem-active::before {
  background: var(--jp-brand-color0);
  opacity: 1;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Collapser {
  flex: 0 0 var(--jp-cell-collapser-width);
  padding: 0;
  margin: 0;
  border: none;
  outline: none;
  background: transparent;
  border-radius: var(--jp-border-radius);
  opacity: 1;
}

.jp-Collapser-child {
  display: block;
  width: 100%;
  box-sizing: border-box;

  /* height: 100% doesn't work because the height of its parent is computed from content */
  position: absolute;
  top: 0;
  bottom: 0;
}

/*-----------------------------------------------------------------------------
| Printing
|----------------------------------------------------------------------------*/

/*
Hiding collapsers in print mode.

Note: input and output wrappers have "display: block" propery in print mode.
*/

@media print {
  .jp-Collapser {
    display: none;
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Header/Footer
|----------------------------------------------------------------------------*/

/* Hidden by zero height by default */
.jp-CellHeader,
.jp-CellFooter {
  height: 0;
  width: 100%;
  padding: 0;
  margin: 0;
  border: none;
  outline: none;
  background: transparent;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Input
|----------------------------------------------------------------------------*/

/* All input areas */
.jp-InputArea {
  display: table;
  table-layout: fixed;
  width: 100%;
  overflow: hidden;
}

.jp-InputArea-editor {
  display: table-cell;
  overflow: hidden;
  vertical-align: top;

  /* This is the non-active, default styling */
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  border-radius: 0;
  background: var(--jp-cell-editor-background);
}

.jp-InputPrompt {
  display: table-cell;
  vertical-align: top;
  width: var(--jp-cell-prompt-width);
  color: var(--jp-cell-inprompt-font-color);
  font-family: var(--jp-cell-prompt-font-family);
  padding: var(--jp-code-padding);
  letter-spacing: var(--jp-cell-prompt-letter-spacing);
  opacity: var(--jp-cell-prompt-opacity);
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  border: var(--jp-border-width) solid transparent;

  /* Right align prompt text, don't wrap to handle large prompt numbers */
  text-align: right;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;

  /* Disable text selection */
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

/*-----------------------------------------------------------------------------
| Mobile
|----------------------------------------------------------------------------*/
@media only screen and (max-width: 760px) {
  .jp-InputArea-editor {
    display: table-row;
    margin-left: var(--jp-notebook-padding);
  }

  .jp-InputPrompt {
    display: table-row;
    text-align: left;
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Placeholder
|----------------------------------------------------------------------------*/

.jp-Placeholder {
  display: table;
  table-layout: fixed;
  width: 100%;
}

.jp-Placeholder-prompt {
  display: table-cell;
  box-sizing: border-box;
}

.jp-Placeholder-content {
  display: table-cell;
  padding: 4px 6px;
  border: 1px solid transparent;
  border-radius: 0;
  background: none;
  box-sizing: border-box;
  cursor: pointer;
}

.jp-Placeholder-contentContainer {
  display: flex;
}

.jp-Placeholder-content:hover,
.jp-InputPlaceholder > .jp-Placeholder-content:hover {
  border-color: var(--jp-layout-color3);
}

.jp-Placeholder-content .jp-MoreHorizIcon {
  width: 32px;
  height: 16px;
  border: 1px solid transparent;
  border-radius: var(--jp-border-radius);
}

.jp-Placeholder-content .jp-MoreHorizIcon:hover {
  border: 1px solid var(--jp-border-color1);
  box-shadow: 0 0 2px 0 rgba(0, 0, 0, 0.25);
  background-color: var(--jp-layout-color0);
}

.jp-PlaceholderText {
  white-space: nowrap;
  overflow-x: hidden;
  color: var(--jp-inverse-layout-color3);
  font-family: var(--jp-code-font-family);
}

.jp-InputPlaceholder > .jp-Placeholder-content {
  border-color: var(--jp-cell-editor-border-color);
  background: var(--jp-cell-editor-background);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Private CSS variables
|----------------------------------------------------------------------------*/

:root {
  --jp-private-cell-scrolling-output-offset: 5px;
}

/*-----------------------------------------------------------------------------
| Cell
|----------------------------------------------------------------------------*/

.jp-Cell {
  padding: var(--jp-cell-padding);
  margin: 0;
  border: none;
  outline: none;
  background: transparent;
}

/*-----------------------------------------------------------------------------
| Common input/output
|----------------------------------------------------------------------------*/

.jp-Cell-inputWrapper,
.jp-Cell-outputWrapper {
  display: flex;
  flex-direction: row;
  padding: 0;
  margin: 0;

  /* Added to reveal the box-shadow on the input and output collapsers. */
  overflow: visible;
}

/* Only input/output areas inside cells */
.jp-Cell-inputArea,
.jp-Cell-outputArea {
  flex: 1 1 auto;
}

/*-----------------------------------------------------------------------------
| Collapser
|----------------------------------------------------------------------------*/

/* Make the output collapser disappear when there is not output, but do so
 * in a manner that leaves it in the layout and preserves its width.
 */
.jp-Cell.jp-mod-noOutputs .jp-Cell-outputCollapser {
  border: none !important;
  background: transparent !important;
}

.jp-Cell:not(.jp-mod-noOutputs) .jp-Cell-outputCollapser {
  min-height: var(--jp-cell-collapser-min-height);
}

/*-----------------------------------------------------------------------------
| Output
|----------------------------------------------------------------------------*/

/* Put a space between input and output when there IS output */
.jp-Cell:not(.jp-mod-noOutputs) .jp-Cell-outputWrapper {
  margin-top: 5px;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-Cell-outputArea {
  overflow-y: auto;
  max-height: 24em;
  margin-left: var(--jp-private-cell-scrolling-output-offset);
  resize: vertical;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-Cell-outputArea[style*='height'] {
  max-height: unset;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-Cell-outputArea::after {
  content: ' ';
  box-shadow: inset 0 0 6px 2px rgb(0 0 0 / 30%);
  width: 100%;
  height: 100%;
  position: sticky;
  bottom: 0;
  top: 0;
  margin-top: -50%;
  float: left;
  display: block;
  pointer-events: none;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-child {
  padding-top: 6px;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-prompt {
  width: calc(
    var(--jp-cell-prompt-width) - var(--jp-private-cell-scrolling-output-offset)
  );
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-promptOverlay {
  left: calc(-1 * var(--jp-private-cell-scrolling-output-offset));
}

/*-----------------------------------------------------------------------------
| CodeCell
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| MarkdownCell
|----------------------------------------------------------------------------*/

.jp-MarkdownOutput {
  display: table-cell;
  width: 100%;
  margin-top: 0;
  margin-bottom: 0;
  padding-left: var(--jp-code-padding);
}

.jp-MarkdownOutput.jp-RenderedHTMLCommon {
  overflow: auto;
}

/* collapseHeadingButton (show always if hiddenCellsButton is _not_ shown) */
.jp-collapseHeadingButton {
  display: flex;
  min-height: var(--jp-cell-collapser-min-height);
  font-size: var(--jp-code-font-size);
  position: absolute;
  background-color: transparent;
  background-size: 25px;
  background-repeat: no-repeat;
  background-position-x: center;
  background-position-y: top;
  background-image: var(--jp-icon-caret-down);
  right: 0;
  top: 0;
  bottom: 0;
}

.jp-collapseHeadingButton.jp-mod-collapsed {
  background-image: var(--jp-icon-caret-right);
}

/*
 set the container font size to match that of content
 so that the nested collapse buttons have the right size
*/
.jp-MarkdownCell .jp-InputPrompt {
  font-size: var(--jp-content-font-size1);
}

/*
  Align collapseHeadingButton with cell top header
  The font sizes are identical to the ones in packages/rendermime/style/base.css
*/
.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='1'] {
  font-size: var(--jp-content-font-size5);
  background-position-y: calc(0.3 * var(--jp-content-font-size5));
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='2'] {
  font-size: var(--jp-content-font-size4);
  background-position-y: calc(0.3 * var(--jp-content-font-size4));
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='3'] {
  font-size: var(--jp-content-font-size3);
  background-position-y: calc(0.3 * var(--jp-content-font-size3));
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='4'] {
  font-size: var(--jp-content-font-size2);
  background-position-y: calc(0.3 * var(--jp-content-font-size2));
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='5'] {
  font-size: var(--jp-content-font-size1);
  background-position-y: top;
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='6'] {
  font-size: var(--jp-content-font-size0);
  background-position-y: top;
}

/* collapseHeadingButton (show only on (hover,active) if hiddenCellsButton is shown) */
.jp-Notebook.jp-mod-showHiddenCellsButton .jp-collapseHeadingButton {
  display: none;
}

.jp-Notebook.jp-mod-showHiddenCellsButton
  :is(.jp-MarkdownCell:hover, .jp-mod-active)
  .jp-collapseHeadingButton {
  display: flex;
}

/* showHiddenCellsButton (only show if jp-mod-showHiddenCellsButton is set, which
is a consequence of the showHiddenCellsButton option in Notebook Settings)*/
.jp-Notebook.jp-mod-showHiddenCellsButton .jp-showHiddenCellsButton {
  margin-left: calc(var(--jp-cell-prompt-width) + 2 * var(--jp-code-padding));
  margin-top: var(--jp-code-padding);
  border: 1px solid var(--jp-border-color2);
  background-color: var(--jp-border-color3) !important;
  color: var(--jp-content-font-color0) !important;
  display: flex;
}

.jp-Notebook.jp-mod-showHiddenCellsButton .jp-showHiddenCellsButton:hover {
  background-color: var(--jp-border-color2) !important;
}

.jp-showHiddenCellsButton {
  display: none;
}

/*-----------------------------------------------------------------------------
| Printing
|----------------------------------------------------------------------------*/

/*
Using block instead of flex to allow the use of the break-inside CSS property for
cell outputs.
*/

@media print {
  .jp-Cell-inputWrapper,
  .jp-Cell-outputWrapper {
    display: block;
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------*/

:root {
  --jp-notebook-toolbar-padding: 2px 5px 2px 2px;
}

/*-----------------------------------------------------------------------------

/*-----------------------------------------------------------------------------
| Styles
|----------------------------------------------------------------------------*/

.jp-NotebookPanel-toolbar {
  padding: var(--jp-notebook-toolbar-padding);

  /* disable paint containment from lumino 2.0 default strict CSS containment */
  contain: style size !important;
}

.jp-Toolbar-item.jp-Notebook-toolbarCellType .jp-select-wrapper.jp-mod-focused {
  border: none;
  box-shadow: none;
}

.jp-Notebook-toolbarCellTypeDropdown select {
  height: 24px;
  font-size: var(--jp-ui-font-size1);
  line-height: 14px;
  border-radius: 0;
  display: block;
}

.jp-Notebook-toolbarCellTypeDropdown span {
  top: 5px !important;
}

.jp-Toolbar-responsive-popup {
  position: absolute;
  height: fit-content;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: flex-end;
  border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  box-shadow: var(--jp-toolbar-box-shadow);
  background: var(--jp-toolbar-background);
  min-height: var(--jp-toolbar-micro-height);
  padding: var(--jp-notebook-toolbar-padding);
  z-index: 1;
  right: 0;
  top: 0;
}

.jp-Toolbar > .jp-Toolbar-responsive-opener {
  margin-left: auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------

/*-----------------------------------------------------------------------------
| Styles
|----------------------------------------------------------------------------*/

.jp-Notebook-ExecutionIndicator {
  position: relative;
  display: inline-block;
  height: 100%;
  z-index: 9997;
}

.jp-Notebook-ExecutionIndicator-tooltip {
  visibility: hidden;
  height: auto;
  width: max-content;
  width: -moz-max-content;
  background-color: var(--jp-layout-color2);
  color: var(--jp-ui-font-color1);
  text-align: justify;
  border-radius: 6px;
  padding: 0 5px;
  position: fixed;
  display: table;
}

.jp-Notebook-ExecutionIndicator-tooltip.up {
  transform: translateX(-50%) translateY(-100%) translateY(-32px);
}

.jp-Notebook-ExecutionIndicator-tooltip.down {
  transform: translateX(calc(-100% + 16px)) translateY(5px);
}

.jp-Notebook-ExecutionIndicator-tooltip.hidden {
  display: none;
}

.jp-Notebook-ExecutionIndicator:hover .jp-Notebook-ExecutionIndicator-tooltip {
  visibility: visible;
}

.jp-Notebook-ExecutionIndicator span {
  font-size: var(--jp-ui-font-size1);
  font-family: var(--jp-ui-font-family);
  color: var(--jp-ui-font-color1);
  line-height: 24px;
  display: block;
}

.jp-Notebook-ExecutionIndicator-progress-bar {
  display: flex;
  justify-content: center;
  height: 100%;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*
 * Execution indicator
 */
.jp-tocItem-content::after {
  content: '';

  /* Must be identical to form a circle */
  width: 12px;
  height: 12px;
  background: none;
  border: none;
  position: absolute;
  right: 0;
}

.jp-tocItem-content[data-running='0']::after {
  border-radius: 50%;
  border: var(--jp-border-width) solid var(--jp-inverse-layout-color3);
  background: none;
}

.jp-tocItem-content[data-running='1']::after {
  border-radius: 50%;
  border: var(--jp-border-width) solid var(--jp-inverse-layout-color3);
  background-color: var(--jp-inverse-layout-color3);
}

.jp-tocItem-content[data-running='0'],
.jp-tocItem-content[data-running='1'] {
  margin-right: 12px;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-Notebook-footer {
  height: 27px;
  margin-left: calc(
    var(--jp-cell-prompt-width) + var(--jp-cell-collapser-width) +
      var(--jp-cell-padding)
  );
  width: calc(
    100% -
      (
        var(--jp-cell-prompt-width) + var(--jp-cell-collapser-width) +
          var(--jp-cell-padding) + var(--jp-cell-padding)
      )
  );
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  color: var(--jp-ui-font-color3);
  margin-top: 6px;
  background: none;
  cursor: pointer;
}

.jp-Notebook-footer:focus {
  border-color: var(--jp-cell-editor-active-border-color);
}

/* For devices that support hovering, hide footer until hover */
@media (hover: hover) {
  .jp-Notebook-footer {
    opacity: 0;
  }

  .jp-Notebook-footer:focus,
  .jp-Notebook-footer:hover {
    opacity: 1;
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Imports
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| CSS variables
|----------------------------------------------------------------------------*/

:root {
  --jp-side-by-side-output-size: 1fr;
  --jp-side-by-side-resized-cell: var(--jp-side-by-side-output-size);
  --jp-private-notebook-dragImage-width: 304px;
  --jp-private-notebook-dragImage-height: 36px;
  --jp-private-notebook-selected-color: var(--md-blue-400);
  --jp-private-notebook-active-color: var(--md-green-400);
}

/*-----------------------------------------------------------------------------
| Notebook
|----------------------------------------------------------------------------*/

/* stylelint-disable selector-max-class */

.jp-NotebookPanel {
  display: block;
  height: 100%;
}

.jp-NotebookPanel.jp-Document {
  min-width: 240px;
  min-height: 120px;
}

.jp-Notebook {
  padding: var(--jp-notebook-padding);
  outline: none;
  overflow: auto;
  background: var(--jp-layout-color0);
}

.jp-Notebook.jp-mod-scrollPastEnd::after {
  display: block;
  content: '';
  min-height: var(--jp-notebook-scroll-padding);
}

.jp-MainAreaWidget-ContainStrict .jp-Notebook * {
  contain: strict;
}

.jp-Notebook .jp-Cell {
  overflow: visible;
}

.jp-Notebook .jp-Cell .jp-InputPrompt {
  cursor: move;
}

/*-----------------------------------------------------------------------------
| Notebook state related styling
|
| The notebook and cells each have states, here are the possibilities:
|
| - Notebook
|   - Command
|   - Edit
| - Cell
|   - None
|   - Active (only one can be active)
|   - Selected (the cells actions are applied to)
|   - Multiselected (when multiple selected, the cursor)
|   - No outputs
|----------------------------------------------------------------------------*/

/* Command or edit modes */

.jp-Notebook .jp-Cell:not(.jp-mod-active) .jp-InputPrompt {
  opacity: var(--jp-cell-prompt-not-active-opacity);
  color: var(--jp-cell-prompt-not-active-font-color);
}

.jp-Notebook .jp-Cell:not(.jp-mod-active) .jp-OutputPrompt {
  opacity: var(--jp-cell-prompt-not-active-opacity);
  color: var(--jp-cell-prompt-not-active-font-color);
}

/* cell is active */
.jp-Notebook .jp-Cell.jp-mod-active .jp-Collapser {
  background: var(--jp-brand-color1);
}

/* cell is dirty */
.jp-Notebook .jp-Cell.jp-mod-dirty .jp-InputPrompt {
  color: var(--jp-warn-color1);
}

.jp-Notebook .jp-Cell.jp-mod-dirty .jp-InputPrompt::before {
  color: var(--jp-warn-color1);
  content: '•';
}

.jp-Notebook .jp-Cell.jp-mod-active.jp-mod-dirty .jp-Collapser {
  background: var(--jp-warn-color1);
}

/* collapser is hovered */
.jp-Notebook .jp-Cell .jp-Collapser:hover {
  box-shadow: var(--jp-elevation-z2);
  background: var(--jp-brand-color1);
  opacity: var(--jp-cell-collapser-not-active-hover-opacity);
}

/* cell is active and collapser is hovered */
.jp-Notebook .jp-Cell.jp-mod-active .jp-Collapser:hover {
  background: var(--jp-brand-color0);
  opacity: 1;
}

/* Command mode */

.jp-Notebook.jp-mod-commandMode .jp-Cell.jp-mod-selected {
  background: var(--jp-notebook-multiselected-color);
}

.jp-Notebook.jp-mod-commandMode
  .jp-Cell.jp-mod-active.jp-mod-selected:not(.jp-mod-multiSelected) {
  background: transparent;
}

/* Edit mode */

.jp-Notebook.jp-mod-editMode .jp-Cell.jp-mod-active .jp-InputArea-editor {
  border: var(--jp-border-width) solid var(--jp-cell-editor-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
  background-color: var(--jp-cell-editor-active-background);
}

/*-----------------------------------------------------------------------------
| Notebook drag and drop
|----------------------------------------------------------------------------*/

.jp-Notebook-cell.jp-mod-dropSource {
  opacity: 0.5;
}

.jp-Notebook-cell.jp-mod-dropTarget,
.jp-Notebook.jp-mod-commandMode
  .jp-Notebook-cell.jp-mod-active.jp-mod-selected.jp-mod-dropTarget {
  border-top-color: var(--jp-private-notebook-selected-color);
  border-top-style: solid;
  border-top-width: 2px;
}

.jp-dragImage {
  display: block;
  flex-direction: row;
  width: var(--jp-private-notebook-dragImage-width);
  height: var(--jp-private-notebook-dragImage-height);
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  background: var(--jp-cell-editor-background);
  overflow: visible;
}

.jp-dragImage-singlePrompt {
  box-shadow: 2px 2px 4px 0 rgba(0, 0, 0, 0.12);
}

.jp-dragImage .jp-dragImage-content {
  flex: 1 1 auto;
  z-index: 2;
  font-size: var(--jp-code-font-size);
  font-family: var(--jp-code-font-family);
  line-height: var(--jp-code-line-height);
  padding: var(--jp-code-padding);
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  background: var(--jp-cell-editor-background-color);
  color: var(--jp-content-font-color3);
  text-align: left;
  margin: 4px 4px 4px 0;
}

.jp-dragImage .jp-dragImage-prompt {
  flex: 0 0 auto;
  min-width: 36px;
  color: var(--jp-cell-inprompt-font-color);
  padding: var(--jp-code-padding);
  padding-left: 12px;
  font-family: var(--jp-cell-prompt-font-family);
  letter-spacing: var(--jp-cell-prompt-letter-spacing);
  line-height: 1.9;
  font-size: var(--jp-code-font-size);
  border: var(--jp-border-width) solid transparent;
}

.jp-dragImage-multipleBack {
  z-index: -1;
  position: absolute;
  height: 32px;
  width: 300px;
  top: 8px;
  left: 8px;
  background: var(--jp-layout-color2);
  border: var(--jp-border-width) solid var(--jp-input-border-color);
  box-shadow: 2px 2px 4px 0 rgba(0, 0, 0, 0.12);
}

/*-----------------------------------------------------------------------------
| Cell toolbar
|----------------------------------------------------------------------------*/

.jp-NotebookTools {
  display: block;
  min-width: var(--jp-sidebar-min-width);
  color: var(--jp-ui-font-color1);
  background: var(--jp-layout-color1);

  /* This is needed so that all font sizing of children done in ems is
    * relative to this base size */
  font-size: var(--jp-ui-font-size1);
  overflow: auto;
}

.jp-ActiveCellTool {
  padding: 12px 0;
  display: flex;
}

.jp-ActiveCellTool-Content {
  flex: 1 1 auto;
}

.jp-ActiveCellTool .jp-ActiveCellTool-CellContent {
  background: var(--jp-cell-editor-background);
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  border-radius: 0;
  min-height: 29px;
}

.jp-ActiveCellTool .jp-InputPrompt {
  min-width: calc(var(--jp-cell-prompt-width) * 0.75);
}

.jp-ActiveCellTool-CellContent > pre {
  padding: 5px 4px;
  margin: 0;
  white-space: normal;
}

.jp-MetadataEditorTool {
  flex-direction: column;
  padding: 12px 0;
}

.jp-RankedPanel > :not(:first-child) {
  margin-top: 12px;
}

.jp-KeySelector select.jp-mod-styled {
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color0);
  border: var(--jp-border-width) solid var(--jp-border-color1);
}

.jp-KeySelector label,
.jp-MetadataEditorTool label,
.jp-NumberSetter label {
  line-height: 1.4;
}

.jp-NotebookTools .jp-select-wrapper {
  margin-top: 4px;
  margin-bottom: 0;
}

.jp-NumberSetter input {
  width: 100%;
  margin-top: 4px;
}

.jp-NotebookTools .jp-Collapse {
  margin-top: 16px;
}

/*-----------------------------------------------------------------------------
| Presentation Mode (.jp-mod-presentationMode)
|----------------------------------------------------------------------------*/

.jp-mod-presentationMode .jp-Notebook {
  --jp-content-font-size1: var(--jp-content-presentation-font-size1);
  --jp-code-font-size: var(--jp-code-presentation-font-size);
}

.jp-mod-presentationMode .jp-Notebook .jp-Cell .jp-InputPrompt,
.jp-mod-presentationMode .jp-Notebook .jp-Cell .jp-OutputPrompt {
  flex: 0 0 110px;
}

/*-----------------------------------------------------------------------------
| Side-by-side Mode (.jp-mod-sideBySide)
|----------------------------------------------------------------------------*/
.jp-mod-sideBySide.jp-Notebook .jp-Notebook-cell {
  margin-top: 3em;
  margin-bottom: 3em;
  margin-left: 5%;
  margin-right: 5%;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell {
  display: grid;
  grid-template-columns: minmax(0, 1fr) min-content minmax(
      0,
      var(--jp-side-by-side-output-size)
    );
  grid-template-rows: auto minmax(0, 1fr) auto;
  grid-template-areas:
    'header header header'
    'input handle output'
    'footer footer footer';
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell.jp-mod-resizedCell {
  grid-template-columns: minmax(0, 1fr) min-content minmax(
      0,
      var(--jp-side-by-side-resized-cell)
    );
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-CellHeader {
  grid-area: header;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-Cell-inputWrapper {
  grid-area: input;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-Cell-outputWrapper {
  /* overwrite the default margin (no vertical separation needed in side by side move */
  margin-top: 0;
  grid-area: output;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-CellFooter {
  grid-area: footer;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-CellResizeHandle {
  grid-area: handle;
  user-select: none;
  display: block;
  height: 100%;
  cursor: ew-resize;
  padding: 0 var(--jp-cell-padding);
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-CellResizeHandle::after {
  content: '';
  display: block;
  background: var(--jp-border-color2);
  height: 100%;
  width: 5px;
}

.jp-mod-sideBySide.jp-Notebook
  .jp-CodeCell.jp-mod-resizedCell
  .jp-CellResizeHandle::after {
  background: var(--jp-border-color0);
}

.jp-CellResizeHandle {
  display: none;
}

/*-----------------------------------------------------------------------------
| Placeholder
|----------------------------------------------------------------------------*/

.jp-Cell-Placeholder {
  padding-left: 55px;
}

.jp-Cell-Placeholder-wrapper {
  background: #fff;
  border: 1px solid;
  border-color: #e5e6e9 #dfe0e4 #d0d1d5;
  border-radius: 4px;
  -webkit-border-radius: 4px;
  margin: 10px 15px;
}

.jp-Cell-Placeholder-wrapper-inner {
  padding: 15px;
  position: relative;
}

.jp-Cell-Placeholder-wrapper-body {
  background-repeat: repeat;
  background-size: 50% auto;
}

.jp-Cell-Placeholder-wrapper-body div {
  background: #f6f7f8;
  background-image: -webkit-linear-gradient(
    left,
    #f6f7f8 0%,
    #edeef1 20%,
    #f6f7f8 40%,
    #f6f7f8 100%
  );
  background-repeat: no-repeat;
  background-size: 800px 104px;
  height: 104px;
  position: absolute;
  right: 15px;
  left: 15px;
  top: 15px;
}

div.jp-Cell-Placeholder-h1 {
  top: 20px;
  height: 20px;
  left: 15px;
  width: 150px;
}

div.jp-Cell-Placeholder-h2 {
  left: 15px;
  top: 50px;
  height: 10px;
  width: 100px;
}

div.jp-Cell-Placeholder-content-1,
div.jp-Cell-Placeholder-content-2,
div.jp-Cell-Placeholder-content-3 {
  left: 15px;
  right: 15px;
  height: 10px;
}

div.jp-Cell-Placeholder-content-1 {
  top: 100px;
}

div.jp-Cell-Placeholder-content-2 {
  top: 120px;
}

div.jp-Cell-Placeholder-content-3 {
  top: 140px;
}

</style>
<style type="text/css">
/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*
The following CSS variables define the main, public API for styling JupyterLab.
These variables should be used by all plugins wherever possible. In other
words, plugins should not define custom colors, sizes, etc unless absolutely
necessary. This enables users to change the visual theme of JupyterLab
by changing these variables.

Many variables appear in an ordered sequence (0,1,2,3). These sequences
are designed to work well together, so for example, `--jp-border-color1` should
be used with `--jp-layout-color1`. The numbers have the following meanings:

* 0: super-primary, reserved for special emphasis
* 1: primary, most important under normal situations
* 2: secondary, next most important under normal situations
* 3: tertiary, next most important under normal situations

Throughout JupyterLab, we are mostly following principles from Google's
Material Design when selecting colors. We are not, however, following
all of MD as it is not optimized for dense, information rich UIs.
*/

:root {
  /* Elevation
   *
   * We style box-shadows using Material Design's idea of elevation. These particular numbers are taken from here:
   *
   * https://github.com/material-components/material-components-web
   * https://material-components-web.appspot.com/elevation.html
   */

  --jp-shadow-base-lightness: 0;
  --jp-shadow-umbra-color: rgba(
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    0.2
  );
  --jp-shadow-penumbra-color: rgba(
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    0.14
  );
  --jp-shadow-ambient-color: rgba(
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    0.12
  );
  --jp-elevation-z0: none;
  --jp-elevation-z1: 0 2px 1px -1px var(--jp-shadow-umbra-color),
    0 1px 1px 0 var(--jp-shadow-penumbra-color),
    0 1px 3px 0 var(--jp-shadow-ambient-color);
  --jp-elevation-z2: 0 3px 1px -2px var(--jp-shadow-umbra-color),
    0 2px 2px 0 var(--jp-shadow-penumbra-color),
    0 1px 5px 0 var(--jp-shadow-ambient-color);
  --jp-elevation-z4: 0 2px 4px -1px var(--jp-shadow-umbra-color),
    0 4px 5px 0 var(--jp-shadow-penumbra-color),
    0 1px 10px 0 var(--jp-shadow-ambient-color);
  --jp-elevation-z6: 0 3px 5px -1px var(--jp-shadow-umbra-color),
    0 6px 10px 0 var(--jp-shadow-penumbra-color),
    0 1px 18px 0 var(--jp-shadow-ambient-color);
  --jp-elevation-z8: 0 5px 5px -3px var(--jp-shadow-umbra-color),
    0 8px 10px 1px var(--jp-shadow-penumbra-color),
    0 3px 14px 2px var(--jp-shadow-ambient-color);
  --jp-elevation-z12: 0 7px 8px -4px var(--jp-shadow-umbra-color),
    0 12px 17px 2px var(--jp-shadow-penumbra-color),
    0 5px 22px 4px var(--jp-shadow-ambient-color);
  --jp-elevation-z16: 0 8px 10px -5px var(--jp-shadow-umbra-color),
    0 16px 24px 2px var(--jp-shadow-penumbra-color),
    0 6px 30px 5px var(--jp-shadow-ambient-color);
  --jp-elevation-z20: 0 10px 13px -6px var(--jp-shadow-umbra-color),
    0 20px 31px 3px var(--jp-shadow-penumbra-color),
    0 8px 38px 7px var(--jp-shadow-ambient-color);
  --jp-elevation-z24: 0 11px 15px -7px var(--jp-shadow-umbra-color),
    0 24px 38px 3px var(--jp-shadow-penumbra-color),
    0 9px 46px 8px var(--jp-shadow-ambient-color);

  /* Borders
   *
   * The following variables, specify the visual styling of borders in JupyterLab.
   */

  --jp-border-width: 1px;
  --jp-border-color0: var(--md-grey-400);
  --jp-border-color1: var(--md-grey-400);
  --jp-border-color2: var(--md-grey-300);
  --jp-border-color3: var(--md-grey-200);
  --jp-inverse-border-color: var(--md-grey-600);
  --jp-border-radius: 2px;

  /* UI Fonts
   *
   * The UI font CSS variables are used for the typography all of the JupyterLab
   * user interface elements that are not directly user generated content.
   *
   * The font sizing here is done assuming that the body font size of --jp-ui-font-size1
   * is applied to a parent element. When children elements, such as headings, are sized
   * in em all things will be computed relative to that body size.
   */

  --jp-ui-font-scale-factor: 1.2;
  --jp-ui-font-size0: 0.83333em;
  --jp-ui-font-size1: 13px; /* Base font size */
  --jp-ui-font-size2: 1.2em;
  --jp-ui-font-size3: 1.44em;
  --jp-ui-font-family: system-ui, -apple-system, blinkmacsystemfont, 'Segoe UI',
    helvetica, arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
    'Segoe UI Symbol';

  /*
   * Use these font colors against the corresponding main layout colors.
   * In a light theme, these go from dark to light.
   */

  /* Defaults use Material Design specification */
  --jp-ui-font-color0: rgba(0, 0, 0, 1);
  --jp-ui-font-color1: rgba(0, 0, 0, 0.87);
  --jp-ui-font-color2: rgba(0, 0, 0, 0.54);
  --jp-ui-font-color3: rgba(0, 0, 0, 0.38);

  /*
   * Use these against the brand/accent/warn/error colors.
   * These will typically go from light to darker, in both a dark and light theme.
   */

  --jp-ui-inverse-font-color0: rgba(255, 255, 255, 1);
  --jp-ui-inverse-font-color1: rgba(255, 255, 255, 1);
  --jp-ui-inverse-font-color2: rgba(255, 255, 255, 0.7);
  --jp-ui-inverse-font-color3: rgba(255, 255, 255, 0.5);

  /* Content Fonts
   *
   * Content font variables are used for typography of user generated content.
   *
   * The font sizing here is done assuming that the body font size of --jp-content-font-size1
   * is applied to a parent element. When children elements, such as headings, are sized
   * in em all things will be computed relative to that body size.
   */

  --jp-content-line-height: 1.6;
  --jp-content-font-scale-factor: 1.2;
  --jp-content-font-size0: 0.83333em;
  --jp-content-font-size1: 14px; /* Base font size */
  --jp-content-font-size2: 1.2em;
  --jp-content-font-size3: 1.44em;
  --jp-content-font-size4: 1.728em;
  --jp-content-font-size5: 2.0736em;

  /* This gives a magnification of about 125% in presentation mode over normal. */
  --jp-content-presentation-font-size1: 17px;
  --jp-content-heading-line-height: 1;
  --jp-content-heading-margin-top: 1.2em;
  --jp-content-heading-margin-bottom: 0.8em;
  --jp-content-heading-font-weight: 500;

  /* Defaults use Material Design specification */
  --jp-content-font-color0: rgba(0, 0, 0, 1);
  --jp-content-font-color1: rgba(0, 0, 0, 0.87);
  --jp-content-font-color2: rgba(0, 0, 0, 0.54);
  --jp-content-font-color3: rgba(0, 0, 0, 0.38);
  --jp-content-link-color: var(--md-blue-900);
  --jp-content-font-family: system-ui, -apple-system, blinkmacsystemfont,
    'Segoe UI', helvetica, arial, sans-serif, 'Apple Color Emoji',
    'Segoe UI Emoji', 'Segoe UI Symbol';

  /*
   * Code Fonts
   *
   * Code font variables are used for typography of code and other monospaces content.
   */

  --jp-code-font-size: 13px;
  --jp-code-line-height: 1.3077; /* 17px for 13px base */
  --jp-code-padding: 5px; /* 5px for 13px base, codemirror highlighting needs integer px value */
  --jp-code-font-family-default: menlo, consolas, 'DejaVu Sans Mono', monospace;
  --jp-code-font-family: var(--jp-code-font-family-default);

  /* This gives a magnification of about 125% in presentation mode over normal. */
  --jp-code-presentation-font-size: 16px;

  /* may need to tweak cursor width if you change font size */
  --jp-code-cursor-width0: 1.4px;
  --jp-code-cursor-width1: 2px;
  --jp-code-cursor-width2: 4px;

  /* Layout
   *
   * The following are the main layout colors use in JupyterLab. In a light
   * theme these would go from light to dark.
   */

  --jp-layout-color0: white;
  --jp-layout-color1: white;
  --jp-layout-color2: var(--md-grey-200);
  --jp-layout-color3: var(--md-grey-400);
  --jp-layout-color4: var(--md-grey-600);

  /* Inverse Layout
   *
   * The following are the inverse layout colors use in JupyterLab. In a light
   * theme these would go from dark to light.
   */

  --jp-inverse-layout-color0: #111;
  --jp-inverse-layout-color1: var(--md-grey-900);
  --jp-inverse-layout-color2: var(--md-grey-800);
  --jp-inverse-layout-color3: var(--md-grey-700);
  --jp-inverse-layout-color4: var(--md-grey-600);

  /* Brand/accent */

  --jp-brand-color0: var(--md-blue-900);
  --jp-brand-color1: var(--md-blue-700);
  --jp-brand-color2: var(--md-blue-300);
  --jp-brand-color3: var(--md-blue-100);
  --jp-brand-color4: var(--md-blue-50);
  --jp-accent-color0: var(--md-green-900);
  --jp-accent-color1: var(--md-green-700);
  --jp-accent-color2: var(--md-green-300);
  --jp-accent-color3: var(--md-green-100);

  /* State colors (warn, error, success, info) */

  --jp-warn-color0: var(--md-orange-900);
  --jp-warn-color1: var(--md-orange-700);
  --jp-warn-color2: var(--md-orange-300);
  --jp-warn-color3: var(--md-orange-100);
  --jp-error-color0: var(--md-red-900);
  --jp-error-color1: var(--md-red-700);
  --jp-error-color2: var(--md-red-300);
  --jp-error-color3: var(--md-red-100);
  --jp-success-color0: var(--md-green-900);
  --jp-success-color1: var(--md-green-700);
  --jp-success-color2: var(--md-green-300);
  --jp-success-color3: var(--md-green-100);
  --jp-info-color0: var(--md-cyan-900);
  --jp-info-color1: var(--md-cyan-700);
  --jp-info-color2: var(--md-cyan-300);
  --jp-info-color3: var(--md-cyan-100);

  /* Cell specific styles */

  --jp-cell-padding: 5px;
  --jp-cell-collapser-width: 8px;
  --jp-cell-collapser-min-height: 20px;
  --jp-cell-collapser-not-active-hover-opacity: 0.6;
  --jp-cell-editor-background: var(--md-grey-100);
  --jp-cell-editor-border-color: var(--md-grey-300);
  --jp-cell-editor-box-shadow: inset 0 0 2px var(--md-blue-300);
  --jp-cell-editor-active-background: var(--jp-layout-color0);
  --jp-cell-editor-active-border-color: var(--jp-brand-color1);
  --jp-cell-prompt-width: 64px;
  --jp-cell-prompt-font-family: var(--jp-code-font-family-default);
  --jp-cell-prompt-letter-spacing: 0;
  --jp-cell-prompt-opacity: 1;
  --jp-cell-prompt-not-active-opacity: 0.5;
  --jp-cell-prompt-not-active-font-color: var(--md-grey-700);

  /* A custom blend of MD grey and blue 600
   * See https://meyerweb.com/eric/tools/color-blend/#546E7A:1E88E5:5:hex */
  --jp-cell-inprompt-font-color: #307fc1;

  /* A custom blend of MD grey and orange 600
   * https://meyerweb.com/eric/tools/color-blend/#546E7A:F4511E:5:hex */
  --jp-cell-outprompt-font-color: #bf5b3d;

  /* Notebook specific styles */

  --jp-notebook-padding: 10px;
  --jp-notebook-select-background: var(--jp-layout-color1);
  --jp-notebook-multiselected-color: var(--md-blue-50);

  /* The scroll padding is calculated to fill enough space at the bottom of the
  notebook to show one single-line cell (with appropriate padding) at the top
  when the notebook is scrolled all the way to the bottom. We also subtract one
  pixel so that no scrollbar appears if we have just one single-line cell in the
  notebook. This padding is to enable a 'scroll past end' feature in a notebook.
  */
  --jp-notebook-scroll-padding: calc(
    100% - var(--jp-code-font-size) * var(--jp-code-line-height) -
      var(--jp-code-padding) - var(--jp-cell-padding) - 1px
  );

  /* Rendermime styles */

  --jp-rendermime-error-background: #fdd;
  --jp-rendermime-table-row-background: var(--md-grey-100);
  --jp-rendermime-table-row-hover-background: var(--md-light-blue-50);

  /* Dialog specific styles */

  --jp-dialog-background: rgba(0, 0, 0, 0.25);

  /* Console specific styles */

  --jp-console-padding: 10px;

  /* Toolbar specific styles */

  --jp-toolbar-border-color: var(--jp-border-color1);
  --jp-toolbar-micro-height: 8px;
  --jp-toolbar-background: var(--jp-layout-color1);
  --jp-toolbar-box-shadow: 0 0 2px 0 rgba(0, 0, 0, 0.24);
  --jp-toolbar-header-margin: 4px 4px 0 4px;
  --jp-toolbar-active-background: var(--md-grey-300);

  /* Statusbar specific styles */

  --jp-statusbar-height: 24px;

  /* Input field styles */

  --jp-input-box-shadow: inset 0 0 2px var(--md-blue-300);
  --jp-input-active-background: var(--jp-layout-color1);
  --jp-input-hover-background: var(--jp-layout-color1);
  --jp-input-background: var(--md-grey-100);
  --jp-input-border-color: var(--jp-inverse-border-color);
  --jp-input-active-border-color: var(--jp-brand-color1);
  --jp-input-active-box-shadow-color: rgba(19, 124, 189, 0.3);

  /* General editor styles */

  --jp-editor-selected-background: #d9d9d9;
  --jp-editor-selected-focused-background: #d7d4f0;
  --jp-editor-cursor-color: var(--jp-ui-font-color0);

  /* Code mirror specific styles */

  --jp-mirror-editor-keyword-color: #008000;
  --jp-mirror-editor-atom-color: #88f;
  --jp-mirror-editor-number-color: #080;
  --jp-mirror-editor-def-color: #00f;
  --jp-mirror-editor-variable-color: var(--md-grey-900);
  --jp-mirror-editor-variable-2-color: rgb(0, 54, 109);
  --jp-mirror-editor-variable-3-color: #085;
  --jp-mirror-editor-punctuation-color: #05a;
  --jp-mirror-editor-property-color: #05a;
  --jp-mirror-editor-operator-color: #a2f;
  --jp-mirror-editor-comment-color: #408080;
  --jp-mirror-editor-string-color: #ba2121;
  --jp-mirror-editor-string-2-color: #708;
  --jp-mirror-editor-meta-color: #a2f;
  --jp-mirror-editor-qualifier-color: #555;
  --jp-mirror-editor-builtin-color: #008000;
  --jp-mirror-editor-bracket-color: #997;
  --jp-mirror-editor-tag-color: #170;
  --jp-mirror-editor-attribute-color: #00c;
  --jp-mirror-editor-header-color: blue;
  --jp-mirror-editor-quote-color: #090;
  --jp-mirror-editor-link-color: #00c;
  --jp-mirror-editor-error-color: #f00;
  --jp-mirror-editor-hr-color: #999;

  /*
    RTC user specific colors.
    These colors are used for the cursor, username in the editor,
    and the icon of the user.
  */

  --jp-collaborator-color1: #ffad8e;
  --jp-collaborator-color2: #dac83d;
  --jp-collaborator-color3: #72dd76;
  --jp-collaborator-color4: #00e4d0;
  --jp-collaborator-color5: #45d4ff;
  --jp-collaborator-color6: #e2b1ff;
  --jp-collaborator-color7: #ff9de6;

  /* Vega extension styles */

  --jp-vega-background: white;

  /* Sidebar-related styles */

  --jp-sidebar-min-width: 250px;

  /* Search-related styles */

  --jp-search-toggle-off-opacity: 0.5;
  --jp-search-toggle-hover-opacity: 0.8;
  --jp-search-toggle-on-opacity: 1;
  --jp-search-selected-match-background-color: rgb(245, 200, 0);
  --jp-search-selected-match-color: black;
  --jp-search-unselected-match-background-color: var(
    --jp-inverse-layout-color0
  );
  --jp-search-unselected-match-color: var(--jp-ui-inverse-font-color0);

  /* Icon colors that work well with light or dark backgrounds */
  --jp-icon-contrast-color0: var(--md-purple-600);
  --jp-icon-contrast-color1: var(--md-green-600);
  --jp-icon-contrast-color2: var(--md-pink-600);
  --jp-icon-contrast-color3: var(--md-blue-600);

  /* Button colors */
  --jp-accept-color-normal: var(--md-blue-700);
  --jp-accept-color-hover: var(--md-blue-800);
  --jp-accept-color-active: var(--md-blue-900);
  --jp-warn-color-normal: var(--md-red-700);
  --jp-warn-color-hover: var(--md-red-800);
  --jp-warn-color-active: var(--md-red-900);
  --jp-reject-color-normal: var(--md-grey-600);
  --jp-reject-color-hover: var(--md-grey-700);
  --jp-reject-color-active: var(--md-grey-800);

  /* File or activity icons and switch semantic variables */
  --jp-jupyter-icon-color: #f37626;
  --jp-notebook-icon-color: #f37626;
  --jp-json-icon-color: var(--md-orange-700);
  --jp-console-icon-background-color: var(--md-blue-700);
  --jp-console-icon-color: white;
  --jp-terminal-icon-background-color: var(--md-grey-800);
  --jp-terminal-icon-color: var(--md-grey-200);
  --jp-text-editor-icon-color: var(--md-grey-700);
  --jp-inspector-icon-color: var(--md-grey-700);
  --jp-switch-color: var(--md-grey-400);
  --jp-switch-true-position-color: var(--md-orange-900);
}
</style>
<style type="text/css">
/* Force rendering true colors when outputing to pdf */
* {
  -webkit-print-color-adjust: exact;
}

/* Misc */
a.anchor-link {
  display: none;
}

/* Input area styling */
.jp-InputArea {
  overflow: hidden;
}

.jp-InputArea-editor {
  overflow: hidden;
}

.cm-editor.cm-s-jupyter .highlight pre {
/* weird, but --jp-code-padding defined to be 5px but 4px horizontal padding is hardcoded for pre.cm-line */
  padding: var(--jp-code-padding) 4px;
  margin: 0;

  font-family: inherit;
  font-size: inherit;
  line-height: inherit;
  color: inherit;

}

.jp-OutputArea-output pre {
  line-height: inherit;
  font-family: inherit;
}

.jp-RenderedText pre {
  color: var(--jp-content-font-color1);
  font-size: var(--jp-code-font-size);
}

/* Hiding the collapser by default */
.jp-Collapser {
  display: none;
}

@page {
    margin: 0.5in; /* Margin for each printed piece of paper */
}

@media print {
  .jp-Cell-inputWrapper,
  .jp-Cell-outputWrapper {
    display: block;
  }
}
</style>
<!-- Load mathjax -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/latest.js?config=TeX-AMS_CHTML-full,Safe"> </script>
<!-- MathJax configuration -->
<script type="text/x-mathjax-config">
    init_mathjax = function() {
        if (window.MathJax) {
        // MathJax loaded
            MathJax.Hub.Config({
                TeX: {
                    equationNumbers: {
                    autoNumber: "AMS",
                    useLabelIds: true
                    }
                },
                tex2jax: {
                    inlineMath: [ ['$','$'], ["\\(","\\)"] ],
                    displayMath: [ ['$$','$$'], ["\\[","\\]"] ],
                    processEscapes: true,
                    processEnvironments: true
                },
                displayAlign: 'center',
                CommonHTML: {
                    linebreaks: {
                    automatic: true
                    }
                }
            });

            MathJax.Hub.Queue(["Typeset", MathJax.Hub]);
        }
    }
    init_mathjax();
    </script>
<!-- End of mathjax configuration --><script type="module">
  document.addEventListener("DOMContentLoaded", async () => {
    const diagrams = document.querySelectorAll(".jp-Mermaid > pre.mermaid");
    // do not load mermaidjs if not needed
    if (!diagrams.length) {
      return;
    }
    const mermaid = (await import("https://cdnjs.cloudflare.com/ajax/libs/mermaid/10.7.0/mermaid.esm.min.mjs")).default;
    const parser = new DOMParser();

    mermaid.initialize({
      maxTextSize: 100000,
      maxEdges: 100000,
      startOnLoad: false,
      fontFamily: window
        .getComputedStyle(document.body)
        .getPropertyValue("--jp-ui-font-family"),
      theme: document.querySelector("body[data-jp-theme-light='true']")
        ? "default"
        : "dark",
    });

    let _nextMermaidId = 0;

    function makeMermaidImage(svg) {
      const img = document.createElement("img");
      const doc = parser.parseFromString(svg, "image/svg+xml");
      const svgEl = doc.querySelector("svg");
      const { maxWidth } = svgEl?.style || {};
      const firstTitle = doc.querySelector("title");
      const firstDesc = doc.querySelector("desc");

      img.setAttribute("src", `data:image/svg+xml,${encodeURIComponent(svg)}`);
      if (maxWidth) {
        img.width = parseInt(maxWidth);
      }
      if (firstTitle) {
        img.setAttribute("alt", firstTitle.textContent);
      }
      if (firstDesc) {
        const caption = document.createElement("figcaption");
        caption.className = "sr-only";
        caption.textContent = firstDesc.textContent;
        return [img, caption];
      }
      return [img];
    }

    async function makeMermaidError(text) {
      let errorMessage = "";
      try {
        await mermaid.parse(text);
      } catch (err) {
        errorMessage = `${err}`;
      }

      const result = document.createElement("details");
      result.className = 'jp-RenderedMermaid-Details';
      const summary = document.createElement("summary");
      summary.className = 'jp-RenderedMermaid-Summary';
      const pre = document.createElement("pre");
      const code = document.createElement("code");
      code.innerText = text;
      pre.appendChild(code);
      summary.appendChild(pre);
      result.appendChild(summary);

      const warning = document.createElement("pre");
      warning.innerText = errorMessage;
      result.appendChild(warning);
      return [result];
    }

    async function renderOneMarmaid(src) {
      const id = `jp-mermaid-${_nextMermaidId++}`;
      const parent = src.parentNode;
      let raw = src.textContent.trim();
      const el = document.createElement("div");
      el.style.visibility = "hidden";
      document.body.appendChild(el);
      let results = null;
      let output = null;
      try {
        let { svg } = await mermaid.render(id, raw, el);
        svg = cleanMermaidSvg(svg);
        results = makeMermaidImage(svg);
        output = document.createElement("figure");
        results.map(output.appendChild, output);
      } catch (err) {
        parent.classList.add("jp-mod-warning");
        results = await makeMermaidError(raw);
        output = results[0];
      } finally {
        el.remove();
      }
      parent.classList.add("jp-RenderedMermaid");
      parent.appendChild(output);
    }


    /**
     * Post-process to ensure mermaid diagrams contain only valid SVG and XHTML.
     */
    function cleanMermaidSvg(svg) {
      return svg.replace(RE_VOID_ELEMENT, replaceVoidElement);
    }


    /**
     * A regular expression for all void elements, which may include attributes and
     * a slash.
     *
     * @see https://developer.mozilla.org/en-US/docs/Glossary/Void_element
     *
     * Of these, only `<br>` is generated by Mermaid in place of `\n`,
     * but _any_ "malformed" tag will break the SVG rendering entirely.
     */
    const RE_VOID_ELEMENT =
      /<\s*(area|base|br|col|embed|hr|img|input|link|meta|param|source|track|wbr)\s*([^>]*?)\s*>/gi;

    /**
     * Ensure a void element is closed with a slash, preserving any attributes.
     */
    function replaceVoidElement(match, tag, rest) {
      rest = rest.trim();
      if (!rest.endsWith('/')) {
        rest = `${rest} /`;
      }
      return `<${tag} ${rest}>`;
    }

    void Promise.all([...diagrams].map(renderOneMarmaid));
  });
</script>
<style>
  .jp-Mermaid:not(.jp-RenderedMermaid) {
    display: none;
  }

  .jp-RenderedMermaid {
    overflow: auto;
    display: flex;
  }

  .jp-RenderedMermaid.jp-mod-warning {
    width: auto;
    padding: 0.5em;
    margin-top: 0.5em;
    border: var(--jp-border-width) solid var(--jp-warn-color2);
    border-radius: var(--jp-border-radius);
    color: var(--jp-ui-font-color1);
    font-size: var(--jp-ui-font-size1);
    white-space: pre-wrap;
    word-wrap: break-word;
  }

  .jp-RenderedMermaid figure {
    margin: 0;
    overflow: auto;
    max-width: 100%;
  }

  .jp-RenderedMermaid img {
    max-width: 100%;
  }

  .jp-RenderedMermaid-Details > pre {
    margin-top: 1em;
  }

  .jp-RenderedMermaid-Summary {
    color: var(--jp-warn-color2);
  }

  .jp-RenderedMermaid:not(.jp-mod-warning) pre {
    display: none;
  }

  .jp-RenderedMermaid-Summary > pre {
    display: inline-block;
    white-space: normal;
  }
</style>
<!-- End of mermaid configuration --></head>
<body class="jp-Notebook" data-jp-theme-light="true" data-jp-theme-name="JupyterLab Light">
<main>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p><strong>Group Member Names:</strong> Daniel Rabi and Joseph Gonzales<br/>
<strong>CCID:</strong> drabi, josephjo</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [ ]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-python"><pre><span></span><span class="kn">import</span> <span class="nn">numpy</span> <span class="k">as</span> <span class="nn">np</span>
<span class="kn">from</span> <span class="nn">datascience</span> <span class="kn">import</span> <span class="o">*</span>
<span class="kn">import</span> <span class="nn">requests</span>
<span class="kn">from</span> <span class="nn">bs4</span> <span class="kn">import</span> <span class="n">BeautifulSoup</span>
<span class="kn">import</span> <span class="nn">pandas</span> <span class="k">as</span> <span class="nn">pd</span>
<span class="kn">from</span> <span class="nn">IPython.core.display</span> <span class="kn">import</span> <span class="n">display</span><span class="p">,</span> <span class="n">HTML</span>

<span class="c1"># These lines set up graphing capabilities.</span>
<span class="kn">import</span> <span class="nn">matplotlib</span>
<span class="o">%</span><span class="n">matplotlib</span> <span class="n">inline</span>
<span class="kn">import</span> <span class="nn">matplotlib.pyplot</span> <span class="k">as</span> <span class="nn">plots</span>
<span class="n">plots</span><span class="o">.</span><span class="n">style</span><span class="o">.</span><span class="n">use</span><span class="p">(</span><span class="s1">'fivethirtyeight'</span><span class="p">)</span>
<span class="n">plots</span><span class="o">.</span><span class="n">style</span><span class="o">.</span><span class="n">use</span><span class="p">(</span><span class="s1">'fivethirtyeight'</span><span class="p">)</span>
<span class="n">plots</span><span class="o">.</span><span class="n">rcParams</span><span class="p">[</span><span class="s2">"patch.force_edgecolor"</span><span class="p">]</span> <span class="o">=</span> <span class="kc">True</span>
<span class="kn">import</span> <span class="nn">warnings</span>
<span class="n">warnings</span><span class="o">.</span><span class="n">simplefilter</span><span class="p">(</span><span class="s1">'ignore'</span><span class="p">,</span> <span class="ne">FutureWarning</span><span class="p">)</span>
</pre></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Connect Google Colab to Drive</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [ ]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-python"><pre><span></span><span class="c1">#from google.colab import drive</span>
<span class="c1">#drive.mount('/content/drive')</span>
</pre></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p><strong>Functions</strong></p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [ ]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-python"><pre><span></span><span class="k">def</span> <span class="nf">display_table</span><span class="p">(</span><span class="n">table</span><span class="p">):</span> <span class="c1"># Converting HTML code into python and displaying it.</span>
  <span class="n">display</span><span class="p">(</span><span class="n">HTML</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">table</span><span class="p">)))</span>

<span class="k">def</span> <span class="nf">scrape_table</span><span class="p">(</span><span class="n">table</span><span class="p">):</span> <span class="c1"># Converting HTML tables into dataframes and then change dataframe code to datascience code.</span>
    <span class="n">df</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">read_html</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">table</span><span class="p">))</span>
    <span class="n">df</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span><span class="n">df</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
    <span class="k">return</span> <span class="n">Table</span><span class="o">.</span><span class="n">from_df</span><span class="p">(</span><span class="n">df</span><span class="p">)</span>

<span class="k">def</span> <span class="nf">citation_remover</span><span class="p">(</span><span class="n">variable</span><span class="p">):</span> <span class="c1"># Cleans a column from citations.</span>
  <span class="n">array</span> <span class="o">=</span> <span class="n">variable</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">"["</span><span class="p">)</span>
  <span class="k">return</span> <span class="n">array</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>

<span class="k">def</span> <span class="nf">remove_dollar_float</span><span class="p">(</span><span class="n">price</span><span class="p">):</span> <span class="c1"># Removes the dollar sign from the column.</span>
  <span class="n">convertedPrice</span> <span class="o">=</span> <span class="nb">float</span><span class="p">(</span><span class="n">price</span><span class="o">.</span><span class="n">strip</span><span class="p">(</span><span class="s1">'$'</span><span class="p">))</span>
  <span class="k">return</span> <span class="n">convertedPrice</span>

<span class="k">def</span> <span class="nf">convert_to_cad</span><span class="p">(</span><span class="n">price</span><span class="p">):</span> <span class="c1"># Converts USD to Canadian currency.</span>
  <span class="n">converted_dollar</span> <span class="o">=</span> <span class="n">price</span> <span class="o">*</span> <span class="p">(</span><span class="n">exchangeRateAPI</span><span class="p">[</span><span class="s1">'rates'</span><span class="p">][</span><span class="s1">'CAD'</span><span class="p">])</span>
  <span class="k">return</span> <span class="nb">round</span><span class="p">(</span><span class="n">converted_dollar</span><span class="p">,</span><span class="mi">2</span><span class="p">)</span>

<span class="k">def</span> <span class="nf">calculateppp</span><span class="p">(</span><span class="n">localgood</span><span class="p">):</span> <span class="c1"># Calculates the Purchase Power Parity Index.</span>
  <span class="n">ppp</span> <span class="o">=</span> <span class="n">localgood</span> <span class="o">/</span> <span class="mf">3.85</span>
  <span class="k">return</span> <span class="n">ppp</span>

<span class="k">def</span> <span class="nf">remove_percent_sign</span><span class="p">(</span><span class="n">percentage</span><span class="p">):</span> <span class="c1"># Removes the percentage sign from a column.</span>
  <span class="n">first_num</span> <span class="o">=</span> <span class="n">percentage</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">"%"</span><span class="p">)</span>
  <span class="n">percent</span> <span class="o">=</span> <span class="nb">float</span><span class="p">(</span><span class="n">first_num</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span> <span class="o">/</span> <span class="mi">100</span>
  <span class="k">return</span> <span class="n">percent</span>

<span class="k">def</span> <span class="nf">capitalize</span><span class="p">(</span><span class="n">text</span><span class="p">):</span> <span class="c1"># Capitalizes a text.</span>
    <span class="k">return</span> <span class="n">text</span><span class="o">.</span><span class="n">upper</span><span class="p">()</span>

<span class="k">def</span> <span class="nf">getExchangeRate</span><span class="p">(</span><span class="n">currency</span><span class="p">):</span> <span class="c1"># Converts the currency to each country's currency's code.</span>
  <span class="n">converted_currency</span> <span class="o">=</span> <span class="n">exchangeRateAPI</span><span class="p">[</span><span class="s1">'rates'</span><span class="p">][</span><span class="n">currency</span><span class="p">]</span>
  <span class="k">return</span> <span class="n">converted_currency</span>

<span class="k">def</span> <span class="nf">getExchangeRateCAD</span><span class="p">(</span><span class="n">currency</span><span class="p">):</span> <span class="c1"># Converts the currency to CAD</span>
  <span class="n">converted_currency</span> <span class="o">=</span> <span class="n">exchangeRateAPICAD</span><span class="p">[</span><span class="s1">'rates'</span><span class="p">][</span><span class="n">currency</span><span class="p">]</span>
  <span class="k">return</span> <span class="n">converted_currency</span>

<span class="k">def</span> <span class="nf">standard_units</span><span class="p">(</span><span class="n">arr</span><span class="p">):</span>
<span class="w">    </span><span class="sd">""" Converts an array to standard units """</span>
    <span class="k">return</span> <span class="p">(</span><span class="n">arr</span> <span class="o">-</span> <span class="n">np</span><span class="o">.</span><span class="n">average</span><span class="p">(</span><span class="n">arr</span><span class="p">))</span><span class="o">/</span><span class="n">np</span><span class="o">.</span><span class="n">std</span><span class="p">(</span><span class="n">arr</span><span class="p">)</span>

<span class="k">def</span> <span class="nf">correlation</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">x</span><span class="p">,</span> <span class="n">y</span><span class="p">):</span>
<span class="w">    </span><span class="sd">""" Computes correlation: t is a table, and x and y are column names """</span>
    <span class="n">x_standard</span> <span class="o">=</span> <span class="n">standard_units</span><span class="p">(</span><span class="n">t</span><span class="o">.</span><span class="n">column</span><span class="p">(</span><span class="n">x</span><span class="p">))</span>
    <span class="n">y_standard</span> <span class="o">=</span> <span class="n">standard_units</span><span class="p">(</span><span class="n">t</span><span class="o">.</span><span class="n">column</span><span class="p">(</span><span class="n">y</span><span class="p">))</span>
    <span class="k">return</span> <span class="n">np</span><span class="o">.</span><span class="n">average</span><span class="p">(</span><span class="n">x_standard</span> <span class="o">*</span> <span class="n">y_standard</span><span class="p">)</span>
</pre></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p><strong>Step 1</strong></p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>We are creating a table to show the prices of tall lattes in US dollars in 19 countries. We will then convert these prices into the Canadian dollar and use an imported API  above to do so.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [ ]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-python"><pre><span></span><span class="c1"># Accessing an API to access nominal exchange rates of USD to other currencies.</span>
<span class="n">endpoint</span> <span class="o">=</span> <span class="s2">"https://api.fxratesapi.com/latest"</span>
<span class="n">endpointCAD</span> <span class="o">=</span> <span class="s2">"https://api.fxratesapi.com/latest?base=CAD"</span>
<span class="n">exchangeRateAPI</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">endpoint</span><span class="p">)</span><span class="o">.</span><span class="n">json</span><span class="p">()</span>
<span class="n">exchangeRateAPICAD</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">endpointCAD</span><span class="p">)</span><span class="o">.</span><span class="n">json</span><span class="p">()</span>
<span class="nb">print</span><span class="p">(</span><span class="n">exchangeRateAPICAD</span><span class="p">)</span> <span class="c1"># Used to test if the API is working.</span>

<span class="n">r</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">"https://embed.neomam.com/big-bucks-coffee/table/"</span><span class="p">)</span>

<span class="n">scrapedData</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">r</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">"html.parser"</span><span class="p">)</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="n">class_</span><span class="o">=</span><span class="s1">'item-line'</span><span class="p">)</span>
<span class="n">headers</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">r</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">"html.parser"</span><span class="p">)</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="n">class_</span><span class="o">=</span><span class="s1">'table-header'</span><span class="p">)</span>

<span class="n">display</span><span class="p">(</span><span class="n">HTML</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">r</span><span class="o">.</span><span class="n">text</span><span class="p">,</span> <span class="s2">"html.parser"</span><span class="p">))))</span>

<span class="n">scrapedData</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>{'success': True, 'terms': 'https://fxratesapi.com/legal/terms-conditions', 'privacy': 'https://fxratesapi.com/legal/privacy-policy', 'timestamp': 1733169960, 'date': '2024-12-02T20:06:00.000Z', 'base': 'CAD', 'rates': {'CAD': 1, 'ADA': 0.578790244, 'AED': 2.614219235, 'AFN': 48.42623707, 'ALL': 66.745743171, 'AMD': 284.218191868, 'ANG': 1.271672205, 'AOA': 649.428863932, 'ARB': 0.734523769, 'ARS': 719.551273774, 'AUD': 1.099804175, 'AWG': 1.274520099, 'AZN': 1.210438083, 'BAM': 1.326312848, 'BBD': 1.424044804, 'BDT': 85.416372518, 'BGN': 1.319185492, 'BHD': 0.267720423, 'BIF': 2066.187010659, 'BMD': 0.712022402, 'BNB': 0.001110132, 'BND': 0.95524227, 'BOB': 4.928313836, 'BRL': 4.317576401, 'BSD': 0.712022402, 'BTC': 7.413e-06, 'BTN': 59.939441214, 'BWP': 9.768863175, 'BYN': 2.32834748, 'BYR': 23283.461599532, 'BZD': 1.424044804, 'CDF': 2025.948991069, 'CHF': 0.631136765, 'CLF': 0.017950088, 'CLP': 696.452844466, 'CNY': 5.171839664, 'COP': 3173.015430676, 'CRC': 361.764409486, 'CUC': 0.712022402, 'CUP': 17.088537646, 'CVE': 74.824288527, 'CZK': 17.116864691, 'DAI': 0.71024638, 'DJF': 126.54133329, 'DKK': 5.060115993, 'DOP': 43.085637478, 'DOT': 0.076805375, 'DZD': 95.004604145, 'EGP': 35.366989417, 'ERN': 10.680336029, 'ETB': 90.527278789, 'ETH': 0.000196671, 'EUR': 0.678422178, 'FJD': 1.616768116, 'FKP': 0.562760104, 'GBP': 0.562690047, 'GEL': 1.983680455, 'GGP': 0.562760088, 'GHS': 10.879667914, 'GIP': 0.562760018, 'GMD': 41.680764316, 'GNF': 6139.175008845, 'GTQ': 5.486532266, 'GYD': 148.628421477, 'HKD': 5.5385598, 'HNL': 17.931532879, 'HRK': 4.763444697, 'HTG': 95.015293477, 'HUF': 281.272480575, 'IDR': 11272.428473645, 'ILS': 2.600932736, 'IMP': 0.562760295, 'INR': 60.270306765, 'IQD': 931.18473387, 'IRR': 29903.267508632, 'ISK': 98.794892576, 'JEP': 0.562759922, 'JMD': 111.407025166, 'JOD': 0.505535905, 'JPY': 106.432842995, 'KES': 92.209859594, 'KGS': 62.064162562, 'KHR': 2866.456267337, 'KMF': 333.920022235, 'KPW': 640.82538095, 'KRW': 999.613439641, 'KWD': 0.218056896, 'KYD': 0.593349628, 'KZT': 367.642043644, 'LAK': 15686.507292319, 'LBP': 63718.474019458, 'LKR': 207.472871991, 'LRD': 127.735730237, 'LSL': 12.939678132, 'LTC': 0.005327339, 'LTL': 2.343129039, 'LVL': 0.476932043, 'LYD': 3.469671584, 'MAD': 7.124896014, 'MDL': 12.996397717, 'MGA': 3338.288785389, 'MKD': 41.524339104, 'MMK': 1498.010682999, 'MNT': 2444.456591154, 'MOP': 5.72053144, 'MRO': 254.191875015, 'MUR': 33.166193351, 'MVR': 10.989341223, 'MWK': 1234.04704333, 'MXN': 14.512963077, 'MYR': 3.174587861, 'MZN': 45.258071558, 'NAD': 12.906084933, 'NGN': 1195.885417943, 'NIO': 26.19060679, 'NOK': 7.91249246, 'NPR': 96.743316719, 'NZD': 1.210003934, 'OMR': 0.273381047, 'OP': 0.293609568, 'PAB': 0.711103969, 'PEN': 2.666004439, 'PGK': 2.847862244, 'PHP': 41.763537622, 'PKR': 197.862678429, 'PLN': 2.904446736, 'PYG': 5570.621220076, 'QAR': 2.591113947, 'RON': 3.37688057, 'RSD': 79.104666415, 'RUB': 75.756665252, 'RWF': 974.236092339, 'SAR': 2.678984734, 'SBD': 5.982948516, 'SCR': 10.740068771, 'SDG': 428.28147475, 'SEK': 7.829662819, 'SGD': 0.957990658, 'SHP': 0.562690046, 'SLL': 16155.959714278, 'SOL': 0.003172142, 'SOS': 406.851982357, 'SRD': 25.054676316, 'STD': 16709.100768365, 'SVC': 6.230196017, 'SYP': 9258.133950451, 'SZL': 12.933718008, 'THB': 24.564578049, 'TJS': 7.775478271, 'TMT': 2.492078407, 'TND': 2.233878106, 'TOP': 1.684759132, 'TRY': 24.704404504, 'TTD': 4.767774008, 'TWD': 23.223795138, 'TZS': 1879.531495645, 'UAH': 29.696535876, 'UGX': 2625.596677519, 'USD': 0.712022402, 'UYU': 30.748258735, 'UZS': 9148.04834917, 'VEF': 3385661.012852594, 'VND': 18036.414878043, 'VUV': 86.145042661, 'WST': 1.968735471, 'XAF': 444.973687313, 'XAG': 0.023423017, 'XAU': 0.000270023, 'XCD': 1.922460485, 'XDR': 0.5400121, 'XOF': 444.973709866, 'XPD': 0.000721894, 'XPF': 80.891211186, 'XPT': 0.000751911, 'XRP': 0.257512295, 'YER': 177.406076299, 'ZAR': 12.91976221, 'ZMK': 6409.056044095, 'ZMW': 19.271180722, 'ZWL': 45331.409019997}}
</pre>
</div>
</div>
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output" data-mime-type="text/html" tabindex="0">
<!DOCTYPE html>

<html data-n-head="%7B%22lang%22:%7B%22ssr%22:%22en%22%7D%7D" data-n-head-ssr="" lang="en"><head>
<title>big-bucks-coffee</title><meta charset="utf-8" data-n-head="ssr"><meta content="width=device-width,initial-scale=1" data-n-head="ssr" name="viewport"/><meta content="" data-hid="description" data-n-head="ssr" name="description"/><meta content="telephone=no" data-n-head="ssr" name="format-detection"/><base href="/big-bucks-coffee/"/><link data-n-head="ssr" href="/favicon.ico" rel="icon" type="image/x-icon"/><link as="script" href="/big-bucks-coffee/_nuxt/2a9e3c7.js" rel="preload"/><link as="script" href="/big-bucks-coffee/_nuxt/0a20845.js" rel="preload"/><link as="script" href="/big-bucks-coffee/_nuxt/7b5510f.js" rel="preload"/><link as="script" href="/big-bucks-coffee/_nuxt/3fdb926.js" rel="preload"/><link as="script" href="/big-bucks-coffee/_nuxt/64c05c8.js" rel="preload"/><link as="script" href="/big-bucks-coffee/_nuxt/2ac100f.js" rel="preload"/><link as="script" href="/big-bucks-coffee/_nuxt/7c95806.js" rel="preload"/><style data-vue-ssr-id="fa7ff0ca:0 1eb45877:0 2bf66f94:0 a9262b60:0 2b6981e6:0 20523a10:0 67170c68:0 1db901ea:0">.nuxt-progress{position:fixed;top:0;left:0;right:0;height:2px;width:0;opacity:1;transition:width .1s,opacity .4s;background-color:#000;z-index:999999}.nuxt-progress.nuxt-progress-notransition{transition:none}.nuxt-progress-failed{background-color:red}@font-face{font-family:Karla;src:url(/big-bucks-coffee/_nuxt/fonts/Karla-Regular.a322767.woff2) format("woff2"),url(/big-bucks-coffee/_nuxt/fonts/Karla-Regular.374e8c3.woff) format("woff");font-weight:400;font-style:normal;font-display:swap}@font-face{font-family:Karla;src:url(/big-bucks-coffee/_nuxt/fonts/Karla-Bold.ae0ef56.woff2) format("woff2"),url(/big-bucks-coffee/_nuxt/fonts/Karla-Bold.2393a9a.woff) format("woff");font-weight:700;font-style:normal;font-display:swap}@font-face{font-family:"DM Serif Display";src:url(/big-bucks-coffee/_nuxt/fonts/DMSerifDisplay-Regular.71ef054.woff2) format("woff2"),url(/big-bucks-coffee/_nuxt/fonts/DMSerifDisplay-Regular.6616fa8.woff) format("woff");font-weight:400;font-style:normal;font-display:swap}@font-face{font-family:Karla;src:url(/big-bucks-coffee/_nuxt/fonts/Karla-ExtraBold.4bc4225.woff2) format("woff2"),url(/big-bucks-coffee/_nuxt/fonts/Karla-ExtraBold.c48bd6f.woff) format("woff");font-weight:700;font-style:normal;font-display:swap}body,html{padding:0;margin:0;font-family:Karla,sans-serif;background-color:#fff;color:#261e1b;font-size:14px;max-width:750px}@media(min-width:700px){body,html{font-size:14px}}main{padding:24px}@media(min-width:700px){.mobile{display:none}}@media(max-width:699px){.desktop{display:none}}button:active,button:focus{outline:0}.table-header{display:flex;align-items:center;padding:12px 0;text-transform:uppercase;color:#066b49;font-size:14px;font-weight:700;grid-gap:24px;gap:24px}.table-header div{cursor:pointer;padding:0 6px;box-sizing:border-box;display:flex;justify-content:space-between;align-items:center}.table-header div svg{min-width:10px;max-width:10px;min-height:10px;max-height:10px}.item-line{display:flex;align-items:center;grid-gap:24px;gap:24px}.item-line div{padding:8px 6px;overflow:hidden}.item-line div:not(:first-child){text-align:center;font-weight:400}.item-line .price{border-left:1px dotted #c5a982;border-right:1px dotted #c5a982}.item-line:nth-child(odd){background-color:#eedec7}.country,.price{width:30%}.most_expensive{width:40%}header[data-v-3437026c]{box-sizing:border-box;background-color:#dcece4;max-width:750px;background-repeat:no-repeat;background-position:0 100%;width:100vw;background-size:cover;padding:24px;position:relative}header img[data-v-3437026c]{width:200px;position:absolute;right:12px;bottom:0}@media(max-width:700px){header img[data-v-3437026c]{display:none}}header img.cup[data-v-3437026c]{right:0;bottom:-6px}h1[data-v-3437026c]{font-family:"DM Serif Display",serif;font-size:50px;max-width:480px;color:#066b49;text-align:left;line-height:1;margin:0}h1 span.lead[data-v-3437026c]{font-family:Karla,serif;font-weight:700;text-transform:uppercase;font-size:20px}@media(max-width:699px){h1[data-v-3437026c]{font-size:40px}}.copy[data-v-3437026c]{max-width:480px;margin-top:24px;text-align:left;font-size:15px;line-height:1.5}p[data-v-3437026c]{margin:0}.buttons[data-v-3437026c]{position:absolute;top:24px;right:24px}svg[data-v-93effdd4]{transition:opacity .4s ease;opacity:.7;cursor:pointer;position:fixed;bottom:60px;right:50px;z-index:100}svg.hide[data-v-93effdd4]{opacity:0;z-index:-1;pointer-events:none}#per-page[data-v-5089cd58]{background-color:transparent;margin:12px 0 0}#per-page button[data-v-5089cd58],#per-page[data-v-5089cd58]{cursor:pointer;display:flex;justify-content:center;align-items:center}#per-page button[data-v-5089cd58]{font-family:Karla,sans-serif;font-weight:600;background:#c5a982;color:#261e1b;border-radius:0;border:none;text-transform:uppercase;font-size:14px;width:100%;height:42px}#per-page button svg[data-v-5089cd58]{margin-left:4px;padding-bottom:2px}footer[data-v-59e3ab94]{display:flex;justify-content:flex-end;align-items:center;margin:24px}img[data-v-59e3ab94]{height:24px}.cls-1[data-v-0ed02d16]{fill:transparent;stroke:#c5a982;stroke-width:2px;transform-origin:center center;transform:scale(.93)}.cls-2[data-v-0ed02d16]{fill:#c5a982}svg[data-v-0ed02d16]{margin:0 3px}.actions[data-v-0ed02d16]{margin-left:-3px;box-sizing:border-box;display:flex;justify-content:left;align-items:center;z-index:10;position:relative}svg[data-v-0ed02d16]{width:22px;height:auto;cursor:pointer}.cls-1[data-v-4bb7d407]{fill:#066b49}.cls-2[data-v-4bb7d407]{fill:none;stroke:#fff;stroke-miterlimit:10;stroke-width:2px}.background[data-v-4bb7d407]{z-index:9;transition:all .3s ease;opacity:0;pointer-events:none;position:fixed;background-color:rgba(0,0,0,.42);width:100vw;height:100vh;left:0;top:0;display:flex;justify-content:center;align-items:center;box-sizing:border-box}.background.visible[data-v-4bb7d407]{opacity:1;pointer-events:all;z-index:20}.modal[data-v-4bb7d407]{margin:0 18px 18px;background-color:#c5a982;position:relative;width:100%;min-height:280px;box-sizing:border-box;padding:18px;max-height:90vh;overflow-y:scroll}.modal.breakdown[data-v-4bb7d407]{padding:0}.modal.breakdown h3[data-v-4bb7d407]{display:none}.close[data-v-4bb7d407]{top:10px;right:10px;height:22px;cursor:pointer}.title[data-v-4bb7d407]{width:100%;display:flex;justify-content:space-between;align-items:center;margin-bottom:18px}h3[data-v-4bb7d407]{font-family:"DM Serif Display",serif;text-transform:capitalize;font-weight:700;font-size:32px;color:#066b49;margin:0}p[data-v-4bb7d407]{color:#261e1b;font-weight:200;font-size:12px;line-height:1.5;margin-bottom:8px}a[data-v-4bb7d407]{color:#066b49;font-weight:700}textarea[data-v-4bb7d407]{display:block;width:100%;background-color:#fff;opacity:1;border-radius:0;color:#261e1b;border:none;font-size:12px;padding:10px;box-sizing:border-box;-webkit-appearance:textfield}button[data-v-4bb7d407]{background-color:#066b49;font-weight:700;color:#fff;text-transform:uppercase;font-size:14px;float:right;padding:8px 12px;border:none;margin-top:18px;border-radius:6px}button[data-v-4bb7d407]:active{filter:invert()}@media (min-width:730px){.modal[data-v-4bb7d407]{margin:auto;padding:28px}.modal.embed[data-v-4bb7d407],.modal.info[data-v-4bb7d407]{width:min(360px,90%)}h3[data-v-4bb7d407]{font-size:32px}.close[data-v-4bb7d407]{top:36px;right:36px;height:26px}p[data-v-4bb7d407]{font-size:12px;line-height:1.4}textarea[data-v-4bb7d407]{font-size:13px}}</style><link as="script" href="/big-bucks-coffee/_nuxt/static/1643642488/table/state.js" rel="preload"/><link as="script" href="/big-bucks-coffee/_nuxt/static/1643642488/table/payload.js" rel="preload"/><link as="script" href="/big-bucks-coffee/_nuxt/static/1643642488/manifest.js" rel="preload"/>
<meta content="noindex, follow" name="robots"/></meta></head>
<body>
<div data-server-rendered="true" id="__nuxt"><!-- --><div id="__layout"><div class="app"><header data-v-3437026c=""><h1 data-v-3437026c=""><span class="lead" data-v-3437026c="">What is the cost of a</span><br data-v-3437026c=""/>
    Starbucks Tall Latte in Every Country?
  </h1> <div class="copy" data-v-3437026c=""><p data-v-3437026c="">
      From just <strong data-v-3437026c="">$1.31</strong> in <strong data-v-3437026c="">Turkey</strong> and <strong data-v-3437026c="">$1.96</strong> in
      <strong data-v-3437026c="">Brazil</strong> to <strong data-v-3437026c="">$6.55</strong> in <strong data-v-3437026c="">Denmark</strong> and an incredible
      <strong data-v-3437026c="">$7.17</strong> in <strong data-v-3437026c="">Switzerland</strong>, the price of a simple Tall Latte from Starbucks varies
      around the world. How much does your Tall Latte cost, and where could you get it cheaper?
    </p></div> <div class="lg-only" data-v-3437026c=""><img alt="coffee shop" data-v-3437026c="" src="/big-bucks-coffee/_nuxt/img/illustration.84cda7e.svg"/></div> <div class="buttons" data-v-3437026c=""></div></header> <main><svg class="hide" data-v-93effdd4="" height="40" id="Layer_1" style="enable-background:new 0 0 32 32" version="1.1" viewbox="0 0 32 32" width="40" x="0px" xml:space="preserve" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" y="0px"><g data-v-93effdd4=""><path d="M16,0C7.2,0,0,7.2,0,16s7.2,16,16,16c8.8,0,16-7.2,16-16S24.8,0,16,0z M21.7,18.7C21.5,18.9,21.3,19,21,19
		c-0.3,0-0.5-0.1-0.7-0.3L17,15.4V24c0,0.6-0.4,1-1,1s-1-0.4-1-1v-8.6l-3.3,3.3c-0.4,0.4-1,0.4-1.4,0c-0.4-0.4-0.4-1,0-1.4l5-5h0
		c0.1-0.1,0.2-0.2,0.3-0.2c0.2-0.1,0.5-0.1,0.8,0c0.1,0.1,0.2,0.1,0.3,0.2l5,5C22.1,17.7,22.1,18.3,21.7,18.7z M22,10H10
		c-0.6,0-1-0.4-1-1s0.4-1,1-1h12c0.6,0,1,0.4,1,1S22.6,10,22,10z" data-v-93effdd4=""></path> <path d="M22,8H10C9.4,8,9,8.4,9,9s0.4,1,1,1h12c0.6,0,1-0.4,1-1S22.6,8,22,8z" data-v-93effdd4="" fill="#FFFFFF"></path> <path d="M16.7,12.3c-0.1-0.1-0.2-0.2-0.3-0.2c-0.2-0.1-0.5-0.1-0.8,0c-0.1,0.1-0.2,0.1-0.3,0.2h0l-5,5
		c-0.4,0.4-0.4,1,0,1.4c0.4,0.4,1,0.4,1.4,0l3.3-3.3V24c0,0.6,0.4,1,1,1s1-0.4,1-1v-8.6l3.3,3.3c0.2,0.2,0.5,0.3,0.7,0.3
		c0.3,0,0.5-0.1,0.7-0.3c0.4-0.4,0.4-1,0-1.4L16.7,12.3z" data-v-93effdd4="" fill="#FFFFFF"></path></g></svg> <div class="table-header"><div class="country selected"><span>Country</span> <svg height="8" style="transform:rotate(180deg)" viewbox="0 0 11.96 6.69" xmlns="http://www.w3.org/2000/svg"><polyline fill="#066B49" points="11.6 0.35 5.98 5.98 0.35 0.35" stroke-miterlimit="10" stroke-width="2"></polyline></svg></div> <div class="price"><span>Tall latte price</span> <svg height="8" style="transform:rotate(0)" viewbox="0 0 11.96 6.69" xmlns="http://www.w3.org/2000/svg"><polyline fill="#C5A982" points="11.6 0.35 5.98 5.98 0.35 0.35" stroke-miterlimit="10" stroke-width="2"></polyline></svg></div> <div class="most_expensive"><span>Price of most expensive item</span> <svg height="8" style="transform:rotate(0)" viewbox="0 0 11.96 6.69" xmlns="http://www.w3.org/2000/svg"><polyline fill="#C5A982" points="11.6 0.35 5.98 5.98 0.35 0.35" stroke-miterlimit="10" stroke-width="2"></polyline></svg></div></div> <div class="dataset"><div class="item-line"><div class="country"><strong>Andorra</strong></div> <div class="price">$3.28</div> <div class="most_expensive">N/A</div></div><div class="item-line"><div class="country"><strong>Argentina</strong></div> <div class="price">$4.67</div> <div class="most_expensive">$5.47</div></div><div class="item-line"><div class="country"><strong>Aruba</strong></div> <div class="price">$2.22</div> <div class="most_expensive">N/A</div></div><div class="item-line"><div class="country"><strong>Australia</strong></div> <div class="price">$3.97</div> <div class="most_expensive">$6.49</div></div><div class="item-line"><div class="country"><strong>Austria</strong></div> <div class="price">$3.48</div> <div class="most_expensive">$4.82</div></div><div class="item-line"><div class="country"><strong>Azerbaijan</strong></div> <div class="price">$3.41</div> <div class="most_expensive">N/A</div></div><div class="item-line"><div class="country"><strong>Bahamas</strong></div> <div class="price">$3.75</div> <div class="most_expensive">N/A</div></div><div class="item-line"><div class="country"><strong>Bahrain</strong></div> <div class="price">$4.24</div> <div class="most_expensive">$6.50</div></div><div class="item-line"><div class="country"><strong>Belgium</strong></div> <div class="price">$3.52</div> <div class="most_expensive">N/A</div></div><div class="item-line"><div class="country"><strong>Bolivia</strong></div> <div class="price">$3.19</div> <div class="most_expensive">$4.49</div></div><div class="item-line"><div class="country"><strong>Brazil</strong></div> <div class="price">$1.96</div> <div class="most_expensive">$2.94</div></div><div class="item-line"><div class="country"><strong>Bulgaria</strong></div> <div class="price">$2.69</div> <div class="most_expensive">$4.13</div></div><div class="item-line"><div class="country"><strong>Cambodia</strong></div> <div class="price">$3.25</div> <div class="most_expensive">$3.75</div></div><div class="item-line"><div class="country"><strong>Canada</strong></div> <div class="price">$3.85</div> <div class="most_expensive">$4.83</div></div><div class="item-line"><div class="country"><strong>Chile</strong></div> <div class="price">$4.95</div> <div class="most_expensive">$5.20</div></div><div class="item-line"><div class="country"><strong>China</strong></div> <div class="price">$4.23</div> <div class="most_expensive">$5.02</div></div><div class="item-line"><div class="country"><strong>Colombia</strong></div> <div class="price">$2.50</div> <div class="most_expensive">$3.50</div></div><div class="item-line"><div class="country"><strong>Costa Rica</strong></div> <div class="price">$4.22</div> <div class="most_expensive">$5.63</div></div><div class="item-line"><div class="country"><strong>Cyprus</strong></div> <div class="price">$2.97</div> <div class="most_expensive">$5.55</div></div><div class="item-line"><div class="country"><strong>Czech Republic</strong></div> <div class="price">$3.93</div> <div class="most_expensive">$5.70</div></div></div> <div data-v-5089cd58="" id="per-page"><button data-v-5089cd58=""><span data-v-5089cd58="">Show more</span> <!-- --></button></div></main> <footer data-v-59e3ab94=""><div data-v-59e3ab94="" style="margin-right:auto"><div class="actions" data-v-0ed02d16=""><a data-v-0ed02d16="" href="https://twitter.com/intent/tweet?url=https://embed.neomam.com/big-bucks-coffee/table/&amp;text=From%20its%20humble%20origins%20in%20Seattle,%20Starbucks%20has%20taken%20over%20the%20world.%20But%20the%20price%20of%20a%20caffeine%20boost%20varies%20from%20country%20to%20country.%20@CashNetUSA%20have%20done%20a%20study%20that%20discovers%20where%20in%20the%20world%20has%20the%20cheapest%20and%20most%20expensive%20Tall%20Lattes." id="twitter" target="_blank"><svg data-v-0ed02d16="" viewbox="0 0 22 22" xmlns="http://www.w3.org/2000/svg"><path class="cls-1" d="M22,11A11,11,0,1,1,11,0,11,11,0,0,1,22,11Z" data-v-0ed02d16=""></path> <path class="cls-2" d="M17.52,7.64A5.66,5.66,0,0,1,16,8.06,2.67,2.67,0,0,0,17.16,6.6a5.53,5.53,0,0,1-1.7.64,2.69,2.69,0,0,0-2-.83A2.66,2.66,0,0,0,10.83,9a2.9,2.9,0,0,0,.07.6A7.64,7.64,0,0,1,5.39,6.89a2.61,2.61,0,0,0,.83,3.51A2.72,2.72,0,0,1,5,10.08v0a2.47,2.47,0,0,0,.18,1,2.67,2.67,0,0,0,2,1.63,2.69,2.69,0,0,1-.7.09,2.07,2.07,0,0,1-.5,0,2.66,2.66,0,0,0,2.49,1.83,5.37,5.37,0,0,1-3.32,1.13,4.58,4.58,0,0,1-.64,0,7.65,7.65,0,0,0,4.1,1.18A7.45,7.45,0,0,0,16,10.94a7.32,7.32,0,0,0,.18-1.59c0-.12,0-.23,0-.34A5.45,5.45,0,0,0,17.52,7.64Z" data-v-0ed02d16=""></path></svg></a> <a data-v-0ed02d16="" href="https://www.facebook.com/sharer/sharer.php?u=https://embed.neomam.com/big-bucks-coffee/table" id="facebook" target="_blank"><svg data-v-0ed02d16="" viewbox="0 0 22 22" xmlns="http://www.w3.org/2000/svg"><circle class="cls-1" cx="11" cy="11" data-v-0ed02d16="" r="11" transform="translate(-0.16 0.16) rotate(-0.82)"></circle> <path class="cls-2" d="M12,8.43v-1a.55.55,0,0,1,.58-.62H14V4.52H12A2.54,2.54,0,0,0,9.25,7.25V8.43H8V11h1.3v6.52h2.61V11H13.8l.1-1L14,8.43Z" data-v-0ed02d16=""></path></svg></a> <a data-v-0ed02d16="" id="embed"><svg data-v-0ed02d16="" viewbox="0 0 22 22" xmlns="http://www.w3.org/2000/svg"><circle class="cls-1" cx="11" cy="11" data-v-0ed02d16="" r="11"></circle> <path class="cls-2" d="M3.9,11.83V10.71L8.47,8V9.91L6,11.27l2.43,1.36V14.5Z" data-v-0ed02d16=""></path> <path class="cls-2" d="M10.61,16H9L11.39,5H13Z" data-v-0ed02d16=""></path> <path class="cls-2" d="M13.53,14.5V12.63L16,11.27,13.53,9.91V8l4.57,2.67v1.12Z" data-v-0ed02d16=""></path></svg></a> <a data-v-0ed02d16="" id="info"><svg data-v-0ed02d16="" viewbox="0 0 22 22" xmlns="http://www.w3.org/2000/svg"><circle class="cls-1" cx="11" cy="11" data-v-0ed02d16="" r="11"></circle> <circle class="cls-2" cx="11" cy="6.5" data-v-0ed02d16="" r="1.66"></circle> <polygon class="cls-2" data-v-0ed02d16="" points="12.52 9.58 9.48 10.21 9.48 17.41 12.52 17.41 12.52 9.58"></polygon></svg></a></div></div> <a data-v-59e3ab94="" href="https://www.cashnetusa.com/blog/" target="_blank"><img alt="SavingSpot" data-v-59e3ab94="" src="/big-bucks-coffee/_nuxt/img/logo.fc5e12c.svg"/></a></footer> <div class="background" data-v-4bb7d407=""><div class="modal info" data-v-4bb7d407=""><div class="title" data-v-4bb7d407=""><h3 data-v-4bb7d407="">info</h3> <svg class="close" data-v-4bb7d407="" viewbox="0 0 18 18" xmlns="http://www.w3.org/2000/svg"><circle class="cls-1 info" cx="9" cy="9" data-v-4bb7d407="" r="9"></circle> <line class="cls-2 info" data-v-4bb7d407="" x1="5.53" x2="12.47" y1="12.47" y2="5.53"></line> <line class="cls-2 info" data-v-4bb7d407="" x1="5.53" x2="12.47" y1="5.53" y2="12.47"></line></svg></div> <!-- --> <div class="info" data-v-4bb7d407=""><p data-v-4bb7d407=""><strong data-v-4bb7d407="">Methodology:</strong></p> <p data-v-4bb7d407="">
        To find the price of a tall latte in every country, we used Starbucks prices on delivery apps that operate
        within each specific region such as Deliveroo, Just Eat, PedidosYa and Uber Eats. For countries without a
        delivery service, we sourced information from third party websites and found updated menus sourcing reviews
        with the help of Google Images and Google Translate.
      </p> <p data-v-4bb7d407="">
        All delivery websites we gathered information from gave us the price of a tall latte and the most expensive
        item which when then converted into USD. For some specific countries, we contacted residents who were able to
        give us the correct information. For the USA, we gathered the price of a Tall Latte in every state and then we
        took an average as the price of a Tall Latte in the country.
      </p></div></div></div></div></div></div><script defer="" src="/big-bucks-coffee/_nuxt/static/1643642488/table/state.js"></script><script defer="" src="/big-bucks-coffee/_nuxt/2a9e3c7.js"></script><script defer="" src="/big-bucks-coffee/_nuxt/64c05c8.js"></script><script defer="" src="/big-bucks-coffee/_nuxt/2ac100f.js"></script><script defer="" src="/big-bucks-coffee/_nuxt/7c95806.js"></script><script defer="" src="/big-bucks-coffee/_nuxt/0a20845.js"></script><script defer="" src="/big-bucks-coffee/_nuxt/7b5510f.js"></script><script defer="" src="/big-bucks-coffee/_nuxt/3fdb926.js"></script>
</body></html>
</div>
</div>
<div class="jp-OutputArea-child jp-OutputArea-executeResult">
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[ ]:</div>
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>&lt;div class="item-line"&gt;&lt;div class="country"&gt;&lt;strong&gt;Andorra&lt;/strong&gt;&lt;/div&gt; &lt;div class="price"&gt;$3.28&lt;/div&gt; &lt;div class="most_expensive"&gt;N/A&lt;/div&gt;&lt;/div&gt;</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [ ]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-python"><pre><span></span><span class="n">countries</span> <span class="o">=</span> <span class="p">[]</span>
<span class="n">latte_prices</span> <span class="o">=</span> <span class="p">[]</span>
<span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">scrapedData</span><span class="p">:</span>
    <span class="n">cols</span> <span class="o">=</span> <span class="n">row</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">"div"</span><span class="p">,</span> <span class="n">class_</span><span class="o">=</span><span class="s2">"country"</span><span class="p">)</span>
    <span class="n">countries</span><span class="o">.</span><span class="n">extend</span><span class="p">([</span><span class="n">col</span><span class="o">.</span><span class="n">get_text</span><span class="p">(</span><span class="n">strip</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="k">for</span> <span class="n">col</span> <span class="ow">in</span> <span class="n">cols</span><span class="p">])</span>
    <span class="n">cols</span> <span class="o">=</span> <span class="n">row</span><span class="o">.</span><span class="n">find_all</span><span class="p">(</span><span class="s2">"div"</span><span class="p">,</span> <span class="n">class_</span><span class="o">=</span><span class="s2">"price"</span><span class="p">)</span>
    <span class="n">latte_prices</span><span class="o">.</span><span class="n">extend</span><span class="p">([</span><span class="n">col</span><span class="o">.</span><span class="n">get_text</span><span class="p">(</span><span class="n">strip</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="k">for</span> <span class="n">col</span> <span class="ow">in</span> <span class="n">cols</span><span class="p">])</span>
<span class="n">pytable</span> <span class="o">=</span> <span class="n">Table</span><span class="p">()</span><span class="o">.</span><span class="n">with_columns</span><span class="p">(</span><span class="s2">"country"</span><span class="p">,</span> <span class="n">countries</span><span class="p">,</span> <span class="s2">"price of latte in USD"</span><span class="p">,</span> <span class="n">latte_prices</span><span class="p">)</span>
<span class="n">pytable</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output" data-mime-type="text/html" tabindex="0">
<table border="1" class="dataframe">
<thead>
<tr>
<th>country</th> <th>price of latte in USD</th>
</tr>
</thead>
<tbody>
<tr>
<td>Andorra       </td> <td>$3.28                </td>
</tr>
<tr>
<td>Argentina     </td> <td>$4.67                </td>
</tr>
<tr>
<td>Aruba         </td> <td>$2.22                </td>
</tr>
<tr>
<td>Australia     </td> <td>$3.97                </td>
</tr>
<tr>
<td>Austria       </td> <td>$3.48                </td>
</tr>
<tr>
<td>Azerbaijan    </td> <td>$3.41                </td>
</tr>
<tr>
<td>Bahamas       </td> <td>$3.75                </td>
</tr>
<tr>
<td>Bahrain       </td> <td>$4.24                </td>
</tr>
<tr>
<td>Belgium       </td> <td>$3.52                </td>
</tr>
<tr>
<td>Bolivia       </td> <td>$3.19                </td>
</tr>
<tr>
<td>Brazil        </td> <td>$1.96                </td>
</tr>
<tr>
<td>Bulgaria      </td> <td>$2.69                </td>
</tr>
<tr>
<td>Cambodia      </td> <td>$3.25                </td>
</tr>
<tr>
<td>Canada        </td> <td>$3.85                </td>
</tr>
<tr>
<td>Chile         </td> <td>$4.95                </td>
</tr>
<tr>
<td>China         </td> <td>$4.23                </td>
</tr>
<tr>
<td>Colombia      </td> <td>$2.50                </td>
</tr>
<tr>
<td>Costa Rica    </td> <td>$4.22                </td>
</tr>
<tr>
<td>Cyprus        </td> <td>$2.97                </td>
</tr>
<tr>
<td>Czech Republic</td> <td>$3.93                </td>
</tr>
</tbody>
</table>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p><strong>Step 2</strong></p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Here we are cleaning the data.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [ ]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-python"><pre><span></span><span class="n">coffeetableUSD</span> <span class="o">=</span> <span class="n">pytable</span><span class="o">.</span><span class="n">with_columns</span><span class="p">(</span><span class="s1">'price of latte in USD'</span><span class="p">,</span> <span class="n">pytable</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="n">remove_dollar_float</span><span class="p">,</span> <span class="s1">'price of latte in USD'</span><span class="p">))</span>
<span class="n">coffeetable</span> <span class="o">=</span> <span class="n">coffeetableUSD</span><span class="o">.</span><span class="n">with_columns</span><span class="p">(</span><span class="s1">'price of latte in CAD'</span><span class="p">,</span> <span class="n">coffeetableUSD</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="n">convert_to_cad</span><span class="p">,</span> <span class="s1">'price of latte in USD'</span><span class="p">),</span> <span class="s1">'Purchasing Power Parity'</span><span class="p">,</span> <span class="n">coffeetableUSD</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="n">calculateppp</span><span class="p">,</span> <span class="s1">'price of latte in USD'</span><span class="p">))</span>
<span class="n">coffeetable</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output" data-mime-type="text/html" tabindex="0">
<table border="1" class="dataframe">
<thead>
<tr>
<th>country</th> <th>price of latte in USD</th> <th>price of latte in CAD</th> <th>Purchasing Power Parity</th>
</tr>
</thead>
<tbody>
<tr>
<td>Andorra       </td> <td>3.28                 </td> <td>4.61                 </td> <td>0.851948               </td>
</tr>
<tr>
<td>Argentina     </td> <td>4.67                 </td> <td>6.56                 </td> <td>1.21299                </td>
</tr>
<tr>
<td>Aruba         </td> <td>2.22                 </td> <td>3.12                 </td> <td>0.576623               </td>
</tr>
<tr>
<td>Australia     </td> <td>3.97                 </td> <td>5.58                 </td> <td>1.03117                </td>
</tr>
<tr>
<td>Austria       </td> <td>3.48                 </td> <td>4.89                 </td> <td>0.903896               </td>
</tr>
<tr>
<td>Azerbaijan    </td> <td>3.41                 </td> <td>4.79                 </td> <td>0.885714               </td>
</tr>
<tr>
<td>Bahamas       </td> <td>3.75                 </td> <td>5.27                 </td> <td>0.974026               </td>
</tr>
<tr>
<td>Bahrain       </td> <td>4.24                 </td> <td>5.95                 </td> <td>1.1013                 </td>
</tr>
<tr>
<td>Belgium       </td> <td>3.52                 </td> <td>4.94                 </td> <td>0.914286               </td>
</tr>
<tr>
<td>Bolivia       </td> <td>3.19                 </td> <td>4.48                 </td> <td>0.828571               </td>
</tr>
<tr>
<td>Brazil        </td> <td>1.96                 </td> <td>2.75                 </td> <td>0.509091               </td>
</tr>
<tr>
<td>Bulgaria      </td> <td>2.69                 </td> <td>3.78                 </td> <td>0.698701               </td>
</tr>
<tr>
<td>Cambodia      </td> <td>3.25                 </td> <td>4.56                 </td> <td>0.844156               </td>
</tr>
<tr>
<td>Canada        </td> <td>3.85                 </td> <td>5.41                 </td> <td>1                      </td>
</tr>
<tr>
<td>Chile         </td> <td>4.95                 </td> <td>6.95                 </td> <td>1.28571                </td>
</tr>
<tr>
<td>China         </td> <td>4.23                 </td> <td>5.94                 </td> <td>1.0987                 </td>
</tr>
<tr>
<td>Colombia      </td> <td>2.5                  </td> <td>3.51                 </td> <td>0.649351               </td>
</tr>
<tr>
<td>Costa Rica    </td> <td>4.22                 </td> <td>5.93                 </td> <td>1.0961                 </td>
</tr>
<tr>
<td>Cyprus        </td> <td>2.97                 </td> <td>4.17                 </td> <td>0.771429               </td>
</tr>
<tr>
<td>Czech Republic</td> <td>3.93                 </td> <td>5.52                 </td> <td>1.02078                </td>
</tr>
</tbody>
</table>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p><strong>Step 3</strong></p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Importing tax data, cleaning the data, and creating a PPP Index that factors local tax into the price.
Brazil's and Canada's sales tax varies with location; therefore, we took the average sales tax that a consumer will pay for coffee.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [ ]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-python"><pre><span></span><span class="n">tax_link</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">"https://en.wikipedia.org/wiki/Value-added_tax#Around_the_world"</span><span class="p">)</span>
<span class="n">scraped_tax_data</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">tax_link</span><span class="o">.</span><span class="n">text</span><span class="p">,</span><span class="s2">"html.parser"</span><span class="p">)</span>


<span class="n">heading1</span> <span class="o">=</span> <span class="n">scraped_tax_data</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">"h3"</span><span class="p">,</span> <span class="p">{</span><span class="s2">"id"</span><span class="p">:</span> <span class="s2">"European_Union_countries"</span><span class="p">})</span> <span class="c1"># Importing European Union Countrys' tax data</span>
<span class="n">euro_table</span> <span class="o">=</span> <span class="n">heading1</span><span class="o">.</span><span class="n">find_next</span><span class="p">(</span><span class="s2">"table"</span><span class="p">,</span> <span class="p">{</span><span class="s2">"class"</span><span class="p">:</span> <span class="s2">"wikitable"</span><span class="p">})</span>
<span class="n">euro_table</span> <span class="o">=</span> <span class="n">scrape_table</span><span class="p">(</span><span class="n">euro_table</span><span class="p">)</span>
<span class="n">euro_table</span> <span class="o">=</span> <span class="n">euro_table</span><span class="o">.</span><span class="n">select</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>

<span class="n">euro_table</span> <span class="o">=</span> <span class="n">euro_table</span><span class="o">.</span><span class="n">with_column</span><span class="p">(</span><span class="s2">"Standard rate (current)"</span><span class="p">,</span> <span class="n">euro_table</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="n">citation_remover</span><span class="p">,</span> <span class="mi">1</span><span class="p">))</span>
<span class="c1">#euro_table = euro_table.with_column("Standard rate (current)", euro_table.apply(remove_percent_sign, 1))</span>


<span class="n">heading2</span> <span class="o">=</span> <span class="n">scraped_tax_data</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">"h3"</span><span class="p">,</span> <span class="p">{</span><span class="s2">"id"</span><span class="p">:</span> <span class="s2">"Non-European_Union_countries"</span><span class="p">})</span> <span class="c1"># Importing non European Union Countrys' tax data</span>
<span class="n">non_euro_table</span> <span class="o">=</span> <span class="n">heading2</span><span class="o">.</span><span class="n">find_next</span><span class="p">(</span><span class="s2">"table"</span><span class="p">,</span> <span class="p">{</span><span class="s2">"class"</span><span class="p">:</span> <span class="s2">"wikitable"</span><span class="p">})</span>
<span class="n">non_euro_table</span> <span class="o">=</span> <span class="n">scrape_table</span><span class="p">(</span><span class="n">non_euro_table</span><span class="p">)</span>
<span class="n">non_euro_table</span> <span class="o">=</span> <span class="n">non_euro_table</span><span class="o">.</span><span class="n">select</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>


<span class="n">non_euro_table</span> <span class="o">=</span> <span class="n">non_euro_table</span><span class="o">.</span><span class="n">with_column</span><span class="p">(</span><span class="s2">"Country"</span><span class="p">,</span> <span class="n">non_euro_table</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="n">citation_remover</span><span class="p">,</span> <span class="mi">0</span><span class="p">))</span>
<span class="c1">#non_euro_table = non_euro_table.with_column("Standard rate (current)", non_euro_table.apply(remove_percent_sign, 1))</span>

<span class="n">tax_table</span> <span class="o">=</span> <span class="n">euro_table</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">non_euro_table</span><span class="p">)</span><span class="o">.</span><span class="n">sort</span><span class="p">(</span><span class="s2">"Country"</span><span class="p">)</span> <span class="c1"># Combining all of the data into one table</span>


<span class="n">coffee_table_tax</span> <span class="o">=</span> <span class="n">coffeetable</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">"country"</span><span class="p">,</span> <span class="n">tax_table</span><span class="p">,</span> <span class="s2">"Country"</span><span class="p">)</span> <span class="c1"># Joining the tax data with the coffee table</span>
<span class="n">coffee_table_tax</span> <span class="o">=</span> <span class="n">coffee_table_tax</span><span class="o">.</span><span class="n">relabel</span><span class="p">(</span><span class="s2">"country"</span><span class="p">,</span> <span class="s2">"Country"</span><span class="p">)</span><span class="o">.</span><span class="n">relabel</span><span class="p">(</span><span class="s2">"price of latte in USD"</span><span class="p">,</span> <span class="s2">"Latte Price (USD)"</span><span class="p">)</span><span class="o">.</span><span class="n">relabel</span><span class="p">(</span><span class="s2">"price of latte in CAD"</span><span class="p">,</span> <span class="s2">"Latte Price (CAD)"</span><span class="p">)</span><span class="o">.</span><span class="n">relabel</span><span class="p">(</span><span class="s2">"Standard rate (current)"</span><span class="p">,</span> <span class="s2">"Sales Tax"</span><span class="p">)</span>

<span class="n">coffee_table_tax_array</span> <span class="o">=</span> <span class="n">coffee_table_tax</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="n">remove_percent_sign</span><span class="p">,</span><span class="s2">"Sales Tax"</span><span class="p">)</span> <span class="c1"># Cleaning the data using a predefined function</span>
<span class="n">coffee_table_tax_array</span><span class="p">[</span><span class="mi">9</span><span class="p">]</span> <span class="o">=</span> <span class="mf">0.22</span> <span class="c1"># Setting the average sales tax for Brazil</span>
<span class="n">coffee_table_tax_array</span><span class="p">[</span><span class="mi">12</span><span class="p">]</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">average</span><span class="p">([</span><span class="mf">0.05</span><span class="p">,</span><span class="mf">0.12</span><span class="p">,</span><span class="mf">0.12</span><span class="p">,</span><span class="mf">0.15</span><span class="p">,</span><span class="mf">0.15</span><span class="p">,</span><span class="mf">0.05</span><span class="p">,</span><span class="mf">0.15</span><span class="p">,</span><span class="mf">0.05</span><span class="p">,</span><span class="mf">0.13</span><span class="p">,</span><span class="mf">0.15</span><span class="p">,</span><span class="mf">0.14975</span><span class="p">,</span><span class="mf">0.11</span><span class="p">,</span><span class="mf">0.05</span><span class="p">])</span> <span class="c1"># Setting the average sales tax for Canada</span>
<span class="n">coffee_table_tax</span> <span class="o">=</span> <span class="n">coffee_table_tax</span><span class="o">.</span><span class="n">with_column</span><span class="p">(</span><span class="s2">"Sales Tax"</span><span class="p">,</span> <span class="n">coffee_table_tax_array</span><span class="p">)</span>

<span class="n">cnd_price</span> <span class="o">=</span> <span class="n">coffee_table_tax</span><span class="o">.</span><span class="n">where</span><span class="p">(</span><span class="s2">"Country"</span><span class="p">,</span> <span class="s2">"Canada"</span><span class="p">)</span><span class="o">.</span><span class="n">column</span><span class="p">(</span><span class="s2">"Latte Price (CAD)"</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>

<span class="c1"># Calculating PPP with tax:</span>
<span class="n">coffee_table_tax</span> <span class="o">=</span> <span class="n">coffee_table_tax</span><span class="o">.</span><span class="n">with_column</span><span class="p">(</span><span class="s2">"Purchasing Power Parity with tax"</span><span class="p">,</span> <span class="p">((</span><span class="n">coffee_table_tax</span><span class="o">.</span><span class="n">column</span><span class="p">(</span><span class="s1">'Latte Price (CAD)'</span><span class="p">)</span> <span class="o">*</span> <span class="p">(</span><span class="mi">1</span> <span class="o">+</span> <span class="n">coffee_table_tax</span><span class="o">.</span><span class="n">column</span><span class="p">(</span><span class="s2">"Sales Tax"</span><span class="p">)))</span> <span class="o">/</span> <span class="p">(</span><span class="n">cnd_price</span> <span class="o">*</span> <span class="p">(</span><span class="mi">1</span> <span class="o">+</span> <span class="n">coffee_table_tax</span><span class="o">.</span><span class="n">column</span><span class="p">(</span><span class="s2">"Sales Tax"</span><span class="p">)))))</span>
<span class="n">coffee_table_tax</span> <span class="o">=</span> <span class="n">coffee_table_tax</span><span class="o">.</span><span class="n">with_column</span><span class="p">(</span><span class="s2">"Country"</span><span class="p">,</span> <span class="n">coffee_table_tax</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="n">capitalize</span><span class="p">,</span> <span class="s1">'Country'</span><span class="p">))</span>
<span class="n">coffee_table_tax</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output" data-mime-type="text/html" tabindex="0">
<table border="1" class="dataframe">
<thead>
<tr>
<th>Country</th> <th>Latte Price (USD)</th> <th>Latte Price (CAD)</th> <th>Purchasing Power Parity</th> <th>Sales Tax</th> <th>Purchasing Power Parity with tax</th>
</tr>
</thead>
<tbody>
<tr>
<td>ANDORRA       </td> <td>3.28             </td> <td>4.61             </td> <td>0.851948               </td> <td>0.045    </td> <td>0.852126                        </td>
</tr>
<tr>
<td>ARGENTINA     </td> <td>4.67             </td> <td>6.56             </td> <td>1.21299                </td> <td>0.21     </td> <td>1.21257                         </td>
</tr>
<tr>
<td>AUSTRALIA     </td> <td>3.97             </td> <td>5.58             </td> <td>1.03117                </td> <td>0.1      </td> <td>1.03142                         </td>
</tr>
<tr>
<td>AUSTRIA       </td> <td>3.48             </td> <td>4.89             </td> <td>0.903896               </td> <td>0.2      </td> <td>0.903882                        </td>
</tr>
<tr>
<td>AZERBAIJAN    </td> <td>3.41             </td> <td>4.79             </td> <td>0.885714               </td> <td>0.18     </td> <td>0.885397                        </td>
</tr>
<tr>
<td>BAHAMAS       </td> <td>3.75             </td> <td>5.27             </td> <td>0.974026               </td> <td>0.12     </td> <td>0.974122                        </td>
</tr>
<tr>
<td>BAHRAIN       </td> <td>4.24             </td> <td>5.95             </td> <td>1.1013                 </td> <td>0.1      </td> <td>1.09982                         </td>
</tr>
<tr>
<td>BELGIUM       </td> <td>3.52             </td> <td>4.94             </td> <td>0.914286               </td> <td>0.21     </td> <td>0.913124                        </td>
</tr>
<tr>
<td>BOLIVIA       </td> <td>3.19             </td> <td>4.48             </td> <td>0.828571               </td> <td>0.13     </td> <td>0.828096                        </td>
</tr>
<tr>
<td>BRAZIL        </td> <td>1.96             </td> <td>2.75             </td> <td>0.509091               </td> <td>0.22     </td> <td>0.508318                        </td>
</tr>
<tr>
<td>BULGARIA      </td> <td>2.69             </td> <td>3.78             </td> <td>0.698701               </td> <td>0.2      </td> <td>0.698706                        </td>
</tr>
<tr>
<td>CAMBODIA      </td> <td>3.25             </td> <td>4.56             </td> <td>0.844156               </td> <td>0.1      </td> <td>0.842884                        </td>
</tr>
<tr>
<td>CANADA        </td> <td>3.85             </td> <td>5.41             </td> <td>1                      </td> <td>0.109981 </td> <td>1                               </td>
</tr>
<tr>
<td>CHILE         </td> <td>4.95             </td> <td>6.95             </td> <td>1.28571                </td> <td>0.19     </td> <td>1.28466                         </td>
</tr>
<tr>
<td>CHINA         </td> <td>4.23             </td> <td>5.94             </td> <td>1.0987                 </td> <td>0.13     </td> <td>1.09797                         </td>
</tr>
<tr>
<td>COLOMBIA      </td> <td>2.5              </td> <td>3.51             </td> <td>0.649351               </td> <td>0.19     </td> <td>0.648799                        </td>
</tr>
<tr>
<td>COSTA RICA    </td> <td>4.22             </td> <td>5.93             </td> <td>1.0961                 </td> <td>0.13     </td> <td>1.09612                         </td>
</tr>
<tr>
<td>CYPRUS        </td> <td>2.97             </td> <td>4.17             </td> <td>0.771429               </td> <td>0.19     </td> <td>0.770795                        </td>
</tr>
<tr>
<td>CZECH REPUBLIC</td> <td>3.93             </td> <td>5.52             </td> <td>1.02078                </td> <td>0.21     </td> <td>1.02033                         </td>
</tr>
</tbody>
</table>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Creating a bar graph to visualize the change of PPP by sales tax.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [ ]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-python"><pre><span></span><span class="n">coffee_table_tax</span><span class="o">.</span><span class="n">select</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">3</span><span class="p">,</span> <span class="mi">5</span><span class="p">)</span><span class="o">.</span><span class="n">barh</span><span class="p">(</span><span class="s2">"Country"</span><span class="p">)</span>
<span class="n">plots</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">"Purchasing Power Parity with Sales Tax"</span><span class="p">)</span>
<span class="n">plots</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">"Purchasing Power Parity Index"</span><span class="p">)</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child jp-OutputArea-executeResult">
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[ ]:</div>
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>Text(0.5, 0, 'Purchasing Power Parity Index')</pre>
</div>
</div>
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,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UW7yWbrEYjGsra0xe/ZspVnQiIiIiOjjxgQSERERERERERGpxSLaRERERERERESkFhNIRERERERERESkFhNIRERERERERESkFhNIRKRVGRkZuHv3LjIyMrQdSpnBNtMc26xw2G6aY5tpjm1GRERUNjCBRERal52dre0Qyhy2mebYZoXDdtMc20xzbDMiIqLSjwkkIiIiIiIiIiJSiwkkIiIiIiIiIiJSiwkkIiIiIiIiIiJSiwkkIiIiIiIiIiJSiwkkIiIiIiIiIiJSiwkkIiIiIiIiIiJSS0/bARARERERkXZIpVKkp6cjIyND26EQEdEHpq+vj0qVKkFHp2B9i5hAIiIiIiL6BEmlUjx//hyGhoaoXr06RCKRtkMiIqIPRCaTISMjA8+fP0e1atUKlETiEDYiIiIiok9Qeno6DA0NYWBgwOQREdEnRiQSwcDAAIaGhkhPTy/QPkwgERERERF9gjIyMqCvr6/tMIiISIv09fULPIyZCSQiIiIiok8Uex4REX3aNPk9wAQSERERERERERGpxQQSERERERERERGpxQQSERERERERERGpxQQSERERERFRKRQREQGxWAxPT09thwIbGxvY2NhoOwwqJTw9PSEWixEREaHtUOgD0tN2AEREREREVPo8/e8FkpJTtR2GStWrVoG5qXGh93/w4AGaN2+usKxcuXIwNTVFhw4dMH36dFhbWxc1TCpBnp6e8PLyUlhWsWJF1K1bF3379sXUqVNRqVIlLUX3YURERKBv374KyypUqABzc3N06dIFM2bMQJ06dT5YPPLX1bBhw+Dt7f3BzksfDhNIRERERESkJCk5FYtW+2s7DJXmTXEtUgJJrl69ehg6dCgAID09HefOncOuXbtw8OBB7N+/H7a2tkU+x8fiwIED2g5BpX79+qFJkyYAgMTERBw6dAheXl4ICQnB4cOHUb58eS1HWPJatGiBnj17AgBevnyJyMhIbNu2DQcOHMDRo0fx2WefFfs5x48fj0GDBqF27drFfmwqvZhAIiIiIiKiT5KVlRXmzp2rsGzx4sVYtmwZFi1ahKCgIC1FVvrUq1dP2yGo9NVXX2HQoEHC94sWLUL37t1x6dIl7Ny5E25ublqM7sNo2bKlwn0sk8kwceJEBAYGYtmyZSXSG6hatWqoVq1asR+XSjfWQCIiIiIiIvp/48ePBwDExsYC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zQqH7aY5tpnm2Gba8+zZszxnpgKAp/+9QFJy6geMqOCqV60Cc1NjbYdBxWjbtm2YOnUqli9fjjFjxmg7HCphzs7OCAsLw/nz52FlZaXtcD55+f0+kGOqj4iIiIiIlJibGjNJQ8UuMTERpqamCrN7PX78GL///jt0dXXRs2dPLUZHH8L169cRFhaGrl27MnlUxjCBRFQC4m4/RHa2NP8NCVJpNl6/zsSbe4+go1P83aQ/RmwzzbHNCqck2o29BoiIPm0rV65EWFgYOnToABMTEyQkJCA0NBRpaWmYM2eOUjFr+njs3LkTt27dwvbt2wHk1OCisoUJJKISsHzjHqS9+nAzK5RlUmk23rzJgIGBPh/sC4htpjm2WeGURLvNm+LKBBIR0SfMwcEBN27cQFhYGFJSUqCvr4+mTZtizJgxGDJkiLbDoxK0ZcsWnD59GhYWFli9ejXat2+v7ZBIQ0wgERERERER0Qfh4OAABwcHbYdBWhAUFKTtEKiIOAsbERERERERERGpxQQSERERERERERGpxQQSERERERERERGpxQQSERERERERERGpxQQSERERERERERGpxQQSERERERERERGpxQTSR8TDwwNisRj16tVDZmamym2cnJwgFothZmaGhw8fqtymbdu2EIvFCssiIiIgFosV/tWqVQtNmzbF4MGDsXLlSjx58kRtfNnZ2fD19UX//v3x2WefwcTEBA0bNoSzszP279+f537vn7datWpo0KABnJ2dceLECZX7eHp6Ku1Xo0YNdOjQAYsWLUJqaqraWE+dOiXst2/fPrXbEhEREREREX3s9LQdABWPtLQ07Nu3DyKRCMnJyQgKCsLAgQPz3D4zMxOLFy/Ghg0bNDpPixYt0LNnTwDAmzdvkJiYiOjoaBw5cgReXl5YsGABJkyYoLTfs2fP4OrqipiYGJibm8PR0REmJiZ49OgRwsLCEBoail69emHTpk2oVKmS0v7GxsYYN26cEHtcXJyw38aNGzF48GCV8fbr1w9NmjQRYggLC8Py5csREhKCY8eOoUKFCir3k0gkAACRSCQkvYiIiIiIiIg+VUwgfST27t2L9PR0eHh4wNvbGxKJRG0CqV69eti1axemTp0Ka2vrAp+nZcuWmDt3rtLyoKAgTJkyBbNnz0bFihXh7u4urHv79i3c3NwQExMDd3d3LF26FAYGBsL6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ZUZGRgaWLVuGa9eu4dChQzA3N8fAgQO1HRYRERERERHRR489kKjMyMjIwPLly3H69Gn06dMHQUFBMDIy0nZYRERERERERB899kCiMkMsFiM5OVnbYRARERERERF9ctgDiYiIiIiIiIiI1GICiYiIiIiIiIiI1OIQNqISkFHNHSJItR1GmSDNzsabN68hMqgIHV1dbYdTJrDNNMc2K5zS0m4yXbHWzk1EREREOZhAIioBMn0ryLQdRBmRkZGBR8nxsDC0gL6+vrbDKRPYZppjmxUO242IiIiI5DiEjYiIiIiIiIiI1GICiYiIiIiIiIiI1GICiYiIiIiIiIiI1GICiYiIiIiIiIiI1GICiYiIiIiIiIiI1OIsbEQlIO72Q2RnS7UdRpkglWbj9etMvLn3CDo6nF69INhmmmObFQ7bTVH1qlVgbmqs7TCIiIiItIIJJKISsHzjHqS9eq3tMMoEqTQbb95kwMBAnw+oBcQ20xzbrHDYbormTXFlAomIiIg+WRzCRkREREREREREajGBREREREREREREajGBRERERERERERE/8fevcdFWeb/H3/PDHLSdCQFQzEhczusZZalltpmrueyTEHU0tosNy396q6HLA9ZaHmo1Wy/33QzGYRUPGaZqXlEzbLssG1q4NmwQDzBQMw9vz9a5hcBAwPoMPB6Ph48jLmv+74+92fbR/D2vq7bLQIkAAAAAAAAuEWABAAAAAAAALcIkAAAAAAAAOAWARIAAAAAAADcIkDycUePHpXVai3yFR4ervbt22vGjBm6ePFiiefv2rXLdc7q1atLHJeQkCCr1aq5c+eWOCYuLk5Wq1XJyckljklMTHTNt3///lKvZbVaNWnSpBLHTZ482TUuLi6uxHFlvU9JOn78uMaMGaPWrVsrLCxMjRs31i233KL+/fvr9ddf16VLl9yeDwAAAABAdePn7QJQOSIjI9W/f39JktPpVEZGhj7++GPNmDFDmzdv1oYNG2SxWIqcFx8fL0kymUyy2Wzq06fPZa0zPj5eJpNJTqdTNptNrVu3djvez89Py5Yt05QpU+TnV/hf1/z8fCUlJcnPz0/5+fmlziuVfp9ff/21evXqpXPnzqlt27a6//77VadOHZ04cUIpKSnauHGjHnjgAUVFRZX9pgEAAAAA8HEESNVEVFSUJkyYUOiz3NxcdenSRfv27dPO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CggIUIcOHSRJmZmZRY4nJycrOztbMTExiomJkWEYWrp06RWrr23btmrRooVycnL0/fffFzsmPj5efn5+eu6559ShQwdt27ZNx44d83iu66+/XtHR0friiy+0atWqipYOAAAAAEC1QIAE5eXlaefOnTKZTGrZsmWR4/Hx8bJYLOrfv7969+6tOnXqKCEhQU6n84rXWtzyuv/85z/at2+f7rvvPoWGhrpCroSEhHLNMXHiRAUEBGj69On65ZdfKloyAAAAAAA+jyVsNUxqaqri4uIk/boHUmZmpjZv3qzTp09r2rRpat68eaHx3377rfbv36/OnTsrLCxMktSrVy8lJSVp+/btJe4TtHXrVtnt9mKP7dy506Oa9+zZo4MHDyokJEQtWrQocrxgf6bo6GhJUu/evTV27FglJCRo3LhxMps9y0kjIiI0bNgwzZs3T++8846GDRvm0fmS5DQcMgyHx+fVRIZhFPoTpaNnnqNn5UPfPFfVe2YYjhL/++wteXl5hf6sjgIDA71dAgAAFUaAVMOkpaVp5syZRT7v2rVrsWFQQTgTExPj+mzAgAFKSkpSfHx8iQHStm3btG3bNo/ry8/PdwVcv91E22w2a/bs2UV+APvll1/03nvvqW7duurZs6ckqU6dOurZs6eWLVumrVu36r777vO4jjFjxmjJkiV67bXXFBsbqzp16nh0/pwx98tp5Hs8LwAAl5Nhcer48ePeLqNYv307anVisVgUFRXl7TIAAKgwAqQapnPnzkpOTnZ9n5mZqT179mj8+PHq1q2b1q5dqzvuuEPSr5trL1u2TFdddZV69erlOqdDhw5q0qSJ3n//fWVlZclqtRaZZ/LkyRo9enSxNcTFxRUbYkmSw+EocszPz0+LFy8uVEOBDz74QD///LMGDx5cKFwaMGCAli1bpvj4+HIFSFarVaNHj9aUKVM0b968Iht7lyY0d6VMxiWP562JDKeh3NxcBQQEyGxiVW1Z0DPP0bPyoW+eq+o9szd8UsF1r/V2GYXk5eUpPT1dYWFh8vf393Y5AACgBARINVxISIh69Oih4OBg9enTR9OnT9fq1aslSevXr1dmZqYGDhyooKAg1zlms1n9+vXT3LlztXz5cj355JOVVk9AQIDrbyAvXryo7du3a8SIEXr66af14YcfFtmjqbgnpCSpU6dOCg8P1wcffKCzZ8+q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fTMMh+x2u9fmz8vLK/QnSlcTesZfQgEAqgMCpBokLS2t2CVhXbt2LbL3UYH58+cX+3ndunXLFSAVPN1zzTXXFHu8uA2zf79v0+XSqlUr3XzzzUpISHAFSAkJCfrjH/+oVq1aeRQgzRlzv5wGG24DwJWU46itrGzp+PHj3i5F6enp3i7B51TXnlksFkVFRXm7DAAAKowAqQbp3LmzkpOTXd9nZmZqz549Gj9+vLp166a1a9fqjjvuKHTO999/X+mbaLtTXMB1pQIkSRo0aJAmTJigTz/9VNKv9z9jxgyPrxOau1Im41Jll1ctGU5Dubm5CggIkNnEqtqyoGeeo2fl42t9szd8UvUbNPZqDXl5eUpPT1dYWJj8/f29WouvoGcAAPgGAqQaLCQkRD169FBwcLD69Omj6dOna/Xq1Zd1zoYNG0qSTp8+XezxrKws1z+3adNGhw4dKtN1TSaTnE5niccLll+Yze5/AYqOjtbkyZNdm2n7+/urf//+Zarht8wWs0w+8MtWlfDflX5mk1lmCz0rE3rmOXpWPj7WN7PFUmWWCvn7+1eZWnwFPQMAoGojQIJuv/12SdL+/fsv+1y33XabatWqpQMHDujChQuVtg9S3bp1dfbsWTmdTplMpiLHMzIyXOPcKQjVVq1aJUnq2bOnQkJCKqVGAAAAAAB8VdX/60RcdgVP/bh7gqey1K5dWw899JCys7O1YMGCSrvuTTfdpEuXLunbb78t9njBkrSbb7651GsNGjRIFy5c0IULFzRo0KBKqxEAAAAAAF9FgAS9+eabkqT27dtfkflefPFFNWjQQK+++qreeustORxF31Zmt9uVm5tb5msOGDBAkjR58uQi52VlZbk25y4Y5859992nhIQEJSQk6E9/+lOZawAAAAAAoLpiCVsNkpqaWugtZ2fPntXevXt14MABWa1WTZkypcg58+bNU+3atYu93v333682bdoU+mzRokXatGlTseMfffRRtWvXTk2aNNGqVatcG1bPnz9fHTp0UHh4uHJycnT69Gl98sknOnfunNq1a1emexs0aJA2btyo999/X7fffrv+/Oc/KyQkROnp6frggw+UkZGhp59+usS3zf2W2WxWz549yzQvAAAAAAA1AQFSDZKWllboLWcBAQEKDw/XE088oVGjRikiIqLIOfPnzy/xevXq1SsSIKWkpCglJaXY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VeWeNahfV41CQ7xdBgAAAOBWhQKkAwcOaMyYMXI4HGrXrp1Gjhypm266SY0aNdKPP/6of//735o3b552796t//mf/9Gtt96qW2+9tbJqB6qs2QtX6sLFbG+X4RMMw6GcHLuCggKr3C/2VRU981xV7tkLI2MJkAAAAFDlVWgT7fnz58vhcGjEiBH64IMP1L17d1177bUKCAjQtddeq+7du+uDDz7QyJEj5XA49Oabb1ZW3QAAAAAAALhCKhQgpaSkqF69enrxxRfdjnvhhRdUt25d7dq1qyLTAQAAAAAAwAsqFCD99NNPuu6661SrVi2342rVqqXmzZvr559/rsh0AAAAAAAA8IIKBUh16tRRenp6mcamp6erdu3aFZkOAAAAAAAAXlChAOmWW27RqVOn9MEHH7gdt379ep08eVK33HJLRaYDAAAAAACAF1QoQBo0aJCcTqeGDRum+fPnKzu78FunsrOzNW/ePD311FMymUwaPHhwhYoFAAAAAADAledXkZMfeeQRrVu3TmvXrtWLL76oV155RU2bNlVoaKjOnDmjY8eOyW63y+l06sEHH1Tfvn0rq24AAAAAAABcIRV6AkmS/vWvf2ncuHGqU6eOcnJy9P3332vHjh36/vvvlZOTozp16mj8+PFatGhRZdSL/zp69KisVmuRr/DwcLVv314zZszQxYsXC53TsmVLWa1Wt9ctbkxCQoKsVqvmzp1b5vry8/P13nvvacCAAbrxxhsVGhqq8PBw3X777Ro2bJjWrVsnwzBKPN/pdOq2226T1WpV//793c71+x5cffXVuv766xUdHa2tW7cWe05cXJysVquSk5NLvG5iYqLrmvv37y/TfQMAAAAAUB1V6AkkSbJYLBo/fryeffZZ7d69W4cOHdLFixdVp04dtWjRQm3btlVwcHBl1IpiREZGugIWp9OpjIwMffzxx5oxY4Y2b96sDRs2yGKxXNGajh07pkGDBumrr77S1VdfrU6dOikiIkKGYejo0aPatGmTli1bpp49eyohIaHYa+zYsUNpaWkymUzavHmzTp8+rWuuuabEOUNCQvTkk09KknJzc/Xdd99p48aN+uijj7Rw4UI98sgjHt9HfHy8TCaTnE6nbDabWrdu7fE1AAAAAACoDiocIBUIDg5W586d1blz58q6JMogKipKEyZMKPRZbm6uunTpon379mnnzp3q1KnTFavn/Pnz6tu3rw4dOqTnnntO48ePV1BQUKExv/zyi5YvX64NGzaUeB2bzSZJGjFihObNm6elS5dqzJgxJY6/+uqri/QhOTlZTzzxhKZOnepxgPTDDz8oJSVF3bt316FDh7RixQq9/PLLRe4FAAAAAICawOMlbD179lRISIhmz55dpvGzZ89WSEiIHnroIY+LQ/kEBASoQ4cOkqTMzMwrOvc//vEPHTp0SAMGDNDUqVOLDVxq1aql2NhY/etf/yr2GllZWVq7dq1uuukmTZw4UVdddZVsNpucTqdHtTz88MOqXbu2jh8/royMDI/OLQiwYmJiFB0drfPnz2vNmjUeXQMAAAAAgOrCowApJSVFKSkpatWqldunQX5rzJgxatWqlbZt26ZPP/20XEXCM3l5edq5c6dMJpNatmx5RedeunSpJOnvf/97qWP9/Ip/AG7FihWy2+2KiYlRUFCQHnjgAaWlpWnnzp3lrsuTZXwOh8O1/1G3bt0UHR0tk8mk+Pj4cs8PAAAAAIAv82gJW3Jyskwmk0aPHu3RJGPGjNGgQYO0fPly3XnnnR6dC/dSU1MVFxcn6dc9kDIzM117Bk2bNk3Nmze/YrUcP35cp06dUpMmTRQZGVnu68THx8tsNqtfv36SpOjoaCUkJCg+Pt71ZFVZJCcn69KlS7rxxhtL3Tz8tzZu3Kgff/xRQ4cOVUBAgJo2bap27dopJSVFqampioqKKvUaTsMhw3CUec6arGAzdXebqqMweua5qtwzw3DIbrd7u4xi5eXlFfoTpaNnnqsJPQsMDPR2CQAAVJhHAdLevXsVGBioLl26eDTJ/fffr8DAQO3du9ej81C6tLQ0zZw5s8jnXbt2vaJ7H0nSmTNnJEmNGjUq9viCBQt07ty5Qp8NHz68ULjz1Vdf6cCBA/rTn/7k2jS7Q4cOatKkidatW6dz586pXr16Ra6dkZHhCtJ+u4l2nTp1yrzcskDBk0YxMTGuz2JiYpSSkiKbzaYXX3yx1GvMGXO/nEa+R/MCqJkMi1PHjx/3dhlupaene7sEn0PPPFdde2axWMr0l08AAFR1HgVIx44dU9OmTT3+W5SAgABde+21Onr0qEfnoXSdO3cu9Cr6zMxM7dmzR+PHj1e3bt20du1a3XHHHV6s8P976623ivySFBsbWyhAKi68MZlMio6O1uzZs7VixQo98cQTRa6dmZlZJEirU6eOVq1apTZt2pS5xvT0dG3cuFFRUVG66667XJ/36dNH48aNU2Jiop5//vlSl8SF5q6UybhU5nlrMsNpKDc3VwEBATKbPN6WrUaiZ56ryj2zN3xSwXWv9XYZxcrLy1N6errCwsLk7+/v7XJ8Aj3zHD0DAMA3eBQg5eTkqE6dOuWaqE6dOsrJySnXuSi7kJAQ9ejRQ8HBwerTp4+mT5+u1atXS5LM5l9/aTIMw/XPv+d0OmUymco1d8OGDSVJP/74Y7HHv/76a9c/9+3bV5s3by503G63a9myZapTp4569+5d6FhMTIxmz54tm81WbIB0/fXXa9++fZJ+3YR7/fr1rqWTn3zyicLDw8t0D4mJicrPz1d0dHShz+vWrasePXooOTlZmzZtUteuXd1ex2wxy1TFfkmtsv670s9sMstsoWdlQs88V4V7ZrZYqvzyFn9//ypfY1VDzzxHzwAAqNo8+inaarV6/DarAhkZGcUuPcLlcfvtt0uS9u/f7/qsbt26kkp+M5vT6dTZs2dd4zzVtGlThYeH68SJE0pLS/P4/IIlahcvXlR4eLisVqvrq+Apoi+++ELffPON2+tYrVYNHDhQr776qtLT0zV27Ngy11Dw9rW4uLhC81utVteTXmymDQAAAACoaTx6Aunaa6/V/v379dNPP7meNimLM2fO6OjRo2rdurXHBaJ8srKyJP0aChW46aab9PXXX+vTTz9Vjx49ipzzzTff6NKlS2rfvn25542NjdWsWbM0a9Ysvfnmmx6dWxDM9OnTR1dddVWR46dOndLmzZsVHx9f7L5Pvzd48GAtWrRIH3zwgfbu3VtoSVpxUlJSdPjwYUVGRuqee+4pdsyHH36ojz76yOP/DwAAAAAA4Ms8CpA6dOig/fv3a9GiRRo/fnyZz1u0aJGcTqc6duzocYEon4Lw5rdhUGxsrN577z298sorat++faG9h3JzczV58mRJhfcf8tSzzz6r1atXKyEhQaGhoRo3blyRx9Hz8/OVnZ1d6LMjR45ox44datq0qd55551il9GdO3dON9xwg5YtW6Zp06YpICDAbS0mk0njxo1TbGysXn75Za1du9bt+IIAq2DpW3GmTZumOXPmKCkpSSNHjnR7PQAAAAAAqguPAqTHHntM8+fP1+uvv6577rmnxKc0fmvHjh16/fXX5efnp0cffbTchaJ4qamprrePSdLZs2e1d+9eHThwQFarVVOmTHEd69Spk55++mn985//1B133KHu3bsrLCxMmZmZ2rhxo06cOKFevXqVGJ6sXr1aBw8eLPZYz5491atXL9WtW1crV67UwIEDNXfuXC1ZskT33nuvIiIilJ+fr/T0dG3btk1nzpzRTTfd5FrWaLPZ5HQ6NWDAgBL3YKpXr5569eql5cuXa/369Xr44YdL7U+PHj3UqlUrbd++XTt37izx39nz589rzZo1ql27tvr06VPi9WJjYzVnzhzFx8cTIAEAAAAAagyPAqRmzZrp6aef1vz589W3b18999xzeuqpp3T11VcXGZuRkaF//vOf+sc//qFffvlFw4cPV7NmzSqrbvxXWlpaoeVcAQEBCg8P1xNPPKFRo0YpIiKi0PgZM2aoffv2evfdd/XBBx/o3Llzql27tm6++Wb9/e9/16BBg0rcYPvAgQM6cOBAsceaNm2qXr16uf75k08+0YoVK7Rq1Srt2rVLmZmZ8vPzU1hYmDp06KCHHnpI3bt3l8VikWEYSkxMlMlk0oABA9ze78CBA7V8+XLFx8eXKUCSpPHjxysmJkYvv/yyPvzww2LHrFy5UtnZ2RowYIDbjeKbN2+utm3bas+ePWVaFgcAAAAAQHVgysrKcpY+7P8zDEOPPvqo1q9fL5PJJLPZrBtuuEHNmjVT7dq1denSJR05ckT/+c9/ZBiGnE6nevToofj4+BKDCaC6CTo5VSbjkrfL8AmGw1COPUdBgUFV7u1YVRU981xV7pm94TAZgc29XUax7Ha7jh8/roiICN6OVUb0zHP0DAAA3+DRE0jSr6+Ct9lsmjdvnubOnauzZ8/q22+/1bfffiuTyVRo0+b69etr1KhRevbZZyu1aAAAAAAAAFw5HgdIBUaOHKknnnhCH3/8sXbv3q1Tp07pwoULuuqqqxQeHq527drp/vvvV+3atSuzXgAAAAAAAFxh5Q6QJCk4OFgPPvigHnzwwcqqBwAAAAAAAFVM1doIAgAAAAAAAFUOARIAAAAAAADcIkACAAAAAACAWxXaAwlA8exXD5ZJhrfL8AmGw6GcnGyZgoJltli8XY5PoGeeq8o9c1qs3i4BAAAAKBUBEnAZOAOj5PR2ET7Cbrfr5NnjiqgTocDAQG+X4xPomefoGQAAAFAxLGEDAAAAAACAWwRIAAAAAAAAcIsACQAAAAAAAG4RIAEAAAAAAMAtAiQAAAAAAAC4xVvYgMvgu8PH5HAY3i7DJxiGQ9nZucpJOymzuWq9Xr2qomeeo2flU1l9a1C/rhqFhlRiZQAAALjSCJCAy2D2wpW6cDHb22X4BMNwKCfHrqCgQH6xLyN65jl6Vj6V1bcXRsYSIAEAAPg4lrABAAAAAADALQIkAAAAAAAAuEWABAAAAAAAALcIkAAAAAAAAOAWARIAAAAAAADcIkACAAAAAACAWwRIAAAAAAAAcIsAyUd8+eWXGjFihFq3bq3w8HA1atRIrVq10rBhw/TJJ58Ue86lS5cUEREhq9WqsWPHlnjto0ePymq1ymq1qkWLFsrPzy923Pfff+8a17Jly0LHEhISXMcKvurXr6+mTZuqe/fustlsJc7vcDhks9nUp08fXXfddWrYsKFatGih6OhorVmzpsTzfj9fo0aN1KJFC3Xr1k2TJk3S119/7fZ++/btW+K1y9o7AAAAAABqAj9vFwD3DMPQpEmTtGDBAvn5+aljx47q3r27atWqpSNHjmjjxo1atmyZJk6cqL///e+Fzl21apUuXLggk8mk5cuXa/r06QoMDCxxLj8/P505c0YbN25Ujx49ihyPj4+X2ew+c+zUqZPatm0r6ddg6MSJE/rggw80YsQIff/993rppZcKjf/pp58UGxurffv2qVGjRurRo4caNmyokydPauPGjfroo4/UrVs3LVq0SLVr1y4yX0hIiJ588klJUn5+vjIyMvTVV19p/vz5mj9/vgYNGqTZs2crICDAbd2/52nvAAAAAACozgiQqrjp06drwYIFatmypZYsWaLIyMhCx3NycvT2228rMzOzyLk2m01+fn568skn9dZbb2ndunXq169fiXPdeeed+uabb2Sz2YoESPn5+Vq2bJnuvfde7dq1q8Rr3HvvvRo9enShz44ePar27dvr//7v/zRx4kQFBQVJkn755RcNHDhQ+/bt0+DBg/Xqq6+6jklSVlaWnnrqKW3YsEHPPPOMFi9eXGS+q6++WhMmTCjy+b///W899dRTstlsysvL0//93/+VWHNxPO0dAAAAAADVGUvYqrDU1FS98cYbCgkJUXJycpHwSJKCgoL07LPPFglRDh06pD179qhz587661//KpPJpPj4eLfzBQUFqW/fvtq4caN++umnQsc2bNigM2fOaNCgQR7fx7XXXqvmzZsrNzdXFy9edH2emJioTz/9VO3atdM//vGPQuGR9OsStcWLFysqKkqrV6/Wtm3byjznTTfdpFWrVqlBgwZatmyZPv/88zKfW57eAQAAAABQnREgVWFLly6Vw+HQ0KFDFRoa6nbs75doFQQeAwYMUEREhO655x7t2LFDR44ccXudQYMGKT8/X0lJSYU+t9lsql+/vnr27OnxfRw7dkyHDx9W48aN1bBhQ9fnCQkJkqSxY8fKZDIVe25QUJBGjBhRaHxZNWjQQEOHDpUkrVy5ssznlbd3AAAAAABUVyxhq8L27NkjSerYsaNH5xUEQPXq1VO3bt0kSdHR0dqxY4dsNpsmTZpU4rm33367brrpJi1dulQjR46UJKWnp2vTpk16/PHHS91LaOvWrbLb7ZJ+3QPp5MmT+vDDDxUcHKwFCxYUqnH//v3y8/PT3Xff7faanTp1kiR9+umnpd/879xzzz167bXXtH///jKNr0jvfstpOGQYDo/rrYkMwyj0J0pHzzxHz8qnsvpmGA7Xfxuqu7y8vEJ/onQ1oWfsowgAqA4IkKqwM2fOSJLCw8M9Oq9gudljjz3m+oHlwQcf1N///nclJiZq4sSJbjfDHjhwoJ5//nl99tlnuuOOO5SYmKj8/PwyLV/btm1bkaVmfn5+Gjp0qG666SbXZ5mZmfrll18UFhZW6g9VjRs3lvRrkOWpa665xjVfWVS0dwXmjLlfTqP4t9kBQE2S46itrGzp+PHj3i7liirPf7NquuraM4vFoqioKG+XAQBAhREgVUMFS7BiYmJcn1111VXq2bOnli9frs2bN6tLly4lnh8dHa0pU6bIZrPpjjvuUEJCgm655Rbdcsstpc49efJk1ybahmHoxx9/1Pr16zVp0iR9/PHH2rZtm+rVq1fBO7x8Ktq7AqG5K2UyLl22OqsTw2koNzdXAQEBMptYVVsW9Mxz9Kx8KqNv9oZPqn6DxpVcWdWVl5en9PR0hYWFyd/f39vl+AR6BgCAbyBAqsJCQ0N18OBBnTp1Stdff32Zzjl9+rQ2bdqkZs2aqV27doWOxcTEaPny5bLZbG5DkAYNGqhbt25auXKl+vTpo0OHDunVV1/1uH6z2azw8HA9+eSTSk9P16xZs/T2229r7NixCgkJUa1atZSRkSG73e72KaSTJ09KksLCwjyu4fTp05J+fVtbWcZWtHcFzBazTPySWjb/XelnNpllttCzMqFnnqNn5VMJfTNbLDVy+Y6/v3+NvO+KoGcAAFRt/BRdhbVt21aStH379jKfU7Dx9pEjR2S1Wgt99e3bV5L04YcfKiMjw+11Bg8erPPnz+uvf/2rAgMD1b9///LfiH7dW0mSay8iPz8/tW7dWvn5+dq1a5fbcwuWxN15550ez7tz505JUuvWrUsdW1m9AwAAAACguuEJpCosNjZWc+fO1eLFizV8+HA1aNCgxLG5ubny9/eXzWZznWuxWIqMO3jwoPbu3aukpCQ988wzJV6vc+fOCg8P16lTp9S3b19ZrdYK3UtWVpakwhuxxsbGau/evZozZ47uu+++Yt/EZrfb9eabb0r6dW8mT/z8889avHixJLkCoJI4nc5K6x0AAAAAANUNAVIVFhUVpeeee05z5szRI488osWLF6tZs2aFxtjtdi1cuFAZGRm67777lJaWpvbt2xd649lvHTp0SG3atJHNZnMbglgsFiUkJOjkyZNq2bJlhe7Dbrdr0aJFklTojWuxsbGKj4/Xrl27NHr0aM2YMaPQo+vnzp3T008/rR9++EF9+vRxvY2tLL777jsNGzZMP/30kwYMGKDbbrvN7fidO3dWWu8AAAAAAKhuCJCquEmTJslut2vBggVq06aNOnbsqBtvvFG1atXS0aNHtXXrVmVmZmrSpEmuDaDdPalz/fXX66677tLevXtdb1kryW233VZq8PJ7W7dudb2q2TAMnTlzRps2bXIFUU888YRrbK1atbR06VINGDBAixcv1kcffaQuXbqoYcOGOnXqlD766CNlZmaqa9eurqeQfi8jI0NxcXGSJIfDoczMTB04cECff/65JOnRRx/VrFmzSq27snsHAAAAAEB1QoBUxZnNZr3yyivq16+fFi1apJSUFKWkpMgwDIWFhalz584aOHCgbrvtNt1www2qXbu2HnzwQbfXHDhwoPbu3av4+PhKD0G2bdvm2rNIkmrXrq2oqCgNHTpUf/3rXxUcHFxofGhoqD766CMtXbpUK1as0Pvvv68LFy7IarWqTZs2io2NdXs/mZmZmjlzpiQpICBAdevW1XXXXaeRI0cqOjpaf/zjH0ut+dy5c1q3bp3XewcAAAAAQFVlysrKcnq7CKC6CTo5VSbjkrfL8AmG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BgAAAAAAALcIkAAAAAAAAOAWARIAAAAAAADcIkACAAAAAACAWwRIAAAAAAAAcIsACQAAAAAAAG4RIAEAAAAAAMAtAiQf8+WXX2rEiBFq3bq1wsPD1ahRI7Vq1UrDhg3TJ598UmS83W7XW2+9pe7duysyMlKhoaG66aabNGTIEG3btq3YOY4ePSqr1aq+ffuWua4DBw7or3/9q2699VY1atRITZs21b333quZM2fq3LlzxZ4zfPhwWa1WWa1W/d///V+J1x46dKhrXEJCQqFjLVu2dB0r+AoNDdUtt9yi5557TkePHi1yvbi4OFmtViUnJ5c4Z2Jiout6+/fvL2MXAAAAAAConvy8XQDKxjAMTZo0SQsWLJCfn586duyo7t27q1atWjpy5Ig2btyoZcuWaeLEifr73/8uSUpNTVX//v11+PBhNWvWTA899JDq1avnGr969WoNGTJEs2bNkp9f+f9VmDlzpmbMmCE/Pz/dd999euihh5STk6OdO3cqLi5O//rXv5SYmKjWrVsXe76fn59sNpuGDRtW5NjZs2f1wQcfyM/PT/n5+cWeb7FYNHbsWNf3586d0+eff653331X69at07Zt2xQREeHRPcXHx8tkMsnpdMpms5VYOwAAAAAANQEBko+YPn26FixYoJYtW2rJkiWKjIwsdDwnJ0dvv/22MjMzJf0aovTt21dpaWn629/+pvHjx8tisbjGnz59WgMHDtTixYtVt25dTZs2rVx1vf3224qLi1OzZs20bNkytWjRotDxd955R2PHjtUjjzyi7du3q0mTJkWucf/992vDhg36+uuv1bJly0LH3nvvPeXm5qp79+768MMPi63Bz89PEyZMKPL52LFjtXDhQi1ZskTPP/98me/phx9+UEpKirp3765Dhw5pxYoVevnllxUUFFTmawAAAAAAUJ2whM0HpKam6o033lBISIiSk5OLhEeSFBQUpGeffdYVpMybN09paWnq37+/nn/++ULhkSRdc801SkpKUv369TV//nylpqZ6XFdWVpamTZsmf39/JSUlFQmPpF+Xn40aNUqZmZl66aWXir3OgAEDZLFYFB8fX+RYQkKC/vCHP+jOO+/0uL7OnTtLkitUKyubzSZJiomJUXR0tM6fP681a9Z4PD8AAAAAANUFAZIPWLp0qRwOh4YOHarQ0FC3YwMCAiTJtVfQ3/72txLHhoaG6rHHHpNhGFq6dKnHda1Zs0YXLlxQ7969dcMNN5Q4buTIkQoMDNTKlSuVnZ1d5Hh4eLjuu+8+rVixQnl5ea7Pv/zyS3399dcaOHCgx7VJ0pYtWyRJt956a5nPcTgcrv2PunXrpujoaJlMpmLDLQAAAAAAagqWsPmAPXv2SJI6duxYpvHHjh3T6dOnFR4eruuvv97t2E6dOun111/Xp59+6nFde/fudV3DHavVqltvvVV79+7Vl19+qfbt2xcZM2jQIH388cf64IMP1KdPH0m/Pgnk5+enmJiYIptn/1Z+fr7i4uJc31+4cEH79+/Xp59+qocfflgxMTFlvqeNGzfqxx9/1NChQxUQEKCmTZuqXbt2SklJUWpqqqKiosp0HafhkGE4yjxvTWYYRqE/UTp65rnK7plhOGS32yvlWlVZQaj/23Af7tEzz9WEngUGBnq7BAAAKowAyQecOXNG0q9P6ngyvnHjxqWOLRiTnp5e7roqY54ePXro6quvls1mU58+fWS327VixQr9+c9/LvWpK4fDoZkzZxb5/KabbtJDDz0kf3//UusrUPCk0W9Dp5iYGKWkpMhms+nFF18s03XmjLlfTqP4Tb8B+D7D4tTx48e9XcYVU57/RtR09Mxz1bVnFoulzH8BBQBAVUaAhCqhVq1a6t+/v/73f/9Xp06dUkpKirKysjRo0KBSzw0ICCj0Q+fFixf1n//8R1OnTtXgwYM1c+ZMPfXUU6VeJz09XRs3blRUVJTuuusu1+d9+vTRuHHjlJiYWOx+UsUJzV0pk3Gp1HGQDKeh3NxcBQQEyGxiVW1Z0DPPVXbP7A2fVHDdayuhsqotLy9P6enpCgsL8yiMr8nomefoGQAAvoEAyQeEhobq4MGDOnXqVKlL0grGS9LJkydLHVswJiwsrFx1VeY8gwYN0ltvvaWlS5dq586dCgsL05///GeP66pTp47uuOMOxcfH6+abb9bLL7+swYMHKzg42O15iYmJys/PV3R0dKHP69atqx49eig5OVmbNm1S165dS63BbDHLxC/2ZfPflX5mk1lmCz0rE3rmuUrumdliqVFLUvz9/WvU/VYGeuY5egYAQNXGbx4+oG3btpKk7du3l2l806ZNdc011+jUqVM6dOiQ27Hbtm2TpHK95azgKZ2Ca5QkKytLBw4ckL+/v1q1alXiuJtvvlmtW7fWwoULtX37dsXExMjPr/wZp9VqVfPmzXX+/HkdPny41PEFb1+Li4uT1Wot9JWcnCxJbKYNAAAAAKiRCJB8QGxsrCwWixYvXqyff/7Z7djc3FzXOZI0a9asEsf+9NNPWrJkicxms2u8Jx588EHVqVNH69at08GDB0scN3/+fNntdj300EOlPgU0aNAg/fjjjzIMo0zL10qTlZUlqfSNc1NSUnT48GFFRkZq8ODBxX41aNBAH330kX766acK1wUAAAAAgC8hQPIBUVFReu6555SRkaFHHnlER44cKTLGbrdr/vz5mjFjhiRp5MiRuvbaa/Xee+9p5syZcjgKvxEsPT1dsbGxyszM1IgRI8q1uaPVatWkSZOUl5enmJiYYp/yWbJkiebOnauQkBC98MILpV6zf//+stlsWrFiRZmW67mzbt06HT16VFarVTfddJPbsQVPFo0ZM0bz5s0r9uvRRx/VL7/8oqSkpArVBQAAAACAr2EPJB8xadIk2e12LViwQG3atFHHjh114403qlatWjp69Ki2bt2qzMxMTZo0SZJcy6769++vuLg4JSUlqXPnzqpbt66OHDmijRs36uLFi3rsscdKfLPYv//9bw0fPrzYYy1atNDo0aP19NNPKyMjQ6+99prat2+vzp076w9/+IPsdrt27typb775RqGhoUpMTFSTJk1Kvc86deqoV69eHvUmPz9fcXFxru+zs7P1n//8R5s2bZLJZNKrr77qdlPO8+fPa82aNapdu7b69OlT4rjY2FjNmTNH8fHxGjlypEc1AgAAAADgywiQfITZbNYrr7yifv36adGiRUpJSVFKSooMw1BYWJg6d+6sgQMH6t5773Wd07x5c+3atUv/+te/tHbtWi1fvlzZ2dlq0KCBOnfurMcff1ydOnUqcc7Tp08rMTGx2GN33323Ro8eLUl6/vnn1bNnT/3zn//Url27tGXLFvn7+ysyMlLjx4/X008/LavVWpntKMThcGjmzJmu7/38/NSgQQP17t1bzzzzTKE3qhVn5cqVys7O1oABA1SnTp0SxzVv3lxt27bVnj17tHfv3lKvCwAAAABAdWHKyspyersIoLoJOjlVJuOSt8vwCYbDUI49R0GBQbxRrIzomecqu2f2hsNkBDavhMqqNrvdruPHjysiIoK3Y5URPfMcPQMAwDfwmwcAAAAAAADcIkAC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69evqygqeQKBAF9//TUEAgGWL18uN6+Jo6MjcnNzcePGDYXHX7p0CQDg5ORU6nPWrVu3/AETERERERER1WAsIJEMOzs7zJo1C5mZmfj000+Rmpoq1yY/Px/ff/89vv7666oP8C1t27aFj48PkpKScPDgQZl9n332GYA3Q99KFrqys7OlE3hL2gFAbm4u1qxZI3066W1FRUXYsGEDgDdPaRERERERERG9TziEjeQsWrQI+fn5CA4OhqurKzw8PODg4ABdXV3cu3cPMTExyMrKwqJFizQdKubPn4/jx4/jm2++waeffgodnTe39OjRoxEZGYljx46hY8eO6N27N0xMTJCeno4TJ04gMzMTX3zxhcwwvcLCQqxcuRJff/01XF1d0aZNGxgbG+PJkyeIjo7GP//8g2bNmklXZyMiIiIiIiJ6X7CARHK0tLSwatUqDB06FCEhIbhw4QIuXLgAsVgMS0tLeHt7Y9SoUejRo4emQ4WzszP69++P8PBw7Nu3D2PGjAHw5hpCQ0OxZ88e7N+/H4cOHUJubi7q16+P9u3bY+zYsRgwYIBMX8bGxvjxxx9x+vRpxMfH4+jRo8jKykKdOnXQvHlz+Pr64osvvkD9+vU1calEREREREREGiPIzs5WvlQVEZWL4T/LuApbKYlFYuTl58HQwPC9n9y4tJizsmPO/pVvPhligxala5ufj7S0NDRt2pSTG5cSc1Z2zBkREVHN8H7/Fk1ERERERERERO/EAhIREREREREREanEAhIREREREREREanEAhIREREREREREanEAhIREREREREREanEAhIREREREREREamko+kAiGqjfNMxEECs6TBqBLFIhLy8VxAY1oGWtramw6kRmLOyY87+Vawt1HQIRERERFQDsYBEVAmKDexQrOkgaoj8/Hz88ywNTes2hYGBgabDqRGYs7JjzoiIiIiIKoZD2IiIiIiIiIiISCUWkIiIiIiIiIiISCUWkIiIiIiIiIiISCUWkIiIiIiIiIiISCUWkIiIiIiIiIiISCUWkIiIiIiIiIiISCUdTQdAVBv9fec+RCKxpsOoEcRiEV69eo28lH+gpaWt6XBqBOas7Jiz8mHeyq40OTNrYIyGFiZVHBkRERFRxbCARFQJvt1+GC9evtJ0GDWCWCxCXl4+DA0N+AG1lJizsmPOyod5K7vS5GzxzJEsIBEREVGNwyFsRERERERERESkEgtIRERERERERESkEgtIRERERERERESkEgtIRERERERERESkEgtIRERERERERESkEgtIRERERERERESkUo0qIF29ehUzZsxAhw4dYGVlhYYNG6J9+/aYPHkyzpw5I2137tw5CIXCUn05OztLj7t3716Z2r/t4cOHWLZsGTw8PGBtbQ1zc3O0atUKw4YNQ1hYGAoKCuTimz17ttJrDQsLg1AoxNq1a0uVm8DAQLlYGzVqhK5du2LFihXIyclReFxpcvQ2Hx8fmX0NGjRAs2bN0LdvX4SFhaG4uFjuOqdOnao0bmVtSp5HKBTCzMwMTk5OmDhxIm7cuFGhnEnydejQIYX7y/J6EhEREREREdV2OpoOoDTEYjEWLVqE4OBg6OjowMPDA3379oWuri5SU1MRGRmJgwcPYsGCBZg3bx6sra0xf/58lX0ePHgQKSkpcHBwkNtna2uLYcOGKTyufv36ctt++uknzJw5E3l5eWjfvj2GDx8OY2NjpKenIzY2FpGRkThw4ADCw8PLl4AyGDBggPSanj59isjISHz77beIiIhAdHQ09PX15Y4xMTHBpEmTynSeGTNmwMjICCKRCPfu3cMvv/yCixcv4urVq1i9erVaruXt8wBAbm4url+/jkOHDuH48eM4ceIEXFxc1HYuier0ehIRERERERFVBzWigLRy5UoEBwfD2dkZoaGhsLW1ldmfl5eHbdu2ISsrCwDQrFkzBAQEKO3v6NGjSElJQdOmTfG///1Pbr+dnZ3K49926tQpTJ48GfXr18fevXvx4YcfyuwvLi7GsWPH8MMPP5Sqv4oaOHAghgwZIv0+Pz8fPXv2xF9//YUff/wRo0ePljvG1NS01NcrMXPmTFhaWkq/v3HjBnr27Int27dj+vTpsLGxKfc1qDoPAGzYsAFLlizB5s2bsWXLFrWcR6K6vZ5ERERERERE1UG1H8J29+5drF+/HiYmJjh06JBc8QgADA0N4efnV6oiyI0bNzBt2jQYGhpiz549MDU1LXdsIpEIc+bMgVgsxq5du+SKDQAgEAjQv39/jRUcDAwMpE9TXbt2rdLO4+TkhG7duqG4uBhXr16ttPMAgLe3NwBIC4bqUhNeTyIiIiIiIiJNqPZPIO3duxcikQjjx4+HhYWFyraKhme97dmzZxg1ahRyc3Oxbds2tGvX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xt8GiYiIiIiIiIhIJRaQiIiIiIiIiIhIJRaQiIiIiIiIiIhIJRaQiIiIiIiIiIhIJRaQiIiIiIiIiIhIJRaQiIiIiIiIiIhIJRaQiIiIiIiIiIhIJR1NB0BUG+WbjoEAYk2HUSOIRSLk5b2CwLAOtLS1NR1OjcCclR1zVj7MW9mVJmfF2sKqDYqIiIhIDVhAIqoExQZ2KNZ0EDVEfn4+/nmWhqZ1m8LAwEDT4dQIzFnZMWflw7yVHXNGREREtRWHsBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBERERERERERkUosIBGRxmlra2s6hBqHOSs75qx8mLeyY87KjjkjIiKq/gTZ2dnFmg6CiIiIiIiIiIiqLz6BREREREREREREKrGAREREREREREREKrGAREREREREREREKrGAREREREREREREKrGAREREREREREREKrGAREREREREREREKrGAREREREREREREKrGARKTClStXMHToUFhbW8PKygo9e/bEzz//XKY+Xr9+jaCgIHTo0AGWlpZo3bo1Zs2ahadPn1ZS1JpVkZwVFxcjKioK/v7+cHNzg7W1NRo1aoRu3brh22+/RX5+fiVHrznquNfelp2dDQcHBwiFQgwZMkSNkVYf6srZ06dPERAQIH2P2traolevXggJCamEqDVLHTl79OgR5s+fj86dO8PKygr29vb46KOPsH//fohEokqKXHMOHDiA//znP+jRowcsLCwgFAoRFhZW5n7EYjG2bNkCNzc3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
"/>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>As we expected it does not create any change to the PPP Index</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p><strong>Step 4</strong></p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Adding a price difference column that compares prices to the Canadian price of $5.40 CAD</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [ ]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-python"><pre><span></span><span class="n">currencyCodeTable</span> <span class="o">=</span> <span class="n">Table</span><span class="p">()</span><span class="o">.</span><span class="n">read_table</span><span class="p">(</span><span class="s1">'/content/currency_code.csv'</span><span class="p">)</span><span class="o">.</span><span class="n">where</span><span class="p">(</span><span class="s1">'WithdrawalDate'</span><span class="p">,</span> <span class="s1">'nan'</span><span class="p">)</span><span class="o">.</span><span class="n">relabel</span><span class="p">(</span><span class="s1">'Entity'</span><span class="p">,</span> <span class="s1">'Country'</span><span class="p">)</span><span class="o">.</span><span class="n">select</span><span class="p">(</span><span class="s1">'Country'</span><span class="p">,</span> <span class="s1">'Currency'</span><span class="p">,</span> <span class="s1">'AlphabeticCode'</span><span class="p">)</span><span class="o">.</span><span class="n">relabel</span><span class="p">(</span><span class="s1">'AlphabeticCode'</span><span class="p">,</span> <span class="s1">'Currency Code'</span><span class="p">)</span>

<span class="n">coffee_table_with_currency</span> <span class="o">=</span> <span class="n">coffee_table_tax</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s1">'Country'</span><span class="p">,</span> <span class="n">currencyCodeTable</span><span class="p">,</span> <span class="s1">'Country'</span><span class="p">)</span> <span class="c1"># Joining the currency data with the coffee table</span>

<span class="n">exchange_rates</span> <span class="o">=</span> <span class="n">coffee_table_with_currency</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="n">getExchangeRate</span><span class="p">,</span> <span class="s1">'Currency Code'</span><span class="p">)</span>
<span class="n">coffee_table_with_currency</span> <span class="o">=</span> <span class="n">coffee_table_with_currency</span><span class="o">.</span><span class="n">with_column</span><span class="p">(</span><span class="s1">'Latte Price in local currency'</span><span class="p">,</span> <span class="n">np</span><span class="o">.</span><span class="n">round</span><span class="p">(</span><span class="n">coffee_table_with_currency</span><span class="o">.</span><span class="n">column</span><span class="p">(</span><span class="s1">'Latte Price (USD)'</span><span class="p">)</span> <span class="o">*</span> <span class="n">exchange_rates</span><span class="p">,</span> <span class="mi">2</span><span class="p">))</span><span class="o">.</span><span class="n">with_column</span><span class="p">(</span><span class="s2">"Price Difference (CAD)"</span><span class="p">,</span> <span class="n">coffee_table_with_currency</span><span class="o">.</span><span class="n">column</span><span class="p">(</span><span class="s2">"Latte Price (CAD)"</span><span class="p">)</span> <span class="o">-</span> <span class="n">cnd_price</span><span class="p">)</span>

<span class="n">coffee_table_final</span> <span class="o">=</span> <span class="n">coffee_table_with_currency</span><span class="o">.</span><span class="n">select</span><span class="p">(</span><span class="s1">'Country'</span><span class="p">,</span> <span class="s1">'Currency'</span><span class="p">,</span> <span class="s1">'Currency Code'</span><span class="p">,</span> <span class="s1">'Latte Price in local currency'</span><span class="p">,</span> <span class="s1">'Latte Price (CAD)'</span><span class="p">,</span> <span class="s1">'Sales Tax'</span><span class="p">,</span> <span class="s1">'Price Difference (CAD)'</span><span class="p">,</span> <span class="s1">'Purchasing Power Parity'</span><span class="p">,</span> <span class="s1">'Purchasing Power Parity with tax'</span><span class="p">)</span>

<span class="n">coffee_table_final</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output" data-mime-type="text/html" tabindex="0">
<table border="1" class="dataframe">
<thead>
<tr>
<th>Country</th> <th>Currency</th> <th>Currency Code</th> <th>Latte Price in local currency</th> <th>Latte Price (CAD)</th> <th>Sales Tax</th> <th>Price Difference (CAD)</th> <th>Purchasing Power Parity</th> <th>Purchasing Power Parity with tax</th>
</tr>
</thead>
<tbody>
<tr>
<td>ANDORRA       </td> <td>Euro             </td> <td>EUR          </td> <td>3.13                         </td> <td>4.61             </td> <td>0.045    </td> <td>-0.8                  </td> <td>0.851948               </td> <td>0.852126                        </td>
</tr>
<tr>
<td>ARGENTINA     </td> <td>Argentine Peso   </td> <td>ARS          </td> <td>4719.38                      </td> <td>6.56             </td> <td>0.21     </td> <td>1.15                  </td> <td>1.21299                </td> <td>1.21257                         </td>
</tr>
<tr>
<td>AUSTRALIA     </td> <td>Australian Dollar</td> <td>AUD          </td> <td>6.13                         </td> <td>5.58             </td> <td>0.1      </td> <td>0.17                  </td> <td>1.03117                </td> <td>1.03142                         </td>
</tr>
<tr>
<td>AUSTRIA       </td> <td>Euro             </td> <td>EUR          </td> <td>3.32                         </td> <td>4.89             </td> <td>0.2      </td> <td>-0.52                 </td> <td>0.903896               </td> <td>0.903882                        </td>
</tr>
<tr>
<td>AZERBAIJAN    </td> <td>Azerbaijan Manat </td> <td>AZN          </td> <td>5.8                          </td> <td>4.79             </td> <td>0.18     </td> <td>-0.62                 </td> <td>0.885714               </td> <td>0.885397                        </td>
</tr>
<tr>
<td>BAHAMAS       </td> <td>Bahamian Dollar  </td> <td>BSD          </td> <td>3.75                         </td> <td>5.27             </td> <td>0.12     </td> <td>-0.14                 </td> <td>0.974026               </td> <td>0.974122                        </td>
</tr>
<tr>
<td>BAHRAIN       </td> <td>Bahraini Dinar   </td> <td>BHD          </td> <td>1.59                         </td> <td>5.95             </td> <td>0.1      </td> <td>0.54                  </td> <td>1.1013                 </td> <td>1.09982                         </td>
</tr>
<tr>
<td>BELGIUM       </td> <td>Euro             </td> <td>EUR          </td> <td>3.35                         </td> <td>4.94             </td> <td>0.21     </td> <td>-0.47                 </td> <td>0.914286               </td> <td>0.913124                        </td>
</tr>
<tr>
<td>BOLIVIA       </td> <td>Boliviano        </td> <td>BOB          </td> <td>22.08                        </td> <td>4.48             </td> <td>0.13     </td> <td>-0.93                 </td> <td>0.828571               </td> <td>0.828096                        </td>
</tr>
<tr>
<td>BRAZIL        </td> <td>Brazilian Real   </td> <td>BRL          </td> <td>11.89                        </td> <td>2.75             </td> <td>0.22     </td> <td>-2.66                 </td> <td>0.509091               </td> <td>0.508318                        </td>
</tr>
<tr>
<td>BULGARIA      </td> <td>Bulgarian Lev    </td> <td>BGN          </td> <td>4.98                         </td> <td>3.78             </td> <td>0.2      </td> <td>-1.63                 </td> <td>0.698701               </td> <td>0.698706                        </td>
</tr>
<tr>
<td>CAMBODIA      </td> <td>Riel             </td> <td>KHR          </td> <td>13083.8                      </td> <td>4.56             </td> <td>0.1      </td> <td>-0.85                 </td> <td>0.844156               </td> <td>0.842884                        </td>
</tr>
<tr>
<td>CANADA        </td> <td>Canadian Dollar  </td> <td>CAD          </td> <td>5.41                         </td> <td>5.41             </td> <td>0.109981 </td> <td>0                     </td> <td>1                      </td> <td>1                               </td>
</tr>
<tr>
<td>CHILE         </td> <td>Chilean Peso     </td> <td>CLP          </td> <td>4841.76                      </td> <td>6.95             </td> <td>0.19     </td> <td>1.54                  </td> <td>1.28571                </td> <td>1.28466                         </td>
</tr>
<tr>
<td>CHINA         </td> <td>Yuan Renminbi    </td> <td>CNY          </td> <td>30.72                        </td> <td>5.94             </td> <td>0.13     </td> <td>0.53                  </td> <td>1.0987                 </td> <td>1.09797                         </td>
</tr>
<tr>
<td>COLOMBIA      </td> <td>Colombian Peso   </td> <td>COP          </td> <td>11140.9                      </td> <td>3.51             </td> <td>0.19     </td> <td>-1.9                  </td> <td>0.649351               </td> <td>0.648799                        </td>
</tr>
<tr>
<td>COSTA RICA    </td> <td>Costa Rican Colon</td> <td>CRC          </td> <td>2144.1                       </td> <td>5.93             </td> <td>0.13     </td> <td>0.52                  </td> <td>1.0961                 </td> <td>1.09612                         </td>
</tr>
<tr>
<td>CYPRUS        </td> <td>Euro             </td> <td>EUR          </td> <td>2.83                         </td> <td>4.17             </td> <td>0.19     </td> <td>-1.24                 </td> <td>0.771429               </td> <td>0.770795                        </td>
</tr>
<tr>
<td>CZECH REPUBLIC</td> <td>Czech Koruna     </td> <td>CZK          </td> <td>94.48                        </td> <td>5.52             </td> <td>0.21     </td> <td>0.11                  </td> <td>1.02078                </td> <td>1.02033                         </td>
</tr>
</tbody>
</table>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>We will import a table for the longitude and latitude of each country so we can map each country and add a label for their currency.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [ ]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-python"><pre><span></span><span class="n">ccll</span> <span class="o">=</span> <span class="n">Table</span><span class="o">.</span><span class="n">read_table</span><span class="p">(</span><span class="s2">"/content/country_capitals_lat_long.csv"</span><span class="p">)</span>

<span class="n">ccll</span> <span class="o">=</span> <span class="n">ccll</span><span class="o">.</span><span class="n">with_column</span><span class="p">(</span><span class="s1">'Country'</span><span class="p">,</span> <span class="n">ccll</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="n">capitalize</span><span class="p">,</span> <span class="s1">'Country'</span><span class="p">))</span>
<span class="n">coffee_table_tax</span> <span class="o">=</span> <span class="n">coffee_table_tax</span><span class="o">.</span><span class="n">with_column</span><span class="p">(</span><span class="s1">'Country'</span><span class="p">,</span> <span class="n">coffee_table_tax</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="n">capitalize</span><span class="p">,</span> <span class="s1">'Country'</span><span class="p">))</span>

<span class="n">mapping_table</span> <span class="o">=</span> <span class="n">coffee_table_final</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">"Country"</span><span class="p">,</span> <span class="n">ccll</span><span class="p">,</span> <span class="s2">"Country"</span><span class="p">)</span><span class="o">.</span><span class="n">select</span><span class="p">(</span><span class="s2">"Country"</span><span class="p">,</span> <span class="s2">"Currency Code"</span><span class="p">,</span> <span class="s2">"Continent"</span><span class="p">,</span> <span class="s2">"Capital"</span><span class="p">,</span> <span class="s2">"Code"</span><span class="p">,</span> <span class="s2">"Longitude"</span><span class="p">,</span> <span class="s2">"Latitude"</span><span class="p">)</span><span class="o">.</span><span class="n">relabel</span><span class="p">(</span><span class="s2">"Code"</span><span class="p">,</span> <span class="s2">"Country Code"</span><span class="p">)</span>
<span class="n">mapping_table</span> <span class="o">=</span> <span class="n">mapping_table</span><span class="o">.</span><span class="n">relabel</span><span class="p">(</span><span class="s2">"Currency Code"</span><span class="p">,</span> <span class="s2">"labels"</span><span class="p">)</span>

<span class="k">def</span> <span class="nf">continent_colour</span><span class="p">(</span><span class="n">continent</span><span class="p">):</span>
  <span class="k">if</span> <span class="n">continent</span> <span class="o">==</span> <span class="s2">"Asia"</span><span class="p">:</span>
    <span class="k">return</span> <span class="s2">"green"</span>
  <span class="k">elif</span> <span class="n">continent</span> <span class="o">==</span> <span class="s2">"Europe"</span><span class="p">:</span>
    <span class="k">return</span> <span class="s2">"red"</span>
  <span class="k">elif</span> <span class="n">continent</span> <span class="o">==</span> <span class="s2">"Africa"</span><span class="p">:</span>
    <span class="k">return</span> <span class="s2">"orange"</span>
  <span class="k">elif</span> <span class="n">continent</span> <span class="o">==</span> <span class="s2">"North America"</span><span class="p">:</span>
    <span class="k">return</span> <span class="s2">"grey"</span>
  <span class="k">elif</span> <span class="n">continent</span> <span class="o">==</span> <span class="s2">"South America"</span><span class="p">:</span>
    <span class="k">return</span> <span class="s2">"orange"</span>
  <span class="k">else</span><span class="p">:</span>
    <span class="k">return</span> <span class="s2">"black"</span>

<span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="n">mapping_table</span><span class="o">.</span><span class="n">num_rows</span><span class="p">):</span>
      <span class="k">if</span> <span class="n">mapping_table</span><span class="o">.</span><span class="n">column</span><span class="p">(</span><span class="s2">"Country"</span><span class="p">)</span><span class="o">.</span><span class="n">item</span><span class="p">(</span><span class="n">i</span><span class="p">)</span> <span class="o">==</span> <span class="s2">"CANADA"</span><span class="p">:</span>
        <span class="n">mapping_table</span><span class="p">[</span><span class="s2">"Continent"</span><span class="p">][</span><span class="n">i</span><span class="p">]</span> <span class="o">=</span> <span class="s2">"North America"</span>

<span class="n">mapping_table</span> <span class="o">=</span> <span class="n">mapping_table</span><span class="o">.</span><span class="n">with_column</span><span class="p">(</span><span class="s2">"color"</span><span class="p">,</span> <span class="n">mapping_table</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="n">continent_colour</span><span class="p">,</span> <span class="s2">"Continent"</span><span class="p">))</span>

<span class="n">Marker</span><span class="o">.</span><span class="n">map_table</span><span class="p">(</span><span class="n">mapping_table</span><span class="o">.</span><span class="n">select</span><span class="p">(</span><span class="s1">'Latitude'</span><span class="p">,</span> <span class="s1">'Longitude'</span><span class="p">,</span> <span class="s1">'labels'</span><span class="p">,</span><span class="s1">'color'</span><span class="p">))</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="application/vnd.jupyter.stderr" tabindex="0">
<pre>/usr/local/lib/python3.10/dist-packages/datascience/maps.py:548: UserWarning: color argument of Icon should be one of: {'orange', 'black', 'darkred', 'lightred', 'blue', 'cadetblue', 'darkpurple', 'lightgray', 'beige', 'darkgreen', 'red', 'white', 'purple', 'gray', 'lightgreen', 'pink', 'darkblue', 'green', 'lightblue'}.
  attrs['icon'] = folium.Icon(**icon_args)
</pre>
</div>
</div>
<div class="jp-OutputArea-child jp-OutputArea-executeResult">
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[ ]:</div>
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html" tabindex="0">
<div style="width:100%;"><div style="position:relative;width:100%;height:0;padding-bottom:60%;"><span style="color:#565656">Make this Notebook Trusted to load map: File -&gt; Trust Notebook</span><iframe allowfullscreen="" mozallowfullscreen="" srcdoc='&lt;!DOCTYPE html&gt;
&lt;html&gt;
&lt;head&gt;
    
    &lt;meta http-equiv="content-type" content="text/html; charset=UTF-8" /&gt;
    
        &lt;script&gt;
            L_NO_TOUCH = false;
            L_DISABLE_3D = false;
        &lt;/script&gt;
    
    &lt;style&gt;html, body {width: 100%;height: 100%;margin: 0;padding: 0;}&lt;/style&gt;
    &lt;style&gt;#map {position:absolute;top:0;bottom:0;right:0;left:0;}&lt;/style&gt;
    &lt;script src="https://cdn.jsdelivr.net/npm/leaflet@1.9.3/dist/leaflet.js"&gt;&lt;/script&gt;
    &lt;script src="https://code.jquery.com/jquery-3.7.1.min.js"&gt;&lt;/script&gt;
    &lt;script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/js/bootstrap.bundle.min.js"&gt;&lt;/script&gt;
    &lt;script src="https://cdnjs.cloudflare.com/ajax/libs/Leaflet.awesome-markers/2.0.2/leaflet.awesome-markers.js"&gt;&lt;/script&gt;
    &lt;link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/leaflet@1.9.3/dist/leaflet.css"/&gt;
    &lt;link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/css/bootstrap.min.css"/&gt;
    &lt;link rel="stylesheet" href="https://netdna.bootstrapcdn.com/bootstrap/3.0.0/css/bootstrap-glyphicons.css"/&gt;
    &lt;link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.2.0/css/all.min.css"/&gt;
    &lt;link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/Leaflet.awesome-markers/2.0.2/leaflet.awesome-markers.css"/&gt;
    &lt;link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/python-visualization/folium/folium/templates/leaflet.awesome.rotate.min.css"/&gt;
    
            &lt;meta name="viewport" content="width=device-width,
                initial-scale=1.0, maximum-scale=1.0, user-scalable=no" /&gt;
            &lt;style&gt;
                #map_d00338a2ea93316dce07ba1c46eede42 {
                    position: relative;
                    width: 960.0px;
                    height: 500.0px;
                    left: 0.0%;
                    top: 0.0%;
                }
                .leaflet-container { font-size: 1rem; }
            &lt;/style&gt;
        
&lt;/head&gt;
&lt;body&gt;
    
    
            &lt;div class="folium-map" id="map_d00338a2ea93316dce07ba1c46eede42" &gt;&lt;/div&gt;
        
&lt;/body&gt;
&lt;script&gt;
    
    
            var map_d00338a2ea93316dce07ba1c46eede42 = L.map(
                "map_d00338a2ea93316dce07ba1c46eede42",
                {
                    center: [7.783333330000001, 32.525],
                    crs: L.CRS.EPSG3857,
                    zoom: 1,
                    zoomControl: true,
                    preferCanvas: false,
                    clusteredMarker: false,
                    includeColorScaleOutliers: true,
                    radiusInMeters: false,
                }
            );

            

        
    
            var tile_layer_4cb4afff0889649c7e5fd6f21d0ee033 = L.tileLayer(
                "https://tile.openstreetmap.org/{z}/{x}/{y}.png",
                {"attribution": "\u0026copy; \u003ca href=\"https://www.openstreetmap.org/copyright\"\u003eOpenStreetMap\u003c/a\u003e contributors", "detectRetina": false, "maxNativeZoom": 19, "maxZoom": 17, "minZoom": -1, "noWrap": false, "opacity": 1, "subdomains": "abc", "tms": false}
            );
        
    
            tile_layer_4cb4afff0889649c7e5fd6f21d0ee033.addTo(map_d00338a2ea93316dce07ba1c46eede42);
        
    
            var marker_b76d47c0b9156ad87611cb38731e2695 = L.marker(
                [42.5, 1.516667],
                {}
            ).addTo(map_d00338a2ea93316dce07ba1c46eede42);
        
    
            var icon_4d74180b40783993bc454f018f85617e = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "sign-blank", "iconColor": "white", "markerColor": "red", "prefix": "glyphicon"}
            );
            marker_b76d47c0b9156ad87611cb38731e2695.setIcon(icon_4d74180b40783993bc454f018f85617e);
        
    
        var popup_5c3018d0a028424a4340218d556614d5 = L.popup({"maxWidth": "100%"});

        
            
                var html_631a81afc11ae3c748eeb1bed305c104 = $(`&lt;div id="html_631a81afc11ae3c748eeb1bed305c104" style="width: 100.0%; height: 100.0%;"&gt;EUR&lt;/div&gt;`)[0];
                popup_5c3018d0a028424a4340218d556614d5.setContent(html_631a81afc11ae3c748eeb1bed305c104);
            
        

        marker_b76d47c0b9156ad87611cb38731e2695.bindPopup(popup_5c3018d0a028424a4340218d556614d5)
        ;

        
    
    
            var marker_b1b1aa49d2355d659eec81015807ac70 = L.marker(
                [-34.58333333, -58.666667],
                {}
            ).addTo(map_d00338a2ea93316dce07ba1c46eede42);
        
    
            var icon_8fa2ee240f70dfe6f40edacd0d8bb737 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "sign-blank", "iconColor": "white", "markerColor": "orange", "prefix": "glyphicon"}
            );
            marker_b1b1aa49d2355d659eec81015807ac70.setIcon(icon_8fa2ee240f70dfe6f40edacd0d8bb737);
        
    
        var popup_4ad58fcd70ab0827d7a01ed8bd294136 = L.popup({"maxWidth": "100%"});

        
            
                var html_2b83eb13c233fd52309077e912783bc5 = $(`&lt;div id="html_2b83eb13c233fd52309077e912783bc5" style="width: 100.0%; height: 100.0%;"&gt;ARS&lt;/div&gt;`)[0];
                popup_4ad58fcd70ab0827d7a01ed8bd294136.setContent(html_2b83eb13c233fd52309077e912783bc5);
            
        

        marker_b1b1aa49d2355d659eec81015807ac70.bindPopup(popup_4ad58fcd70ab0827d7a01ed8bd294136)
        ;

        
    
    
            var marker_45c853ec6c2551228390da42ef620e84 = L.marker(
                [-35.26666667, 149.133333],
                {}
            ).addTo(map_d00338a2ea93316dce07ba1c46eede42);
        
    
            var icon_01e64a5f21cea99266968f85234bb7dc = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "sign-blank", "iconColor": "white", "markerColor": "black", "prefix": "glyphicon"}
            );
            marker_45c853ec6c2551228390da42ef620e84.setIcon(icon_01e64a5f21cea99266968f85234bb7dc);
        
    
        var popup_95a6c92c6a4d19a2b378bb581fa371b8 = L.popup({"maxWidth": "100%"});

        
            
                var html_504daded354ece1cc9883a19c6ef19f6 = $(`&lt;div id="html_504daded354ece1cc9883a19c6ef19f6" style="width: 100.0%; height: 100.0%;"&gt;AUD&lt;/div&gt;`)[0];
                popup_95a6c92c6a4d19a2b378bb581fa371b8.setContent(html_504daded354ece1cc9883a19c6ef19f6);
            
        

        marker_45c853ec6c2551228390da42ef620e84.bindPopup(popup_95a6c92c6a4d19a2b378bb581fa371b8)
        ;

        
    
    
            var marker_eb66e284025c12da013763624eb6059c = L.marker(
                [48.2, 16.366667],
                {}
            ).addTo(map_d00338a2ea93316dce07ba1c46eede42);
        
    
            var icon_4b29e77684cf4a51a163687c5d1dbe44 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "sign-blank", "iconColor": "white", "markerColor": "red", "prefix": "glyphicon"}
            );
            marker_eb66e284025c12da013763624eb6059c.setIcon(icon_4b29e77684cf4a51a163687c5d1dbe44);
        
    
        var popup_d8fc01d8b5f728c7619cad5d6d40d58b = L.popup({"maxWidth": "100%"});

        
            
                var html_8fdc232116d9f284170096f7ca1909ba = $(`&lt;div id="html_8fdc232116d9f284170096f7ca1909ba" style="width: 100.0%; height: 100.0%;"&gt;EUR&lt;/div&gt;`)[0];
                popup_d8fc01d8b5f728c7619cad5d6d40d58b.setContent(html_8fdc232116d9f284170096f7ca1909ba);
            
        

        marker_eb66e284025c12da013763624eb6059c.bindPopup(popup_d8fc01d8b5f728c7619cad5d6d40d58b)
        ;

        
    
    
            var marker_2fd1358543055d63403f03ec4d676620 = L.marker(
                [40.38333333, 49.866667],
                {}
            ).addTo(map_d00338a2ea93316dce07ba1c46eede42);
        
    
            var icon_91d6e3c2beaf501f11247de4bd854ae0 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "sign-blank", "iconColor": "white", "markerColor": "red", "prefix": "glyphicon"}
            );
            marker_2fd1358543055d63403f03ec4d676620.setIcon(icon_91d6e3c2beaf501f11247de4bd854ae0);
        
    
        var popup_c627c4015465ba72d9b94749acc46c13 = L.popup({"maxWidth": "100%"});

        
            
                var html_f9dc68ba06a83908c552ee0ae9f1791f = $(`&lt;div id="html_f9dc68ba06a83908c552ee0ae9f1791f" style="width: 100.0%; height: 100.0%;"&gt;AZN&lt;/div&gt;`)[0];
                popup_c627c4015465ba72d9b94749acc46c13.setContent(html_f9dc68ba06a83908c552ee0ae9f1791f);
            
        

        marker_2fd1358543055d63403f03ec4d676620.bindPopup(popup_c627c4015465ba72d9b94749acc46c13)
        ;

        
    
    
            var marker_b6099ad28af0282fbc0b647f794859d1 = L.marker(
                [25.08333333, -77.35],
                {}
            ).addTo(map_d00338a2ea93316dce07ba1c46eede42);
        
    
            var icon_d1732cc468bbe6da53737c1501d7d5c6 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "sign-blank", "iconColor": "white", "markerColor": "grey", "prefix": "glyphicon"}
            );
            marker_b6099ad28af0282fbc0b647f794859d1.setIcon(icon_d1732cc468bbe6da53737c1501d7d5c6);
        
    
        var popup_36b8057d2cec301aa39c1babadf529b5 = L.popup({"maxWidth": "100%"});

        
            
                var html_4b7fe2d359a330d06bee6a11d216c343 = $(`&lt;div id="html_4b7fe2d359a330d06bee6a11d216c343" style="width: 100.0%; height: 100.0%;"&gt;BSD&lt;/div&gt;`)[0];
                popup_36b8057d2cec301aa39c1babadf529b5.setContent(html_4b7fe2d359a330d06bee6a11d216c343);
            
        

        marker_b6099ad28af0282fbc0b647f794859d1.bindPopup(popup_36b8057d2cec301aa39c1babadf529b5)
        ;

        
    
    
            var marker_7f96fe5e27d07f438b4dc56cd5b3384b = L.marker(
                [26.23333333, 50.566667],
                {}
            ).addTo(map_d00338a2ea93316dce07ba1c46eede42);
        
    
            var icon_e3d97936dac46b0a9c5762504d02e85c = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "sign-blank", "iconColor": "white", "markerColor": "green", "prefix": "glyphicon"}
            );
            marker_7f96fe5e27d07f438b4dc56cd5b3384b.setIcon(icon_e3d97936dac46b0a9c5762504d02e85c);
        
    
        var popup_1895748596a49c3dae6c0050a56564b8 = L.popup({"maxWidth": "100%"});

        
            
                var html_f3962de05e2821439eefea5b7df1cfb3 = $(`&lt;div id="html_f3962de05e2821439eefea5b7df1cfb3" style="width: 100.0%; height: 100.0%;"&gt;BHD&lt;/div&gt;`)[0];
                popup_1895748596a49c3dae6c0050a56564b8.setContent(html_f3962de05e2821439eefea5b7df1cfb3);
            
        

        marker_7f96fe5e27d07f438b4dc56cd5b3384b.bindPopup(popup_1895748596a49c3dae6c0050a56564b8)
        ;

        
    
    
            var marker_fa9affef6bf9305ea2b3acc7e695c96f = L.marker(
                [50.83333333, 4.333333],
                {}
            ).addTo(map_d00338a2ea93316dce07ba1c46eede42);
        
    
            var icon_52409bfff00c9e1593588bdc4e94c15f = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "sign-blank", "iconColor": "white", "markerColor": "red", "prefix": "glyphicon"}
            );
            marker_fa9affef6bf9305ea2b3acc7e695c96f.setIcon(icon_52409bfff00c9e1593588bdc4e94c15f);
        
    
        var popup_cd5c4e0178c64a381a68b87558d37f96 = L.popup({"maxWidth": "100%"});

        
            
                var html_9e3e6505edf399cca90faa74935dee25 = $(`&lt;div id="html_9e3e6505edf399cca90faa74935dee25" style="width: 100.0%; height: 100.0%;"&gt;EUR&lt;/div&gt;`)[0];
                popup_cd5c4e0178c64a381a68b87558d37f96.setContent(html_9e3e6505edf399cca90faa74935dee25);
            
        

        marker_fa9affef6bf9305ea2b3acc7e695c96f.bindPopup(popup_cd5c4e0178c64a381a68b87558d37f96)
        ;

        
    
    
            var marker_eec6ee0741132ab7fd1ed331f3ecb3c9 = L.marker(
                [-16.5, -68.15],
                {}
            ).addTo(map_d00338a2ea93316dce07ba1c46eede42);
        
    
            var icon_1f4c8bcf0e26fe8caafd0626bc424e8c = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "sign-blank", "iconColor": "white", "markerColor": "orange", "prefix": "glyphicon"}
            );
            marker_eec6ee0741132ab7fd1ed331f3ecb3c9.setIcon(icon_1f4c8bcf0e26fe8caafd0626bc424e8c);
        
    
        var popup_86891d1de09959dcbac0cb9aa48f3272 = L.popup({"maxWidth": "100%"});

        
            
                var html_8bf49f49810e5b57b87a85bc7712dbf2 = $(`&lt;div id="html_8bf49f49810e5b57b87a85bc7712dbf2" style="width: 100.0%; height: 100.0%;"&gt;BOB&lt;/div&gt;`)[0];
                popup_86891d1de09959dcbac0cb9aa48f3272.setContent(html_8bf49f49810e5b57b87a85bc7712dbf2);
            
        

        marker_eec6ee0741132ab7fd1ed331f3ecb3c9.bindPopup(popup_86891d1de09959dcbac0cb9aa48f3272)
        ;

        
    
    
            var marker_971f3bb36a87748af07b50b8226f0e93 = L.marker(
                [-15.78333333, -47.916667],
                {}
            ).addTo(map_d00338a2ea93316dce07ba1c46eede42);
        
    
            var icon_00fe82647d7ae11cdc3354afdc31eb5d = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "sign-blank", "iconColor": "white", "markerColor": "orange", "prefix": "glyphicon"}
            );
            marker_971f3bb36a87748af07b50b8226f0e93.setIcon(icon_00fe82647d7ae11cdc3354afdc31eb5d);
        
    
        var popup_01360af8a874d3f4e17c720fd4fd3e8a = L.popup({"maxWidth": "100%"});

        
            
                var html_e2c5fa73e43206b717676f344710396b = $(`&lt;div id="html_e2c5fa73e43206b717676f344710396b" style="width: 100.0%; height: 100.0%;"&gt;BRL&lt;/div&gt;`)[0];
                popup_01360af8a874d3f4e17c720fd4fd3e8a.setContent(html_e2c5fa73e43206b717676f344710396b);
            
        

        marker_971f3bb36a87748af07b50b8226f0e93.bindPopup(popup_01360af8a874d3f4e17c720fd4fd3e8a)
        ;

        
    
    
            var marker_9d530fc0de458f9de808c25afb4952e3 = L.marker(
                [42.68333333, 23.316667],
                {}
            ).addTo(map_d00338a2ea93316dce07ba1c46eede42);
        
    
            var icon_bb84aafd34007c7ba82b44e7d77a9d54 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "sign-blank", "iconColor": "white", "markerColor": "red", "prefix": "glyphicon"}
            );
            marker_9d530fc0de458f9de808c25afb4952e3.setIcon(icon_bb84aafd34007c7ba82b44e7d77a9d54);
        
    
        var popup_08c1b4fed8848b8859848feb5e0a9b4a = L.popup({"maxWidth": "100%"});

        
            
                var html_a9c0743d1c2ed1739c9e8f0d1e577f96 = $(`&lt;div id="html_a9c0743d1c2ed1739c9e8f0d1e577f96" style="width: 100.0%; height: 100.0%;"&gt;BGN&lt;/div&gt;`)[0];
                popup_08c1b4fed8848b8859848feb5e0a9b4a.setContent(html_a9c0743d1c2ed1739c9e8f0d1e577f96);
            
        

        marker_9d530fc0de458f9de808c25afb4952e3.bindPopup(popup_08c1b4fed8848b8859848feb5e0a9b4a)
        ;

        
    
    
            var marker_c0f9ea6499c58d8706b09285ad84ca08 = L.marker(
                [11.55, 104.916667],
                {}
            ).addTo(map_d00338a2ea93316dce07ba1c46eede42);
        
    
            var icon_b36d25c4b614bd305eb3906364421eae = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "sign-blank", "iconColor": "white", "markerColor": "green", "prefix": "glyphicon"}
            );
            marker_c0f9ea6499c58d8706b09285ad84ca08.setIcon(icon_b36d25c4b614bd305eb3906364421eae);
        
    
        var popup_9bbfef5030aa46fe986029b805ebbc88 = L.popup({"maxWidth": "100%"});

        
            
                var html_81a6dbd16e63dbe517a4d0960c930f0c = $(`&lt;div id="html_81a6dbd16e63dbe517a4d0960c930f0c" style="width: 100.0%; height: 100.0%;"&gt;KHR&lt;/div&gt;`)[0];
                popup_9bbfef5030aa46fe986029b805ebbc88.setContent(html_81a6dbd16e63dbe517a4d0960c930f0c);
            
        

        marker_c0f9ea6499c58d8706b09285ad84ca08.bindPopup(popup_9bbfef5030aa46fe986029b805ebbc88)
        ;

        
    
    
            var marker_bcfde36ba6d526d2f6de1c658c5a02fd = L.marker(
                [45.41666667, -75.7],
                {}
            ).addTo(map_d00338a2ea93316dce07ba1c46eede42);
        
    
            var icon_816e6b150d35638587817b382946e294 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "sign-blank", "iconColor": "white", "markerColor": "grey", "prefix": "glyphicon"}
            );
            marker_bcfde36ba6d526d2f6de1c658c5a02fd.setIcon(icon_816e6b150d35638587817b382946e294);
        
    
        var popup_b2c552c6735993bd41ed6740d0565b74 = L.popup({"maxWidth": "100%"});

        
            
                var html_1372b81c1d4bccbb278bad613a27e900 = $(`&lt;div id="html_1372b81c1d4bccbb278bad613a27e900" style="width: 100.0%; height: 100.0%;"&gt;CAD&lt;/div&gt;`)[0];
                popup_b2c552c6735993bd41ed6740d0565b74.setContent(html_1372b81c1d4bccbb278bad613a27e900);
            
        

        marker_bcfde36ba6d526d2f6de1c658c5a02fd.bindPopup(popup_b2c552c6735993bd41ed6740d0565b74)
        ;

        
    
    
            var marker_96c0e10d9cc6bd49f6b5fab5eb0ec066 = L.marker(
                [-33.45, -70.666667],
                {}
            ).addTo(map_d00338a2ea93316dce07ba1c46eede42);
        
    
            var icon_a866cafe2aa8db20c7111d7786bfd157 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "sign-blank", "iconColor": "white", "markerColor": "orange", "prefix": "glyphicon"}
            );
            marker_96c0e10d9cc6bd49f6b5fab5eb0ec066.setIcon(icon_a866cafe2aa8db20c7111d7786bfd157);
        
    
        var popup_722b7e832462e5be8296047f975cc449 = L.popup({"maxWidth": "100%"});

        
            
                var html_c9107b364da0a460026bbc1f066a9aba = $(`&lt;div id="html_c9107b364da0a460026bbc1f066a9aba" style="width: 100.0%; height: 100.0%;"&gt;CLP&lt;/div&gt;`)[0];
                popup_722b7e832462e5be8296047f975cc449.setContent(html_c9107b364da0a460026bbc1f066a9aba);
            
        

        marker_96c0e10d9cc6bd49f6b5fab5eb0ec066.bindPopup(popup_722b7e832462e5be8296047f975cc449)
        ;

        
    
    
            var marker_8862aecc178bc515bc9a50e31a1857b9 = L.marker(
                [39.91666667, 116.383333],
                {}
            ).addTo(map_d00338a2ea93316dce07ba1c46eede42);
        
    
            var icon_b5711c6a612e579d3c0b0a6bd9165175 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "sign-blank", "iconColor": "white", "markerColor": "green", "prefix": "glyphicon"}
            );
            marker_8862aecc178bc515bc9a50e31a1857b9.setIcon(icon_b5711c6a612e579d3c0b0a6bd9165175);
        
    
        var popup_d62a6ab76ec16e8b528920fe14725904 = L.popup({"maxWidth": "100%"});

        
            
                var html_15957001aa3f10e9b0f01bbd3bf4ce64 = $(`&lt;div id="html_15957001aa3f10e9b0f01bbd3bf4ce64" style="width: 100.0%; height: 100.0%;"&gt;CNY&lt;/div&gt;`)[0];
                popup_d62a6ab76ec16e8b528920fe14725904.setContent(html_15957001aa3f10e9b0f01bbd3bf4ce64);
            
        

        marker_8862aecc178bc515bc9a50e31a1857b9.bindPopup(popup_d62a6ab76ec16e8b528920fe14725904)
        ;

        
    
    
            var marker_5ae362211eedef740f1c343fc35d1a3f = L.marker(
                [4.6, -74.083333],
                {}
            ).addTo(map_d00338a2ea93316dce07ba1c46eede42);
        
    
            var icon_8994bfa9ee686956a0ab2088a391e557 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "sign-blank", "iconColor": "white", "markerColor": "orange", "prefix": "glyphicon"}
            );
            marker_5ae362211eedef740f1c343fc35d1a3f.setIcon(icon_8994bfa9ee686956a0ab2088a391e557);
        
    
        var popup_6980bd33d159e0fa251ffbf6c8b05a6d = L.popup({"maxWidth": "100%"});

        
            
                var html_5052fcd2e652e32800cd46bf1cd077cd = $(`&lt;div id="html_5052fcd2e652e32800cd46bf1cd077cd" style="width: 100.0%; height: 100.0%;"&gt;COP&lt;/div&gt;`)[0];
                popup_6980bd33d159e0fa251ffbf6c8b05a6d.setContent(html_5052fcd2e652e32800cd46bf1cd077cd);
            
        

        marker_5ae362211eedef740f1c343fc35d1a3f.bindPopup(popup_6980bd33d159e0fa251ffbf6c8b05a6d)
        ;

        
    
    
            var marker_bf5a4f7ca611613ab7bb8886469f1b50 = L.marker(
                [9.933333333, -84.083333],
                {}
            ).addTo(map_d00338a2ea93316dce07ba1c46eede42);
        
    
            var icon_86e50939db668c6c6b69ef6ae84f8dc0 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "sign-blank", "iconColor": "white", "markerColor": "black", "prefix": "glyphicon"}
            );
            marker_bf5a4f7ca611613ab7bb8886469f1b50.setIcon(icon_86e50939db668c6c6b69ef6ae84f8dc0);
        
    
        var popup_89d5de6e2e099d2757bad4c9cea196cc = L.popup({"maxWidth": "100%"});

        
            
                var html_cb419e789774a8a9fe609ac498f88eea = $(`&lt;div id="html_cb419e789774a8a9fe609ac498f88eea" style="width: 100.0%; height: 100.0%;"&gt;CRC&lt;/div&gt;`)[0];
                popup_89d5de6e2e099d2757bad4c9cea196cc.setContent(html_cb419e789774a8a9fe609ac498f88eea);
            
        

        marker_bf5a4f7ca611613ab7bb8886469f1b50.bindPopup(popup_89d5de6e2e099d2757bad4c9cea196cc)
        ;

        
    
    
            var marker_4e0506b62fde1419436e03d3d9eac421 = L.marker(
                [35.16666667, 33.366667],
                {}
            ).addTo(map_d00338a2ea93316dce07ba1c46eede42);
        
    
            var icon_7db85549d3cb0ea32e6f28dae6c959d7 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "sign-blank", "iconColor": "white", "markerColor": "red", "prefix": "glyphicon"}
            );
            marker_4e0506b62fde1419436e03d3d9eac421.setIcon(icon_7db85549d3cb0ea32e6f28dae6c959d7);
        
    
        var popup_edbae31975131cf15d29f4a0a3834a75 = L.popup({"maxWidth": "100%"});

        
            
                var html_1b6113d516350436594e6c2dbfcc29b3 = $(`&lt;div id="html_1b6113d516350436594e6c2dbfcc29b3" style="width: 100.0%; height: 100.0%;"&gt;EUR&lt;/div&gt;`)[0];
                popup_edbae31975131cf15d29f4a0a3834a75.setContent(html_1b6113d516350436594e6c2dbfcc29b3);
            
        

        marker_4e0506b62fde1419436e03d3d9eac421.bindPopup(popup_edbae31975131cf15d29f4a0a3834a75)
        ;

        
    
    
            var marker_0f724597aa76641bf23ca5f8f56d1fba = L.marker(
                [50.08333333, 14.466667],
                {}
            ).addTo(map_d00338a2ea93316dce07ba1c46eede42);
        
    
            var icon_11c1c80b538b41dcba6c6a8ac3c21fd2 = L.AwesomeMarkers.icon(
                {"extraClasses": "fa-rotate-0", "icon": "sign-blank", "iconColor": "white", "markerColor": "red", "prefix": "glyphicon"}
            );
            marker_0f724597aa76641bf23ca5f8f56d1fba.setIcon(icon_11c1c80b538b41dcba6c6a8ac3c21fd2);
        
    
        var popup_6aedd5f8db40a1409e0748c613ff24eb = L.popup({"maxWidth": "100%"});

        
            
                var html_fef9e121aa14e9a12ad59b1e742eab01 = $(`&lt;div id="html_fef9e121aa14e9a12ad59b1e742eab01" style="width: 100.0%; height: 100.0%;"&gt;CZK&lt;/div&gt;`)[0];
                popup_6aedd5f8db40a1409e0748c613ff24eb.setContent(html_fef9e121aa14e9a12ad59b1e742eab01);
            
        

        marker_0f724597aa76641bf23ca5f8f56d1fba.bindPopup(popup_6aedd5f8db40a1409e0748c613ff24eb)
        ;

        
    
&lt;/script&gt;
&lt;/html&gt;' style="position:absolute;width:100%;height:100%;left:0;top:0;border:none !important;" webkitallowfullscreen=""></iframe></div></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p><strong>Step 5</strong></p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [ ]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-python"><pre><span></span><span class="n">coffee_table_final</span><span class="o">.</span><span class="n">sort</span><span class="p">(</span><span class="s2">"Price Difference (CAD)"</span><span class="p">,</span> <span class="n">descending</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span><span class="o">.</span><span class="n">barh</span><span class="p">(</span><span class="s2">"Country"</span><span class="p">,</span> <span class="s2">"Price Difference (CAD)"</span><span class="p">)</span>
<span class="n">plots</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">"Differences of Latte Prices Around the World to a Canadian Latte"</span><span class="p">)</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child jp-OutputArea-executeResult">
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[ ]:</div>
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>Text(0.5, 1.0, 'Differences of Latte Prices Around the World to a Canadian Latte')</pre>
</div>
</div>
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,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6BiMEhERERERkdExGCUiIiIiIiKjYzBKRERERERERsdglIiIiIiIiIyOwSgREREREREZHYNRIiIiIiIiMjoGo0RERERERGR0DEaJiIiIiIjI6BiMEhERERERkdExGCUiIiIiIiKjYzBKRERERERERsdglIiIiIiIiIyOwSgREREREREZHYNRIiIiIiIiMjoGo0RERERERGR0pmVdASIiInpzvFSIcSvuAcRik7KuCpWAXJ6P7Oxc5LxlbVizujVq29qUdTWI3joMRomIiMhgnj3PwcqNO9+qQOZNIpfnIydHBktLi7eqDRf6ejMYJSoD7KZLRERERERERsdglIiIiIiIiIyOwSgREREREREZHYNRIiIiIiIiMjoGo0RERERERGR0DEaJiIiIiIjI6BiMEhERERERkdExGKVSdfnyZUydOhVt27aFvb09ateujdatW2PixIk4evSokG7ZsmWQSCQIDQ3VuK7JkydDIpHg/Pnzhd6XSCRo3759ofcCAgIgkUiwatWqIuuoLFvba9myZcXcciIiIiIi0sa0rCtAbya5XI4FCxbAz88Ppqam6N69O/r164dKlSohPj4eERERCAkJwfz58/Hll1+WdXUBAAMHDkSTJk3ULuvatauRa0NERERE9GZjMEqlYsmSJfDz80OLFi2wdetWODs7F1qek5OD9evXIzU1tYxqqGrQoEEYOnRoWVeDiIiIiOitwGCUDC42Nha//vorbGxsEBoaCltbW5U0lpaWmDZtGnJzc8ughkREREREVNY4ZpQMLjAwEPn5+RgzZozaQLQgc3NzI9WKiIiIiIjKE94ZJYM7e/YsAKB79+7Fzrtr1y7cunVL7bIrV67oVS99yh47dizs7Oy05pfJZKVRLdJRXl5eoX+p4mEbVnzKtpPL5WVcEyopZdu9bW0ol+cb/DxuYWFh0PURvYkYjJLBPX78GABgb29f7Ly7d+/G7t27DV0lvct2dXUtMhhNSkpCfn5+aVSNiiE5Obmsq0B6YhtWfLm5vKBQ0b1tbZidnYOEhASDrc/ExAQuLi4GWx/Rm4rBKJUrGzdu1DiJ0OTJkxEUFFQmZeuiJME3GU5eXh6Sk5NhZ2cHMzOzsq4OlQDbsOLLy8tDSsZ9mJubQSzmSKCKSC6XIzc3761rw8qVLeHgULesq0H01mEwSgZna2uLW7duISkpCQ0bNizr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POImMzMTYWFhqFKlCjZv3gwrKyuV/HK5HC1atMChQ4eEcWxERERERGQYDEaN5MSJE7h37x66dOmiMRAFAB8fH0RHR0MqlRYZjNra2mLs2LFYu3Yt/Pz8MHfuXGHZmjVrIBaLsX37drRq1QrdunVDo0aNYGZmhsePH+PixYu4ceMGatSogUaNGqmsW9ujXYBXgXBRd1zt7Ozw+eef46efftKarrRYWlpi7ty5mDZtGp4/f15o2d9//43MzEyMGDFCbSAKvBov4+XlhZUrVyIoKAgzZswwQq2JiIiIiN4OHDNqJMouod7e3lrTDR48GJaWltixYwdycnKKXO/06dNRuXJl+Pn5IT09XXjf0tIS69evx549ezBo0CDcvn0bmzZtwtq1axEZGYl69eph5cqVuHTpkvBIk4KUj3bR9NL1+WHTpk1DjRo1dEpbGnx8fPDuu++qvO/v7w+g6PZQLlemJyIiIiIiwxClp6cryroSRET6kslkSEhIgIODA2dxrKDYhhWfTCbD5Wt3sHLjTs6mW0HJ5fnIyZHB0tKixG240Ncbzd91MmzFiOiNxDujREREREREZHQMRomIiIiIiMjoGIwSERERERGR0TEYJSIiIiIiIqNjMEpERERERERGx2CUiIiIiIiIjM60rCtAREREb45qVS2x0Nebj3apoOTyfGRn56ByZcsSt2HN6tYGrhURvakYjBIREZHBmIrkcHbms2Irqv8977cu25CISh276RIREREREZHRMRglIiIiIiIio2MwSkREREREREbHYJSIiIiIiIiMjsEoERERERERGR1n0yUiIiKDeakQ41bcg7fq0S41q1ujtq1NWVeDiKjCYTBKREREBvPseQ5Wbtz5VgWjC329GYwSEZUAu+kSERERERGR0TEYJSIiIiIiIqNjMEpERERERERGx2CUiIiIiIiIjI7BKBERERERERkdg1EiIiIiIiIyOgajREREREREZHQMRt9g9+7dg0QiUXnZ29ujc+fOWL58OTIzMzXmP336tJAnLCxMY7qAgABIJBKsWrVKY5ply5ZBIpEgNDS00PstWrQoVDcbGxs4Oztj4MCBWstUmjJlCiQSCZydnZGbm6sxnaurKyQSCZKTk4X3Cn4+Q4YMUZvv/PnzkEgkmDx5cpF1ISIiIiIi3ZmWdQWo9Dk7O8PDwwMAoFAokJKSgkOHDmH5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4p1RIiIiIiIiMjoGo0RERERERGR0DEaJiIiIiIjI6BiMEhERERERkdExGCUiIiIiIiKjYzBKRERERERERmda1hUgIiKiN0e1qpZY6Ov9Vj3apWZ167KuAhFRhcRglIiIiAzGVCSHszOfUUlEREVjN10iIiIiIiIyOgajREREREREZHQMRomIiIiIiMjoGIwSERERERGR0TEYJSIiIiIiIqNjMEpERERERERGx0e7EBERkcG8VIhxK+7BW/Gc0ZrVrVHb1qasq0FEVGExGCUiIiKDefY8Bys37nwrgtGFvt4MRomI9MBuukRERERERGR0DEaJiIiIiIjI6BiMEhERERERkdExGCUiIiIiIiKjYzBKRERERERERsdglIiIiIiIiIyOwSgZzOXLlzF16lS0bdsW9vb2qF27Nlq3bo2JEyfi6NGjQrply5ZBIpEgNDRU47omT54MiUSC8+fPF3pfIpGgffv2hd4LCAiARCKBRCLBzz//rHZ9q1atgkQiQUBAgMYyg4KChPVcvHhRl00mIiIiIqISYjBKepPL5Zg/fz4++OADBAcHw8nJCWPGjMGkSZPQunVrREREYPDgwfjhhx9KvS6//PIL0tLSSpRXKpVCJBIBAPz9/Q1ZLSIiIiIieo1pWVeAKr4lS5bAz88PLVq0wNatW+Hs7FxoeU5ODtavX4/U1NRSrYezszPi4uLw008/4fvvvy9W3rt37yIqKgr9+vXD7du3sWPHDnz//fewtLQspdoSEREREb3deGeU9BIbG4tff/0VNjY2CA0NVQlEAcDS0hLTpk3DvHnzSrUu3t7ecHFxwYYNG5CQkFCsvMo7oV5eXvD09ERGRgZ27dpVGtUkIiIiIiIwGCU9BQYGIj8/H2PGjIGtra3WtObm5qVaF1NTUyxcuBC5ubnFujOan58vjBft27cvPD09IRKJIJVKS7G2RERERERvN3bTJb2cPXsWANC9e/di5921axdu3bqldtmVK1dKVB93d3esXr0aISEhmDp1Kpo3b15knoiICDx69AhjxoyBubk5HB0d0alTJ0RFRSE2NhYuLi4lqgsREREREWnGYJT08vjxYwCAvb19sfPu3r0bu3fvNmh9RCIRFi9ejIEDB+Kbb77B9u3bi8yjvAPq5eUlvOfl5YWoqCj4+/vj66+/1qlsmUxWskqTQeTl5RX6lyoetmHFp2w7uVxexjUxDrk8/4079nM/NBwLC4uyrgJRucdglMrMxo0bMXToULXLJk+ejKCgoBKtt3v37ujduzcOHTqEU6dOoWvXrhrTJicnIyIiAi4uLujQoYPwvru7O+bMmYOgoCB89dVXMDExKbLcpKQk5Ofnl6jOZDjJycllXQXSE9uw4svNfTsCmezsnGLPUVBRcD/Uj4mJCXtWEemAwSjpxdbWFrdu3UJSUhIaNmxY1tURLFq0CJGRkVi0aBGOHDmiMV1QUBBevnwJT0/PQu9bW1ujf//+CA0NxeHDh9GnT58iyyzJ3WEynLy8PCQnJ8POzg5mZmZlXR0qAbZhxZeXl4eUjPswNzeDWPzmT0tRubIlHBzqlnU1DIr7IREZE4NR0kvHjh1x6tQpnDhxAj169Cjr6ghatGiB4cOHY9u2bQgLC9OYTjmL7rJly7Bs2TK1aaRSqU7BKLvjlA9mZmZsiwqObVjxicViiMVF9yip6MRikzf2u8r9kIiMgcEo6cXb2xurVq3Cli1bMHnyZNSsWVNj2tzc3FKfUbegr776CmFhYfjuu+8KjQdVioqKwp07d+Ds7KyxK+/+/ftx8OBBPHnyBLVq1SrtKhMRERERvTUYjJJeXFxcMH36dPz8888YNmwYtmzZAicnp0JpZDIZNmzYgJSUFCxatMhodXN0dMS4cePg5+eHwMBAleXKiYtmzZqFkSNHql3Ht99+i59//hnBwcHw9fUt1foSEREREb1NGIyS3hYsWACZTAY/Pz+0b98e3bt3R5MmTVCpUiXcu3cPx44dQ2pqKhYsWGD0us2ePRv+/v6Ii4sr9H5GRgZ27dqFKlWqwN3dXWN+b29v/Pzzz5BKpQxGiYiIiIgM6M2fXYBKnVgsxtKlS3H06FF4enoiLi4OGzduhJ+fH/755x/06tULYWFhmD17ttHrZmNjgxkzZqi8//fffyM7OxsDBw6ElZWVxvwNGjRAx44dcevWLZw7d64Ua0pERERE9HYRpaenK8q6EkRE+pLJZEhISICDgwMn3aig2IYVn0wmw+Vrd7By4863YgKjhb7eaP6uU1lXw6C4HxKRMfHOKBERERERERkdg1EiIiIiIiIyOgajREREREREZHQMRomIiIiIiMjoGIwSERERERGR0TEYJSIiIiIiIqMzLesKEBER0ZujWlVLLPT1fise7VKzunVZV4GIqEJjMEpEREQGYyqSw9mZz6gkIqKisZsuERERERERGR2DUSIiIiIiIjI6BqNERERERERkdAxGiYiIiIiIyOgYjBIREREREZHRMRglIiIiIiIio+OjXYiIiMhgXirEuBX34I1/zmjN6taobWtT1tUgIqrQGIwSERGRwTx7noOVG3e+8cHoQl9vBqNERHpiN10iIiIiIiIyOgajREREREREZHQMRomIiIiIiMjoGIwSERERERGR0TEYJSIiIiIiIqNjMEpERERERERGx2CUiIiIiIiIjI7BqBFdvnwZU6dORdu2bWFvb4/atWujdevWmDhxIo4ePao2j0wmw7p169CvXz84OzvD1tYWTZs2xejRo3H8+HGNZWVlZWHlypXo3r076tatK+Tr168fvvnmG8TFxQEAJk+eDIlEovMrICCgUDlubm6QSCTo1KlTiT4TdeXXq1cPPXr0wK+//orc3FyVPPfu3YNEIsHQoUPVrvPly5fw9/fH8OHD0ahRI9SqVQuOjo748MMPsWTJEty/f19jfYKCgoR6XLx4sUTbRERERERERTMt6wq8DeRyORYsWAA/Pz+Ympqie/fu6NevHypVqoT4+HhEREQgJCQE8+fPx5dffinki42NhYeHB+7cuQMnJycMHjwY1apVE/KEhYVh9OjR+Omnn2Bq+r+mfP78Ofr27Ytr167BxcUFHh4esLGxQUpKCi5cuIBVq1bB2dkZzs7OcHV1haOjY6H6njp1CqdPn0b//v3RokWLQssK/j8+Ph6nTp2CSCTCjRs38M8//6Bdu3Yl+oxGjRoFe3t7KBQKPHr0CHv37sWiRYtw4sQJhIaG6rye+/fvw9vbG1evXoWtrS0++OAD1KtXD1lZWfj333+xatUqrF69GmfOnIGLi4tKfqlUCpFIBIVCAX9/f7Rt27ZE20NERERERNoxGDWCJUuWwM/PDy1atMDWrVvh7OxcaHlOTg7Wr1+P1NRU4b1nz55h6NChiIuLwxdffIG5c+fCxMREWP7w4UP4+Phgy5YtsLa2xrfffissW7duHa5du4ZPPvkEv/76K0QiUaHy4uPjkZeXBwAYMGAABgwYUGj5smXLcPr0abi6usLHx0fjdvn7+0OhUMDX1xerV6+GVCotcTD6ySefoH379sL/Fy9ejC5duuDIkSM4ceIEunfvXuQ6nj9/jqFDh+L27duYNm0avvrq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BBITEzFgwACMHDmy0HrWrl2L5cuXo02bNmjdujWqV6+O1NRUnDx5Enfu3IGNjQ2WLFlSatvbv39/tG7dGidOnMCpU6cQGxuLzMxMjBgxQuOdWbFYLIzhDAoKwowZM4RlL168wOTJkzWWt27dOrXv+/v7Q6FQYMSIERrH1VarVg0DBgzA9u3bER4ejiFDhui+oUREREREpBWD0TKm7Crq7e2tNd3gwYMxd+5c7NixA99//z0sLS2xfPlydO7cGX/99Rf27duHZ8+eoUqVKmjWrBm+/PJLjBw5UmVyo+DgYBw6dAinT5/G/v378fTpU5ibm6N+/frw9fXFlClT1HaVNaS5c+fCy8sL33//vfAolKK239vbW5hQqGAwKpfLtU62pC4YVeYRiUQYMWKE1nJ9fHywfft2SKVSBqNERERERAYkSk9PV5R1JYiI9CWTyZCQkAAHBwfOAFlBsQ0rPplMhsvX7mDlxp0GmU13oa83mr/rpH/FSGfcD4nImDibLhERERERERkdg1EiIiIiIiIyOgajREREREREZHQMRomIiIiIiMjoGIwSERERERGR0TEYJSIiIiIiIqPjc0aJiIjIYKpVtcRCX2+DPNqlZnVrA9SIiIjKKwajREREZDCmIjmcnfmMSiIiKhq76RIREREREZHRMRglIiIiIiIio2MwSkREREREREbHYJSIiIiIiIiMjsEoERERERERGR1n0yUiIiKDeakQ41bcA50f7VKzujVq29qUcq2IiKg8YjBKREREBvPseQ5WbtypczC60NebwSgR0VuK3XSJiIiIiIjI6BiMEhERERERkdExGCUiIiIiIiKjYzBKRERERERERsdglIiIiIiIiIyOwSgREREREREZHYNRIiIiIiIiMrpyH4xevnwZU6dORdu2bWFvb4/atWujdevWmDhxIo4ePSqkO3nyJCQSiU6vFi1aCPnu3btXrPQFJSUl4ZtvvkH37t3h6OiIWrVq4d1334WHhwcCAgKQl5enUr+ZM2dq3NaAgABIJBKsWrVKp89m2bJlKnWtU6cOOnXqhO+++w4ZGRlq8+nyGRXk6upaaFn16tVRv3599OvXDwEBAVAoFCrbOXnyZI311pTm9XIkEglq1qyJZs2aYfz48bh27Zpen5ny8woNDVW7vDjtSURERERE+jEt6wpoIpfLsWDBAvj5+cHU1BTdu3dH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IzY2FpaWlvjpp5+EdcvlcgQEBEAkEsHb21tjeYMHD8a8efMQEhKC7777juNniIiIiIgMhMHoW0YsFmPp0qUYPnw4Nm7ciKioKERFRUEul8POzg69evWCj48P2rRpg8aNG6NKlSoYNGiQ1nX6+Pjg3LlzkEqlRQajwKu7k693i719+zbOnDmD+vXro2vXrlrrP2LECPz0008IDAzErFmzhGWXL1/G5cuXAQCVK1dG9erV0bhxY3zyySfw8vJC7dq1hbTHjh1DYmIiunTponJ3uKBq1arBzc0NISEh2LNnD4YPH17k9hERERERUdFE6enpirKuBBGRvmQyGRISEuDg4MA72BUU27Dik8lkyMrKQpUqVdiGFRT3QyIyJs6mS0REREREREbHYJSIiIiIiIiMjsEoERERERERGR2DUSIiIiIiIjI6BqNERERERERkdAxGiYiIiIiIyOgYjBIREZHBZGdnl3UViIiogmAwSkRERAYjk8nKugpERFRBMBglIiIiIiIio2MwSkREREREREbHYJSIiIiIiIiMjsEoERERERERGR2DUSIiIiIiIjI6BqNERERERERkdKZlXQEiIiIqPx49TsXTtIwS5ZXL81HJhNe5iYhINwxGiYiISPA0LQPfrQ4sUV65PB+zxg02cI2IiOhNxcuXREREREREZHQMRomIiIiIiMjoGIwSERERERGR0TEYJSIiIiIiIqNjMEpERERERERGx2CUiIiIiIiIjI7BaAV07949SCQSlZe9vT06d+6M5cuXIzMzU2P+06dPC3nCwsI0pgsICIBEIsGqVas0plm2bBkkEglCQ0M1pgkKChLKu3jxYpHrkkgkWLBggcZ0ixYtEtItW7ZMYzpdtxMAEhISMGvWLLRt2xZ2dnaoW7cuWrZsCQ8PD/zyyy/IysrSmp+IiIiIiIqHzxmtwJydneHh4QEAUCgUSElJwaFDh7B8+XIcOXIEBw4cgImJiUo+qVQKABCJRPD394e7u3up1lMqlUIkEkGhUMDf3x9t27bVmt7U1BQhISFYvHgxTE0Lf0VfvnyJ4OBgmJqa4uXLl0WWCxS9nVeuXMGAAQPw7NkzdOzYEb1794aVlRUSExMRFRWFiIgIDBw4EC4uLrpvNBERERERacVgtAJzcXHBvHnzCr2Xm5uLjz76COfPn8epU6fQo0ePQsszMjKwe/duNGvW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8rsMAEAhkeOPL69du6b69etn2a5+/fq6du1aTg8DAAAAAHgE5TiMFitWTNevX8+y3fXr11WsWLGcHgYAAAAA8AjKcRitW7euQkND9fvvv2fY5sSJEzpw4IDq1q2b08MAAAAAAB5BOQ6jr776qu7du6fu3bvrq6++0u3bt03bbt++rS+++EI9evRQUlKSBgwYkBu1AgAAAAAeETmewKhXr17avn27VqxYoffff1/vv/++nJ2dJUmRkZGSpOTkZHl7e6tnz565Uy0AAAAA4JHwUPOvf/bZZ5o7d64qV66s5ORkRUREKCIiQsnJyapSpYrmzZunJUuW5FatAAAAAIBHRI6vjKZ47bXX9NprryksLExXr16VJJUrV05ubm4PXRwAAAAA4NGUrSujR48e1ebNm3XmzJk029zc3NS4cWM1btxYbm5uOnPmjDZv3qxffvkl14pF7hg6dKgMBoOqVq2q+Pj4dNvUrVtXBoMh034yanPp0iWNGjVKjRo1kqurq8qXL6969eqpT58++u9//6s7d+6k2t/crwsXLkhSmsdLlSqlGjVqyMvLK8M1bWfMmCGDwaDVq1dn+HyCgoJMfR49ejTT5w4AAADg4Zh9ZTQiIkIvvfSSHB0dtW/fvizblyhRQqNHj9bdu3f166+/ZhlsYBm3bt3SunXrZGVlpaioKG3atClX7+k9fvy4unbtqps3b6pZs2Zq3769HB0ddfnyZYWGhiokJEQvvvii3N3dNWTIEN28eTPV/oGBgbp06ZIGDx6sEiVKpNr24PfOzs564403JEnx8fH6888/FRISom3btumrr75S7969s127n5+frKyslJycLH9/fzVq1CgHrwAAAAAAc5gdRlesWKHbt29r+vTpKl26dJbtS5curXHjxumdd97RypUr9eabbz5Uocgda9eu1Z07dzR06FAtWbJEfn5+uRpGP/jgA928eVOfffaZvL2902w/fPiwaaKrt99+O832/fv369KlSxoyZIgqV66c4XFKlSqlcePGpXps9erVGjRokCZPnpztMHrmzBmFhoaqc+fOOnXqlFatWqXp06fLwcEhW/0AAAAAMI/Zw3S3b9+u4sWLy8fHx+zOvb295ejoqG3btuWoOOQ+Pz8/2dra6t1331XLli21Z88eXbx4Mdf6P3LkiEqUKJFuEJWkZ555Js+ukvfs2VPFixfXpUuX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uenJJ59Ux44d9d5772nPnj1KTk7OsI+XXnpJFStWVHh4eOYvAADAbLb5XQAAPG6aNWumqlWrSpJu3rypX3/9VWvXrtW6des0depUDRs2LJ8rzH3FixfXiy++KEkyGo2KiYnRhQsXtGbNGq1atUoffPCBJk6cqLfeektWVlZm97tt2zYNGzZMRYsWVevWreXs7CxJcnR0lCQtXbpUH374oZycnNS+fXs98cQTuf/kYHLjxg3NnDlTjRo10ksvvZRum08++UTTp09XQkKCHB0d1bhxY5UpU0a3bt3SH3/8oc8//1yff/653nnnHU2ZMiXdPjZv3qyIiAhJ0rVr17Rt27YMP6x40NNPP626detKku7du6fIyEidOHFChw4d0pdffqk6depo8eLFql+/fpp9J02apOeff16TJ0/W4sWLzX1JAACZIIwCgIX1799fffv2NX0fFxenESNGKDg4WB999JE6deqk6tWrm93fRx99pJEjR8rV1TUvys0Vzs7OWrJkSZrH//nnH33yySf67LPPNHbsWIWFhaUJII0bN9bhw4fl4OCQZv9169ZJkmbNmqVXX301zfa1a9dKkr799ls9//zzufBMkJlZs2bp5s2bGjt2bLrbJ02apP/+978qUqSIpk6dqjfffFP29vap2hw5ckRTp07V6dOnMzyOn5+fJMnNzU1hYWHy8/MzK4x6enpq3LhxaR4PDQ3VxIkT9fPPP6tz587atGmTGjZsmKpNw4YN1bFjRwUFBWnIkCGmUAsAyDmG6QJAPitatKjmzJmj4sWLKykpSRs3bszW/mXLllXNmjVVokSJPKow75QtW1YzZszQ//3f/0mSPv300zTDlYsVK6aaNWuqYsWKafa/fPmyJMnd3T3d/rPajtwTHR2twMBAubm5qX379mm279mzR//9738lSV9//bWGDx+eJohKUtOmTbV+/foMRwhcvnxZP/zwg2xsbPTNN9/IyspK27dv1z///JPj2ps3b64tW7bIw8NDd+/e1euvv66kpKQ07fr376/k5GR99tlnOT4WAOB/CKMAUAA4OjqaroZevHjR9PiD9zj6+/urQ4cOqlSpUqr7IrO6Z/TXX3/V4MGDVa9ePbm6uqpKlSpq0aKFJk6cmOpYKa5evarx48frmWeeUbly5VShQgU9//zz+uKLL7K8Ny+nXn/9dTVq1EjS/WGcD0rvntGU57xv3z5JUrdu3Uyv1ZAhQ0z3CKa8RvXr1zdtnzFjRqr+T58+rREjRqhBgwZydXVVpUqV1LlzZ61YsSLdWlP63rdvn0JDQ+Xl5aVq1aqpZMmSqc5BbGysFixYoPbt26tSpUpydXVVkyZN9OGHHyoyMjJNvyn31w4ZMkR37tzR5MmT1bBhQ7m4uKhmzZoaPHiwwsLCMnwNw8LCNHHiRDVv3lwVKlSQm5ubGjdurCFDhujQoUNp2me3vqwEBATozp078vLykrV12j8vUj5w6Ny5s7p165ZpX1ZWVmrevHm62/z9/WU0GtW+fXs9++yzatWqlZKSkhQUFJTtmh9kZ2enefPmSZLOnDmj77//Pk2bjh07qlSpUlq9erWioqIe6ngAAMIoABQYt27dknT/j+J/e++99/TOO+/I1tZWL7zwgpo0aWLWvZWffvqp2rZtq+DgYNnZ2alLly5q1qyZEhMTtWDBAlOYS3HgwAF5eHho8eLFiouLU5s2bfTss8/q3Llzev/999WnTx/du3cvd57wv/Tp08dUQ1ah18PDQz4+PnJxcZEktWvXTj4+PvLx8ZGHh4fat28vHx8fFS9eXJL04osvmrY/OLxy3bp1eu6557Rs2TLZ2dmpQ4cOatCggX777Te99dZbGjp0aIY1rF+/Xl27dtWFCxfUpk0bPf/886YrfVevXlW7du00ceJEnTlzRo0aNVKHDh0UHx+vTz/9VG3atEn3gwBJiomJ0QsvvKCvv/5aTz75pNq3b6/k5GQFBwerY8eOunnzZpp99uzZIw8PDy1YsEDXr19Xq1at9MILL6hEiRJatWqVli1blqr9w9SXkU2bNkmS2rRpk2ZbdHS06Yq3j49Ptvp9UHJysinw9+vXL9W/uTGBV61atVSvXj1J0u7du9NsL1KkiJ577jnFxcVp586dD308AHjccc8oABQAJ06c0Pnz5yUp3XvRVqxYoW3btqlp06Zm97l582Z9+OGHKlq0qJYsWaIePXqk2v7XX3+lCrTh4eHq37+/bt68qblz52rgwIGmK1yRkZEaMGCAdu3apXnz5mnMmDE5eJaZa9CggSTp9u3bunTpkmmSp/S88soreuWVV+Tp6alr165pxIgRatmyZZp2+/fv1507dzR16lRVrlw51bbfQ68JqAAACrBJREFUf//dNGHS8uXLTRMsSfevTnt7eysgIEDPPfdcugHqq6++0pw5c/T666+nejw5OVkDBw7UH3/8of79++vjjz82TZyUmJioSZMmaeHChRo6dGi6Q7I3bdqkdu3aacuWLXJycpJ0P8x169ZNx48f19KlS/Wf//zH1P7y5cvq37+/YmJiNHLkSI0bNy7VBxrXr19Pdf/lw9aXntjYWP3000+ytrY2XeF+0LFjx2Q0GiUp3e3m2r17ty5duqQyZcqoU6dOku5fFS9RooROnz6t0NDQDK+omivlw4i//vor3e3PPPOM1q9frz179qh3794PdSwAeNxxZRQA8tHNmzcVEhKi/v37y2g0qly5cmlCoyQNGzYsW0FUkmk46oQJE9Lt86mnntKTTz5p+n7JkiWKjIzU66+/rkGDBqUaauns7KzPPvtMRYoU0ZdffpnpEhg5VapUKdN/52SYaHbNnTtX8fHx+uCDD1IFUUmqVKmSFi5cKEn6/PPP092/VatWaYKoJO3cuVMHDx5U3bp1NX/+/FQz+Nra2mrKlCmqXbu29u3bpz/++CPN/sWLF9eiRYtMQVS6P1x75MiRktJesVu0aJFiYmLUqVMnffTRR2murJcpU0YeHh65Vl96/vrrLyUkJMjNzS3dGYtTZr5NqSenUiYu8vLyUpEiRSTdv+f65ZdfTrX9YaT8HGb0M1irVi1J9wM2AODhEEYBwMKGDh1qun+xcuXK6tOnj86dO6eqVatq5cqVpqGlD8pomYyMhIeH6/jx47K2tlb//v3N2ickJESS1LNnz3S3u7m5qVq1arpx44bOnDmTrXrMkXLlTFK2lnfJ6bF27NghKePn27BhQzk6Ouq3335TXFxcmu0ZnZNt27ZJuj802NY27QAka2tr09W7w4cPp9neoEEDlS1bNs3jNWvWlHR/iO2DUoaLDhgwIN16cru+9Fy7dk2STEvr5IXIyEjTUOCUobkpUr5fv369abh7TqX8HGb0M5jyHK9fv/5QxwEAMEwXACzuwXVG7ezsVKZMGTVp0kTt27dPNxxI96/UZUfKLLJly5Y1e5bdlGHCnTt3zrLtjRs3srX8jDkevHpWsmTJXO373yIjIxUTEyNJqlOnjlnt3dzcUj2W0TlJmTRp+vTpmj59eqb93rhxI81jFSpUSLdtyhXHfwfjS5cuSfpfWM3Kw9aXnpTXMqN1XB+86n39+vUMn2NmVqxYofj4eDVp0kRPPfVUqm0NGjRQnTp19Pvvv2vNmjXpLvNjrpSfw4x+BlOeY3R0dI6PAQC4jzAKABb273VGzZHeGpu5LeWK0EsvvaRixYpl2jYvroClDHt84oknsh2+s+vBq7DmTKiT3hIkRYsWzbRvDw8PValSJdN+/x2qJKU7E21uetj60pPygUdGVyXr168va2trGY1GHT16NEdhNGUIblhYmOl+0QelhEg/P7+HCqMpP4e1a9dOd3tK8E6Z5RoAkHOEUQB4BKX8sf/PP//o5s2bZl0dLV++vM6cOaMRI0aoYcOGeV1iGt99950kqWXLlrKxscnTY5UqVUoODg6KjY3VtGnTUl25e1jly5eXJHXp0kXDhw/PtX4zUqFCBZ06dUonT540az3VvKgv5T7QjO6zNBgM8vDw0IEDBxQUFJTmHt2sHD161HT/alhYWKZL3Pz000/6888/Tfd2Zseff/6p48ePS5Kef/75dNukPMeHufcVAHAf94wCwCPI1dVVTz/9tIxGo/z9/c3ap3379pKktWvX5mVp6frqq6909OhRSdK7776b58ezsbExLUGS28835XVct25dnkz09G/t2rWTJH377bdmtc+L+p566inZ2dkpLCwsw6ujo0ePliRt2bIly1l6k5OT9eOPP5q+X758uaT79/dGR0dn+JUyUVdOJjJKSEgwzVJcs2ZNdenSJd12KaE4ZfZnAEDOEUYB4BGVsvzKtGnTtH79+jTb//rrL/3999+m79955x2VKFFCixYt0oIFC5SQkJBmn/Pnz2vFihW5VmN4eLjGjx+v9957T5L0n//8R88++2yu9Z+ZMWPGyM7OTh9++KECAwNTDd1N8ccff2jDhg3Z6tfT01ONGjXSzz//rLfffjvd+y6jo6P19ddfZ7meqjmGDh2qJ554Qlu2bNG0adPSrAN7/fr1VMEuL+pzcHBQkyZNZDQa9fPPP6fb5vnnn9ewYcMkSYMGDdLChQsVHx+fpt2vv/6qnj17asGCBZKku3fvas2aNZKyHlLt7e0tSVq5cmW21sM9ePCgOnfurB9//FGOjo764osvMhwunTKpU6tWrczuHwCQPobpAsAjqlu3bpo4caKmTZumV199VTVr1tTTTz+t2NhYnTt3Tn/99ZcWLVpkWt6lfPnyCgwM1CuvvKKJEyfq008/Va1atVS2bFndvHlTJ0+e1Llz59SkSRN5eXllq5bIyEgNGTJE0v17Fm/fvm2qwWg0ytHRUR9++KHeeOONXH8dMtKgQQN98cUXevvtt/X2229r+vTpevLJJ1W6dGlFRUXpjz/+0JUrV9SzZ89sDSu1trZWQECA+vTpo6CgIG3YsEFPP/20KlSooISEBJ0/f15//PGHkpKS5Ovrm+GkVeaqWLGivv32W7366quaM2eOli9frqZNm6pIkSK6dOmSfvvtN/Xu3du0vEte1efp6anQ0FD98MMPpqvO/zZt2jSVLFlSM2fO1IQJEzRr1iw1btxYZcqU0e3bt/X777/r4sWLkqQRI0ZIun8FNyYmRq6urmrbtm2mNbRr104uLi66du2aNm/enGbG402bNpn6T0xMVFRUlI4fP67w8HBJ0tNPP63FixerXr166fZ/7949hYaGqmjRoqYr0gCAnCOMAsAjbNSoUWrVqpU+//xzhYaGauPGjXJ0dFT58uX17rvvprm606JFCx08eFBffPGFQkJC9Msvvyg+Pl5lypRRhQoV1KdPn2zf7ydJd+7cUVBQkCSpSJEicnR0lIuLi3r06KGWLVuqZ8+eqdbVtJTu3burYcOG+vzzz7V7924dOnRISUlJKlOmjKpWrao33ngj28vqSFK5cuW0Y8cOBQYGas2aNfr999/1888/q2TJkipbtqxee+01de7cOcNJkLKrbdu2Cg0N1aJFi7Rz507t3LlTtra2Klu2rLy8vNJM6JMX9fXt21cff/yxVq5cqQ8//DDD+35HjRqll19+WcuWLdPu3bv122+/KSYmRsWKFVOVKlXUpUsX+fj4qH79+pL+N+S2T58+Wd5LbGtrq169emnJkiXy9/dPc+5OnDihEydOSLp/NdfJyUmVK1fWiy++qK5du6pVq1aZLiu0detWRUREqG/fvnk+4zMAPA6soqOj8/6GFgAA8Mh77//bu4OSCQEgAKNTwJsJrGADSwj2WPAmlvBiADt4EQtoEUNsgf+HPcjILu8lmOvHwMzrFfM8x7IsH70I+jZt28a6rrHv+7/bUwA+J0YBgFtc1xV1XUdVVbFt29Pj3Oo4jmiaJrqui2manh4H4Cc4YAQA3KIsy+j7Ps7z/PNo1jcbxzGKoohhGJ4eBeBn2IwCAACQzmYUAACAdGIUAACAdGIUAACAdGIUAACAdGIUAACAdGIUAACAdGIUAACAdGIUAACAdGIUAACAdGIUAACAdG8cP8DwAfdmIgAAAABJRU5ErkJggg==
"/>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p><strong>Step 6</strong></p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Our research is poised to reveal a correlation between each country's nominal GDP per capita and the differences in prices between the countries. This correlation, once established, could reshape our understanding of economic studies. To achieve this, we will import nominal GDP per capita data by country, clean it, and then integrate it with our latest coffee table data.
Nominal GDP per capita, a measure of the average production of a person in the country being measured, is a vital indicator of the standard of living. It provides a practical understanding of how much an average person contributes to the economy in that country, such as their earnings. Our research will further enhance the practical application of this measure in economic studies.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [ ]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-python"><pre><span></span><span class="n">gdp_data_usd_per_capita</span> <span class="o">=</span> <span class="n">Table</span><span class="p">()</span><span class="o">.</span><span class="n">read_table</span><span class="p">(</span><span class="s1">'/content/gdppercapita.csv'</span><span class="p">)</span><span class="o">.</span><span class="n">drop</span><span class="p">(</span><span class="s1">'Year'</span><span class="p">,</span> <span class="s1">'Unit'</span><span class="p">)</span>
<span class="n">gdp_data_usd_per_capita</span> <span class="o">=</span> <span class="n">gdp_data_usd_per_capita</span><span class="o">.</span><span class="n">with_column</span><span class="p">(</span><span class="s1">'Country/Area'</span><span class="p">,</span> <span class="n">gdp_data_usd_per_capita</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="n">capitalize</span><span class="p">,</span> <span class="s1">'Country/Area'</span><span class="p">))</span>
<span class="n">gdp_data_usd_per_capita</span> <span class="o">=</span> <span class="n">gdp_data_usd_per_capita</span><span class="o">.</span><span class="n">where</span><span class="p">(</span><span class="s1">'Country/Area'</span><span class="p">,</span> <span class="n">coffee_table_final</span><span class="o">.</span><span class="n">column</span><span class="p">(</span><span class="s1">'Country'</span><span class="p">))</span><span class="o">.</span><span class="n">sort</span><span class="p">(</span><span class="s1">'GDP, Per Capita GDP - US Dollars'</span><span class="p">,</span> <span class="n">descending</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span>
<span class="n">gdp_data_usd_per_capita</span> <span class="o">=</span> <span class="n">gdp_data_usd_per_capita</span><span class="o">.</span><span class="n">with_column</span><span class="p">(</span><span class="s1">'GDP, Per Capita GDP - Canadian Dollars'</span><span class="p">,</span> <span class="n">gdp_data_usd_per_capita</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="n">convert_to_cad</span><span class="p">,</span><span class="s1">'GDP, Per Capita GDP - US Dollars'</span><span class="p">))</span>

<span class="n">coffee_table_gdp</span> <span class="o">=</span>  <span class="n">coffee_table_final</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s1">'Country'</span><span class="p">,</span> <span class="n">gdp_data_usd_per_capita</span><span class="p">,</span> <span class="s1">'Country/Area'</span><span class="p">)</span>
<span class="n">coffee_table_gdp</span> <span class="o">=</span> <span class="n">coffee_table_gdp</span><span class="o">.</span><span class="n">with_column</span><span class="p">(</span><span class="s1">'GDP difference'</span><span class="p">,</span> <span class="n">coffee_table_gdp</span><span class="o">.</span><span class="n">column</span><span class="p">(</span><span class="s1">'GDP, Per Capita GDP - Canadian Dollars'</span><span class="p">)</span> <span class="o">-</span> <span class="n">coffee_table_gdp</span><span class="o">.</span><span class="n">column</span><span class="p">(</span><span class="s1">'GDP, Per Capita GDP - Canadian Dollars'</span><span class="p">)[</span><span class="mi">12</span><span class="p">])</span>

<span class="n">coffee_table_gdp</span> <span class="o">=</span> <span class="n">coffee_table_gdp</span><span class="o">.</span><span class="n">relabel</span><span class="p">(</span><span class="s2">"GDP, Per Capita GDP - US Dollars"</span><span class="p">,</span> <span class="s2">"Nominal GDP Per Capita (USD)"</span><span class="p">)</span><span class="o">.</span><span class="n">relabel</span><span class="p">(</span><span class="s2">"GDP, Per Capita GDP - Canadian Dollars"</span><span class="p">,</span> <span class="s2">"Nominal GDP Per Capita (CAD)"</span><span class="p">)</span>

<span class="n">coffee_table_gdp</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>


<span class="n">coffee_table_gdp</span><span class="o">.</span><span class="n">select</span><span class="p">(</span><span class="s1">'Country'</span><span class="p">,</span><span class="s1">'Nominal GDP Per Capita (CAD)'</span><span class="p">)</span><span class="o">.</span><span class="n">sort</span><span class="p">(</span><span class="s1">'Nominal GDP Per Capita (CAD)'</span><span class="p">,</span><span class="n">descending</span> <span class="o">=</span> <span class="kc">True</span><span class="p">)</span><span class="o">.</span><span class="n">barh</span><span class="p">(</span><span class="s1">'Country'</span><span class="p">)</span>
<span class="n">plots</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">'Nominal GDP Per Capita in Canadian Dollars Of Different Countries'</span><span class="p">)</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="application/vnd.jupyter.stderr" tabindex="0">
<pre>/usr/local/lib/python3.10/dist-packages/datascience/predicates.py:257: SyntaxWarning: Do not pass an array or list to a predicate.                 If you are trying to find rows where two columns are the                 same, use table.where('c', are.equal_to, table.column('d'))                instead of table.where('c', are.equal_to(table.column('d'))).
  warnings.warn("Do not pass an array or list to a predicate. \
</pre>
</div>
</div>
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output" data-mime-type="text/html" tabindex="0">
<table border="1" class="dataframe">
<thead>
<tr>
<th>Country</th> <th>Currency</th> <th>Currency Code</th> <th>Latte Price in local currency</th> <th>Latte Price (CAD)</th> <th>Sales Tax</th> <th>Price Difference (CAD)</th> <th>Purchasing Power Parity</th> <th>Purchasing Power Parity with tax</th> <th>Nominal GDP Per Capita (USD)</th> <th>Nominal GDP Per Capita (CAD)</th> <th>GDP difference</th>
</tr>
</thead>
<tbody>
<tr>
<td>ANDORRA       </td> <td>Euro             </td> <td>EUR          </td> <td>3.13                         </td> <td>4.61             </td> <td>0.045    </td> <td>-0.8                  </td> <td>0.851948               </td> <td>0.852126                        </td> <td>42293.3                     </td> <td>59398.8                     </td> <td>-18684.2      </td>
</tr>
<tr>
<td>ARGENTINA     </td> <td>Argentine Peso   </td> <td>ARS          </td> <td>4719.38                      </td> <td>6.56             </td> <td>0.21     </td> <td>1.15                  </td> <td>1.21299                </td> <td>1.21257                         </td> <td>13867.9                     </td> <td>19476.8                     </td> <td>-58606.2      </td>
</tr>
<tr>
<td>AUSTRALIA     </td> <td>Australian Dollar</td> <td>AUD          </td> <td>6.13                         </td> <td>5.58             </td> <td>0.1      </td> <td>0.17                  </td> <td>1.03117                </td> <td>1.03142                         </td> <td>67866.8                     </td> <td>95315.5                     </td> <td>17232.5       </td>
</tr>
<tr>
<td>AUSTRIA       </td> <td>Euro             </td> <td>EUR          </td> <td>3.32                         </td> <td>4.89             </td> <td>0.2      </td> <td>-0.52                 </td> <td>0.903896               </td> <td>0.903882                        </td> <td>52608.8                     </td> <td>73886.4                     </td> <td>-4196.62      </td>
</tr>
<tr>
<td>AZERBAIJAN    </td> <td>Azerbaijan Manat </td> <td>AZN          </td> <td>5.8                          </td> <td>4.79             </td> <td>0.18     </td> <td>-0.62                 </td> <td>0.885714               </td> <td>0.885397                        </td> <td>7599.97                     </td> <td>10673.8                     </td> <td>-67409.2      </td>
</tr>
<tr>
<td>BAHAMAS       </td> <td>Bahamian Dollar  </td> <td>BSD          </td> <td>3.75                         </td> <td>5.27             </td> <td>0.12     </td> <td>-0.14                 </td> <td>0.974026               </td> <td>0.974122                        </td> <td>31458.4                     </td> <td>44181.7                     </td> <td>-33901.3      </td>
</tr>
<tr>
<td>BAHRAIN       </td> <td>Bahraini Dinar   </td> <td>BHD          </td> <td>1.59                         </td> <td>5.95             </td> <td>0.1      </td> <td>0.54                  </td> <td>1.1013                 </td> <td>1.09982                         </td> <td>30146.5                     </td> <td>42339.3                     </td> <td>-35743.7      </td>
</tr>
<tr>
<td>BELGIUM       </td> <td>Euro             </td> <td>EUR          </td> <td>3.35                         </td> <td>4.94             </td> <td>0.21     </td> <td>-0.47                 </td> <td>0.914286               </td> <td>0.913124                        </td> <td>49986.8                     </td> <td>70204                       </td> <td>-7878.98      </td>
</tr>
<tr>
<td>BOLIVIA       </td> <td>Boliviano        </td> <td>BOB          </td> <td>22.08                        </td> <td>4.48             </td> <td>0.13     </td> <td>-0.93                 </td> <td>0.828571               </td> <td>0.828096                        </td> <td>3600.12                     </td> <td>5056.19                     </td> <td>-73026.8      </td>
</tr>
<tr>
<td>BRAZIL        </td> <td>Brazilian Real   </td> <td>BRL          </td> <td>11.89                        </td> <td>2.75             </td> <td>0.22     </td> <td>-2.66                 </td> <td>0.509091               </td> <td>0.508318                        </td> <td>8917.67                     </td> <td>12524.4                     </td> <td>-65558.6      </td>
</tr>
<tr>
<td>BULGARIA      </td> <td>Bulgarian Lev    </td> <td>BGN          </td> <td>4.98                         </td> <td>3.78             </td> <td>0.2      </td> <td>-1.63                 </td> <td>0.698701               </td> <td>0.698706                        </td> <td>13301.9                     </td> <td>18681.9                     </td> <td>-59401.1      </td>
</tr>
<tr>
<td>CAMBODIA      </td> <td>Riel             </td> <td>KHR          </td> <td>13083.8                      </td> <td>4.56             </td> <td>0.1      </td> <td>-0.85                 </td> <td>0.844156               </td> <td>0.842884                        </td> <td>1759.61                     </td> <td>2471.28                     </td> <td>-75611.7      </td>
</tr>
<tr>
<td>CANADA        </td> <td>Canadian Dollar  </td> <td>CAD          </td> <td>5.41                         </td> <td>5.41             </td> <td>0.109981 </td> <td>0                     </td> <td>1                      </td> <td>1                               </td> <td>55596.8                     </td> <td>78083                       </td> <td>0             </td>
</tr>
<tr>
<td>CHILE         </td> <td>Chilean Peso     </td> <td>CLP          </td> <td>4841.76                      </td> <td>6.95             </td> <td>0.19     </td> <td>1.54                  </td> <td>1.28571                </td> <td>1.28466                         </td> <td>15338.2                     </td> <td>21541.7                     </td> <td>-56541.3      </td>
</tr>
<tr>
<td>CHINA         </td> <td>Yuan Renminbi    </td> <td>CNY          </td> <td>30.72                        </td> <td>5.94             </td> <td>0.13     </td> <td>0.53                  </td> <td>1.0987                 </td> <td>1.09797                         </td> <td>12597.9                     </td> <td>17693.1                     </td> <td>-60389.9      </td>
</tr>
<tr>
<td>COLOMBIA      </td> <td>Colombian Peso   </td> <td>COP          </td> <td>11140.9                      </td> <td>3.51             </td> <td>0.19     </td> <td>-1.9                  </td> <td>0.649351               </td> <td>0.648799                        </td> <td>6630.28                     </td> <td>9311.9                      </td> <td>-68771.1      </td>
</tr>
<tr>
<td>COSTA RICA    </td> <td>Costa Rican Colon</td> <td>CRC          </td> <td>2144.1                       </td> <td>5.93             </td> <td>0.13     </td> <td>0.52                  </td> <td>1.0961                 </td> <td>1.09612                         </td> <td>13198.8                     </td> <td>18537.1                     </td> <td>-59545.9      </td>
</tr>
<tr>
<td>CYPRUS        </td> <td>Euro             </td> <td>EUR          </td> <td>2.83                         </td> <td>4.17             </td> <td>0.19     </td> <td>-1.24                 </td> <td>0.771429               </td> <td>0.770795                        </td> <td>32999.4                     </td> <td>46346                       </td> <td>-31737        </td>
</tr>
<tr>
<td>CZECH REPUBLIC</td> <td>Czech Koruna     </td> <td>CZK          </td> <td>94.48                        </td> <td>5.52             </td> <td>0.21     </td> <td>0.11                  </td> <td>1.02078                </td> <td>1.02033                         </td> <td>27685.1                     </td> <td>38882.4                     </td> <td>-39200.6      </td>
</tr>
</tbody>
</table>
</div>
</div>
<div class="jp-OutputArea-child jp-OutputArea-executeResult">
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[ ]:</div>
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>Text(0.5, 1.0, 'Nominal GDP Per Capita in Canadian Dollars Of Different Countries')</pre>
</div>
</div>
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,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Inpn5efnazoEUoL1o91YP9qPdURE7yImuERERERERKQTmOASERERERGRTmCCS0RERERERDqBCS4RERERERHpBCa4REREREREpBOY4BIREREREZFOYIJLREREREREOoEJLhEREREREekEJrhERERERESkE5jgEhERERERkU5ggktEREREREQ6gQkuERERERER6QQmuERERERERKQTmOASERERERGRTmCCS0RERERERDqBCS4RERERERHpBCa4REREREREpBOY4BIREREREZFOYIJLREREREREOoEJLhEREREREekEJrhERERERESkE5jgEhERERERkU5ggktEREREREQ6gQkuERERERER6QQmuERERERERKQTmOASERERERGRTmCCS0RERERERDqBCS4RERERERHpBCa4REREREREpBOY4BIREREREZFOYIJLREREREREOkGUnp5eoOkgiHTZ3/eeID9fqukwqBipNB9ZWdkwNTWBnp6+psOhYlg/2o31o/1YR5VTq4Y56lhZajoMIqoAA00HQKTrVm/dh1evszQdBhUjleYjO1sCExNjXvxpIdaPdmP9aD/WUeUs8nZngkv0H8UmykRERERERKQTmOASERERERGRTmCCS0RERERERDqBCS4RERERERHpBCa4REREREREpBOY4BIREREREZFOYIJLREREREREOoEJ7n+Il5cXxGIxmjRpgpycHLnztGnTBmKxWOl6FM2TkJCA2bNno127drC2toaNjQ0++ugjuLi44Oeff0ZmZqbM8mX9efz4MQCU+LxmzZpo1qwZXF1dcfr06VK339nZGWKxGA4ODqVun7W1danrK4ypY8eOCqcXFBTA3t4eYrEYLi4uZVonERERERFphoGmA6CyefXqFfbv3w+RSIS0tDSEhYVh+PDhKlv/tWvXMHjwYGRkZKBLly7o27cvzMzMkJiYiJiYGERERGDIkCGwtbXF1KlTkZGRIbN8YGAgEhISMGXKFFhYWMhMK/q7paUlJk6cCADIycnB33//jYiICBw7dgxbt27FiBEj5Mb36NEjnD17FiKRCH///Tf+/PNPdOjQQWXbr0h0dDQePnwIkUiEkydPIikpCXXr1lV7uUREREREVH5McP8jQkNDkZmZCS8vL2zatAl+fn4qTXC/+eYbZGRk4Ndff4Wbm1uJ6XFxcbC0tAQAfPnl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C19fX6Vjvb58+RIffvghqlWrhtu3b8PExAQAcPDgQezYsQNXr15FRkYGqlevjlatWsHNzQ2enp4lOqCKiYnB8ePHce7cOSQkJODFixcwMjJCo0aN0Lt3b3h5ecltJlzIyckJ586dQ3x8PBo1aiR3HrFYLNPJVHFHjx6Fm5sbHBwckJ+fj7i4OBw6dEjpmLP3799H+/bt0bRpU/z5558AgDZt2pTatX96enqJmAqfCP/zzz+4cuWK0hsLp0+fxtChQ/Hxxx8jNDRUaVkT5v2MV6+zlM5DVU8qzUd2tgQmJsbsgEULsX60G+tH+7GOKmeRtztaf9hY02EQUQUwwSVSMya42okXf9qN9aPdWD/aj3VUOUxwif672IsyERERERER6QQmuERERERERKQTmOASERERERGRTmCCS0RERERERDqBCS4RERERERHpBCa4REREREREpBM4TBCRmv197wny86WaDoOKkUrzkZWVDVNTEw6hoYVYP9qN9aP9WEeVU6uGOepYWWo6DCKqACa4RPROkkgkSEhIQIMGDWBsbKzpcKgY1o92Y/1oP9YREb2r2ESZiIiIiIiIdAITXCIiIiIiItIJTHCJiIiIiIhIJzDBJSIiIiIiIp3ABJeIiIiIiIh0goGmAyDSdRwmSDu9HUIjB9kPn3IIDS3E+tFurB/N4hA2RESKMcElUrPVW/fh1essTYdBxUil+cjOlsDExJgX6FqI9aPdWD+atcjbnQkuEZECbKJMREREREREOoEJLhEREREREekEJrhERERERESkE5jgEhERERERkU5ggktEREREREQ6gQkuERERERER6QQmuERERERERKQTmOCSjKtXr2LatGlo164d6tWrhzp16sDOzg6TJk3CqVOn5C6TmZmJBg0aQCwWY86cOQrX/fjxY4jFYojFYgwfPlzuPBcvXoRYLMbUqVMVrufJkyewtLSEWCzGunXrFM4XHR0tlFf4Y2Njg1atWmHEiBFYu3YtkpKSFC5f6Ny5c8Ly+/fvL3V+IiIiIiLSDCa4BACQSqVYsGABevXqhaCgIDRu3Bhjx47FlClTYGdnh4iICAwbNgyrVq0qsWxoaChevXoFkUiEPXv2QCKRlFpeZGQkoqKiKhSrv78/pFIpRCIR/P39S53fzs4Oc+fOxdy5czF+/Hh0794d9+/fx3fffQd7e3v89ttvSpf3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tpJIJEhISECDBg3YQ6+WYh0R0buK7+ASERERERGRTmCCS0RERERERDqBCS4RERERERHpBCa4REREREREpBOY4BIREREREZFOYIJLREREREREOoHj4BKp2ewJw5GfL9V0GFSMVJqPrKxsmJqacJggLaQt9VOrhrnGyiYiIqLyY4JLpGYtmjbUdAgkx/+NEWnDMSK1EOuHiIiIKoJNlImIiIiIiEgnMMElIiIiIiIincAEl4iIiIiIiHQCE1wiIiIiIiLSCUxwiYiIiIiISCewF2UiNfv73hMOE6SF3g5Dk4Psh085TJAWUmf91KphjjpWlipdJxEREWkHJrhEarZ66z68ep2l6TCoGKk0H9nZEpiYGDPB1ULqrJ9F3u5McImIiHQUmygTERERERGRTmCCS0RERERERDqBCS4RERERERHpBCa4REREREREpBOY4BIREREREZFOYIJLREREREREOoEJLhEREREREekEJrg65PHjxxCLxSV+6tWrh65du2LFihV4/fq1wuXPnTsnLLN//36F8wUEBEAsFmPt2rUK5/Hx8YFYLEZISIjCeXbt2iWUd/ny5VLXJRaLsXDhQoXzLV68WJjPx8dH4Xxl3U4ASEhIwOzZs9GuXTtYW1vDxsYGH330EVxcXPDzzz8jMzNT6fJERERERFR1DDQdAKlekyZN4OLiAgAoKChASkoKjh8/jhUrVuDkyZM4evQo9PX1Syzn5+cHABCJRPD398fQoUPVGqefnx9EIhEKCgrg7++Pdu3aKZ3fwMAAwcHBWLJkCQwMZHfdvLw8BAUFwcDAAHl5eaWWC5S+ndeuXcPgwYORkZGBLl26oG/fvjAzM0NiYiJiYmIQERGBIUOGwNbWtuwbTUREREREasMEVwfZ2tpi/vz5Mp/l5OSgX79+uHjxIs6ePYuePXvKTH/58iUOHjyIVq1awcrKCpGRkUhMTET9+vXVEuP9+/cRExODgQMH4u7du9i7dy+WL18OExMThcv07dsXR48exdGjRzF48GCZaREREUhOTsbAgQNx5MgRhesoz3Z+8803yMjIwK+//go3N7cS0+Pi4mBpaVmOrSYiIiIiInViE+V3hJGRERwdHQEAqampJaaHhIQgKysLbm5ucHNzg1QqRWBgoNri8ff3BwC4ubnB1dUVL1++xIEDB5Qu4+zsDAsLC2HZ4usTi8UlEt/i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fpXWER0dXeKrf9zd3TFgwADF96W9JqhZs2ZvtAAVERERERGpT7WtoiyTyZCWloZ79+4BAD744AMYGKj99KTl9PT0sGzZMgwbNgxbt25FQkICEhISIJPJYGNjAzc3N/j6+qJnz55VWsfly5dx+fJllfscHByUAm5prwnq378/Ay4RERERkZYQZGVlyavzhFevXsVXX30FKysr7N69G/r6XF2WdNuYgB/wIjtX02XQa2QyKfLyJDA1NSlxFeVAfx+0fMexegsjAK8eV0hLS4O9vT1XgNVCHB/txzEiopqq2heZatmyJUQiEc6dO4f/+7//q+7TExERERERkY7SyCrKjRs3xvvvv4/w8HBNnJ6IiIiIiIh0kMZeE2RlZYU7d+5o6vRERERERESkYzQScAsKCnDx4kWYmppq4vRERERERESkg6o14Obk5ODPP/+En58f7t27h27dulXn6YmIiIiIiEiHqf09PZaWlmW2kcvlqFOnTpW/65SIiIiIiIhqDrUHXLm85LcOGRoaokGDBujZsye+/vprNG7cWN2nJ9I6M8YMhlQq03QZ9BqZTIrc3DzUqmVa4muCrOpaVHNVRERERPQm1B5wnz59qu4uid5qzV0cNF0CqfC/d0Q25DsiiYiIiHSExlZRJiIiIiIiIlInBlwiIiIiIiLSCWqfolwkMzMTv/zyC06fPo0HDx4AABo0aIDu3bvj888/L9diVERERERERETlVSUB9/jx4xg9ejSePXumtOjUv//+ixMnTuD//u//sGXLFvTq1asqTk9EREREREQ1kNoD7q1bt+Dn54fc3Fy899578PX1hZOTEwDg9u3b2LlzJ65cuQI/Pz+cOnUKTZo0UXcJREREREREVAOpPeCuXbsWubm5CAgIwOzZs4vtnzBhAlauXImgoCD88MMPWL9+vbpLINIq15Lu8DVBWsSqrgVsrfmIBBEREZEuUnvAPXnyJJo2baoy3BaZNWsW9uzZgxMnTqj79ERaZ/WWKLzIztV0GfT/Bfr7MOASERER6Si1r6L86NEjtG7dusx2rVu3xqNHj9R9eiIiIiIiIqqh1B5wa9WqhcePH5fZ7vHjx6hVq5a6T09EREREREQ1lNoDrqurKxISEvD333+X2Obq1as4c+YMXF1d1X16IiIiIiIiqqHUHnC/+OILvHz5Eh4eHtiyZQuys7MV+7Kzs/Hz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f/vtN+zZswd79+7FmTNnkJmZCQMDA9jY2KBbt24YNGgQ+vXrB319fchkMoSFhUEgEMDb27vU6/X19cXu3bshEonKFXABICAgAF5eXli6dCl+/fVXlW2ioqKQm5sLb29vmJubl9iXi4sLOnbsiHPnzpVr2jMREREREVUtQVZWlrzsZkRUWWMCfsCL7NyyG1KVCPT3Qct3HIttl0gkSEtLg729PVcY1UIcH+3G8dF+HCMiqqm4ijIRERERERHpBAZcIiIiIiIi0gkMuERERERERKQTGHCJiIiIiIhIJzDgEhERERERkU5gwCUiIiIiIiKdwPfgElWxGWMGQyqVabqMGsuqroWmSyAiIiKiasKAS1TFmrs4aLoEIiIiIqIagVOUiYiIiIiISCcw4BIREREREZFOYMAlIiIiIiIincCAS0RERERERDqBAZeIiIiIiIh0AgMuERERERER6QS+Joioil1LusP34GqIVV0L2FpbaroMIiIiIqomDLhEVWz1lii8yM7VdBk1UqC/DwMuERERUQ3CKcpERERERESkExhwiYiIiIiISCcw4BIREREREZFOYMAlIiIiIiIincCAS0RERERERDqBAZeIiIiIiIh0AgOuFrh06RImT56Mtm3bws7ODra2tmjTpg3GjRuH3377TeUxEokEmzZtQr9+/eDk5ARra2u0aNECI0eOxMmTJ0s8V05ODlavXo3u3bujYcOGiuP69euHRYsWISUlBQAwceJECIXCcn+FhoYqnefTTz+FUChEp06dKvWZqDp/o0aN0KNHD6xbtw75+fnFjklNTYVQKMSQIUNU9llYWAixWIxhw4ahWbNmqF+/PhwcHPDRRx9hyZIluHPnTon1hIWFKeq4ePFipa6JiIiIiIiqFt+Dq0EymQzz589HcHAwDAwM0L17d/Tr1w+Ghoa4ffs2YmJiEBERgblz52LWrFmK45KTkzF8+HAkJSXB0dERgwYNQp06dRTHREdHY+TIkVi1ahUMDP43xC9evEDfvn3x999/w9nZGcOHD4elpSUyMjLwxx9/YO3atXBycoKTkxPc3d3h4OCgVG98fDzOnDmD/v37w9XVVWnff7+/ffs24uPjIRAIcO3aNfz+++9o3759pT4jPz8/2NnZQS6X4+HDhzh48CAWLFiAU6dOITIystz93LlzBz4+Prh69Sqsra3Rs2dPNGrU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H49Tp06hR48emi5HwdXVFcOGDcOuXbsQHR1dYrui1ZODgoIQFBSkso1IJCpXwBXo6UNPr+w7vfTm9PT0Kzz1y8jIiNPFtBjHR7txfLQfx4iIahoGXKoSPj4+WLt2LUJCQjBx4kRYWVmV2DY/P7/KV1L+r3nz5iE6Ohrfffed0vO1RRISEpCUlAQnJ6cSpzH/+uuvOHr0KB4/foz69etXdclERERERFQODLhUJZydnTF16lSsWbMGQ4cORUhICBwdHZXaSCQSbNmyBRkZGViwYEG11ebg4IDRo0cjODgYO3fuLLa/aHGpGTNmYMSIESr7WLx4MdasWYPw8HD4+/tXab1ERERERFQ+DLhUZebPnw+JRILg4GB06NAB3bt3R/PmzWFoaIjU1FScOHECmZmZmD9/frXXNnPmTIjFYqSkpChtf/78Ofbt2wczMzN4eHiUeLyPjw/WrFkDkUjEgEtEREREpCX0NF0A6S49PT0sW7YMv/32Gzw9PZGSkoKtW7ciODgYv//+O9zc3BAdHY2ZM2dWe22WlpaYNm1ase1RUVHIzc3FZ599BnNz8xKPd3FxQceOHXHjxg0kJiZWYaVERERERFRegqysLLmmiyDSZWMCfsCL7FxNl1EjBPr7oOU7juVqK5FIkJaWBnt7ey7AooU4PtqN46P9OEZEVFPxDi4RERERERHpBAZcIiIiIiIi0gkMuERERERERKQTGHCJiIiIiIhIJzDgEhERERERkU5gwCUiIiIiIiKdwIBLREREREREOsFA0wUQ6boZYwZDKpVpuowawaquhaZLICIiIiINYsAlqmLNXRw0XQIRERERUY3AKcpERERERESkExhwiYiIiIiISCcw4BIREREREZFOYMAlIiIiIiIincCAS0RERERERDqBqygTVbFrSXdq9GuCrOpawNbaUtNlEBEREVENwIBLVMVWb4nCi+xcTZehMYH+Pgy4RERERFQtOEWZiIiIiIiIdAIDLhEREREREekEBlwiIiIiIiLSCQy4REREREREpBMYcImIiIiIiEgnMOASERERERGRTmDAJSIiIiIiIp3AgEuVlpqaCqFQWOzLzs4OnTt3xvLly5Gdna10jLu7u1LbunXrwsHBAX369MH27dshk8lKPeeKFSsgFAphZWWF9PR0lW1CQ0NV1qXqy93dXXHc6dOnIRQKMX36dKX+Jk6c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+DG8vb3x/vvvl9o+Pj5ebZ8dERERERFVHwbct8j8+fMhkUgQHByMDh06oHv37mjevDkMDQ2RmpqKEydOIDMzE/Pnz1cskFTanc6mTZviww8/RGJiomKV5JK8//77ZQbD1504cUKxIrBMJsOjR49w7NgxRVAePXq0oq2hoSF27twJb29vhISE4OjRo+jduzfq16+P+/fv4+jRo8jMzESfPn0Ud3Ffl5GRgaCgIACAVCpFZmYmLl++jD/++AMA8Pnnn2PVqlVl1q3uz46IiIiIiKoHA+5bRE9PD8uWLcOwYcOwdetWJCQkICEhATKZDDY2NnBzc4Ovry/ef/99vPvuuzAzM8PAgQNL7dPX1xeJiYkQiURqD2mvvybIzMwMzs7OGDVqFL766ivUqlVLqb21tTWOHj2KnTt3Ys+ePTh48CBevHgBoVCIDh06wMfHp9TryczMxIoVKwAAxsbGsLCwQJMmTeDv7w9PT0+0bNmyzJqfPXuGAwcOaPyzIyIiIiKiihNkZWXJNV0EkS4bE/ADXmTnlqttoL8PWr7jWLUFEYBX0+XT0tJgb2/PBVi0EMdHu3F8tB/HiIhqKj1NF0BERERERESkDgy4REREREREpBMYcImIiIiIiEgnMOASERERERGRTmDAJSIiIiIiIp3AgEtEREREREQ6gQGXiIiIiIiIdIKBpgsg0nUzxgyGVCorV1uruhZVXA0RERERke5iwCWqYs1dHDRdAhERERFRjcApykRERERERKQTGHCJiIiIiIhIJzDgEhERERERkU5gwCUiIiIiIiKdwIBLREREREREOoEBl4iIiIiIiHQCAy4RERERERHpBAZcIiIiIiIi0gkMuERERERERKQTGHCJiIiIiIhIJzDgEhERERERkU5gwCUiIiIiIiKdwIBLREREREREOoEBl4iIiIiIiHQCAy4RERERERHpBAZcIiIiIiIi0gkMuERERERERKQTGHCJiIiIiIhIJzDgEhERERERkU5gwCUiIiIiIiKdwIBLREREREREOoEBl4iIiIiIiHQCAy4RERERERHpBAZcIiIiIiIi0gkMuERERERERKQTGHCJiIiIiIhIJzDgEhERERERkU5gwCUiIiIiIiKdwIBLREREREREOoEBl4iIiIiIiHQCAy4R1Vj6+vqaLoFKwfHRbhwf7ccxIqKaSJCVlSXXdBFERERE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
"/>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p><strong>Step 7</strong></p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [ ]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-python"><pre><span></span><span class="n">coeff</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">polyfit</span><span class="p">(</span><span class="n">coffee_table_gdp</span><span class="o">.</span><span class="n">column</span><span class="p">(</span><span class="s1">'Price Difference (CAD)'</span><span class="p">),</span><span class="n">coffee_table_gdp</span><span class="o">.</span><span class="n">column</span><span class="p">(</span><span class="s1">'Nominal GDP Per Capita (CAD)'</span><span class="p">),</span> <span class="mi">1</span><span class="p">)</span>

<span class="n">fitted_y</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">polyval</span><span class="p">(</span><span class="n">coeff</span><span class="p">,</span> <span class="n">coffee_table_gdp</span><span class="o">.</span><span class="n">column</span><span class="p">(</span><span class="s1">'Price Difference (CAD)'</span><span class="p">))</span>
<span class="n">plots</span><span class="o">.</span><span class="n">scatter</span><span class="p">(</span><span class="n">coffee_table_gdp</span><span class="o">.</span><span class="n">column</span><span class="p">(</span><span class="s1">'Price Difference (CAD)'</span><span class="p">),</span><span class="n">coffee_table_gdp</span><span class="o">.</span><span class="n">column</span><span class="p">(</span><span class="s1">'Nominal GDP Per Capita (CAD)'</span><span class="p">))</span>
<span class="n">plots</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">coffee_table_gdp</span><span class="o">.</span><span class="n">column</span><span class="p">(</span><span class="s1">'Price Difference (CAD)'</span><span class="p">),</span> <span class="n">fitted_y</span><span class="p">,</span> <span class="n">color</span><span class="o">=</span><span class="s1">'orange'</span><span class="p">,</span> <span class="n">label</span><span class="o">=</span><span class="s1">'Fitted Curve'</span><span class="p">)</span>

<span class="n">plots</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">'Price Difference'</span><span class="p">)</span>
<span class="n">plots</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">'GDP Per Capita in CAD'</span><span class="p">)</span>
<span class="n">plots</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">'Price Difference vs GDP Per Capita'</span><span class="p">)</span>

<span class="nb">print</span><span class="p">(</span><span class="s1">'correlation = '</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">correlation</span><span class="p">(</span><span class="n">coffee_table_gdp</span><span class="p">,</span><span class="s1">'Price Difference (CAD)'</span><span class="p">,</span><span class="s1">'Nominal GDP Per Capita (CAD)'</span><span class="p">)))</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>correlation = 0.188986908305
</pre>
</div>
</div>
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,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mHwSERERkdEw+SQiIiIio2HySURERERGw9HuRERERGQ0bPkkIiIiIqNh8klERERERsPkk4iIiIiMhsknUTFlZWUhNjYWWVlZpg6FSgDr1/yxjs0b67f0YfJJZAB5eXmmDoFKEOvX/LGOzRvrt3Rh8klERERERsPkk4iIiIiMhsknERERERkNk08iIiIiMhomn0RERERkNEw+iYiIiMhomHwSERERkdEw+SQiIiIio2HySUREZGByudzUIRCVWpamDoCIiMgcpEllWHA5FUcSsiCVyWElFCDIwwbzmjnA3optPUQKTD6JiIiKKU0qQ9cDL3BPnAtZge3r7koQ+TQb4b2rMQEl+h++E4iIiIppweVUtcQTAGQA7olzsfByqinCIiqVmHwSEREV05GELLXEU0EG4HBCljHDISrVmHwSEREVg1wuh1RW+AAjqUzOQUhE/8Pkk4iIqBgEAgGshIJCy1gJBRAICi9DVF4w+SQiIiqmIA8brX9QhQB6eNgYMxyiUo3JJxERUTHNa+aAOk6Wan9UhQDqOllibjMHU4RFVCox+SQiIiomeyshwntXw4T6InjaWcC1ohCedhaYUF+EY5xmiUgF5/kkIiIyAHsrIRa3dsLi1vmDkNjHk0gzfhUjIiIyMCaeRNox+SQiIiIio2HySURERERGw+STiIiIiIyGyScRERERGQ2TTyIiIiIyGiafRERERGQ0TD6JiIiIyGiYfBIRERGR0TD5JCIiIiKjYfJJREREREbD5JOIiIiIjIbJJxEREREZDZNPIiIiIjIaJp9EREREZDRMPomIiIjIaJh8EhEREZHRMPkkIiIiIqNh8klERERERsPkk4iIiIiMhsknERERERkNk08iIiIiMhomn0RERERkNEw+iYiIiMhomHwSERERkdEw+SQiIiIio2HySURERERGw+STiIiIiIyGyScRERERGQ2TTyIiIiIyGiafRERERGQ0TD6JiIiIyGiYfBIRERGR0TD5JCIiIiKjYfJJREREREbD5JOIiIiIjIbJJxEREREZDZNPIiIiIjIaJp9EREREZDRMPomIiIjIaJh8EhEREZHRMPkkIiIiIqOxLO4JXr58iefPnyM9PR0ODg6oXr06KleubIjYiIiIiMjM6JV8JiUl4eeff8bhw4cRHx+vtr9mzZro1asXPvzwQ1SvXr3YQRIRERGReSjy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iIiobNJ7fp++ffvi2rVrSEpKAgBUrVoVK1aswKRJk3Dp0iVcvnxZObdnu3btMGvWLMNETERERERllt7Jp4+PDzZt2qSyrV+/fnjnnXewe/duxMfHw9bWFm3btkXPnj3Zn4mIiIiIDLe2u4KnpyemT59u6NMSERERkRnQu8/n4sWLsXXrVp3Kbtu2DYsXL9b3UkRERERkJvROPhctWoQtW7boVHbr1q1MPomIiIhI/+SzKBQDj4iIiIiofDNK8vny5UtUrFjRGJciIiIiolJM5wFHqampSElJUdmWk5ODhIQErcdkZmbi5MmTuHfvHho1aqR/lERERERkFnROPn/99Vd8//33KtuuXr0Kf39/nY4fOnRo0SIjIiIiIrOjc/Ipl8tV+m4KBIK39uWsWLEiatasiWHDhmHKlCn6R0lEREREZkHn5POzzz7DZ599pvy9UqVKaN26NQ4fPlwigRERERGR+dF7kvnZs2fD3d3dkLEQERERkZnTO/n89NNPDRkHEREREZUDRplqiYiIiIgI0LHlc+rUqQAAFxcXzJs3T2WbrgQCAVasWFHE8IiIiIjInOiUfP7xxx8AgDp16iiTzz/++EOnEe8KTD6JiIiISKfkc/bs2QCAKlWqqG0jIiIiItKVTsmnpsFFHHBEREREREXFAUdEREREZDRMPomIiIjIaPSe51MhLS0NmzdvxrFjx3Dv3j2kp6fDzs4OderUQffu3TFixAg4ODgYIlYiIiIiKuOKlXyeP38e48ePR1JSksqo97S0NDx9+hSRkZH45ZdfsG7dOgQEBBQ7WCIiIiIq2/ROPh88eIBBgwZBIpHAyckJo0ePRr169VC9enU8f/4c0dHR2Lx5M54+fYohQ4bg77//hq+vryFjJyIiIqIyRu/kc9GiRZBIJOjevTvWr18PkUikVmbWrFl4//33ceTIESxevBjr1q0rVrBEREREVLbpPeDo1KlTsLGxwerVqzUmngAgEomwatUq2NjY4NSpU3oHSURERETmQe/kMz09HfXq1YOTk1Oh5ZycnFCvXj2kp6freykiIiIiMhN6J5/u7u5IS0vTqWxaWho8PDz0vRQRERERmQm9k8/+/fsjNjYW//zzT6Hl/vnnH8TExKB///76XoqIiIiIzITeyed///tftGjRAu+99x52796tMtUSAMjlcoSFhWHkyJFo1aoV/vvf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n7hx44Zye0pKinL1qmHDhpkwQiLzxhWOiAzk3r17aN++PbKzszFw4EDUrl1brYynpydX2Cjj7t27hx9//BEAkJWVhbCwMFSvXl05PyQArFq1ylThkY60La+ZkJCABQsWcHnNMi40NBRRUVEAgDt37uD69eto3bo1atasCQBo06YNRo8ebcoQyzUmn0QGcvr0afTp06fQMlyGsezTpZ7FYrFxgqFiuXz5Mr777jtcvHgRUqkUfn5+mDp1KgYMGGDq0KiYJk+eXOgqVcOHD+eXRBNi8klERERERsM+n0RERERkNEw+iYiIiMhomHwSERERkdEw+SQiIiIio2HySURERERGw+STiIiIiIyGyScRERERGQ2TTyIiIiIyGiafRERERGQ0TD6JqFzYunUrnJyc0KtXL1OHUuJOnz4NJycnNGrUSON+sViMmTNnolGjRqhatara8yKTybBy5UoEBATAxcUFTk5OcHJyMlL0RGTuLE0dABGRQq9evXD27FmVbUKhEA4ODqhTpw569eqF999/HyKRyEQRlqz4+Hj4+/urbBMIBLCzs4O9vT1q1qyJJk2aoE+fPmjdurXe1xkxYgTOnj0LW1tbNGjQALa2tvDz81PuX7x4MRYvXgyBQID69evDwcFB72sREb2JyScRlTru7u5wd3cHAEilUsTFxeHixYu4ePEiQkNDceDAAbi6uhbpnA4ODvD19VWet7R75513UKFCBQBAZmYmXr16hbNnz+Ls2bNYuXIlmjRpgpUrV6JBgwZqx1asWBG+vr4an6M7d+4oE8/z58/Dy8tLZb9cLse6desAABs2bEBwcHAJPDoiKs8EYrFYbuogiIiA/2/5nD17Nj777DOVfXv37sWUKVMgkUjQo0cPbNu2zURRlpyCLZ/Xr19XSwzFYjH27duHpUuX4tGjR7CxscG+ffvQsmVLna8RFhaGcePGoWnTpoiIiFDb/+LFC/j6+gIAnjx5gooVKxbjERERqWOfTyIqE/r164eZM2cCAI4ePQqxWGzagEzAyckJo0ePRmRkJJo1a4asrCyMGjUKGRkZOp8jMzMTAGBra1vofgBMPImoRDD5JKIyo2PHjgDyB8TExsYCUB9c8+eff6Jnz57w9vaGk5MTTp8+DeDtA47kcjkOHDiA4cOHo169eqhevTp8fX3x7rvv4vvvv0dSUpLaMXl5ediyZQv6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
"/>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Our research, employing simple linear regression, has produced a correlation coefficient of 0.18716967518. This coefficient suggests a weak correlation between the price difference of Starbucks' latte and a country's GDP. However, this could be due to a variety of external factors influencing the price of a Starbucks latte. For example, countries experiencing political instability often have a higher cost of living, leading to increased prices of goods. It's important to note that countries with low GDP often experience political instability simultaneously (Aisen, A., &amp; Veiga, F. J., 2013). Inflation can also impact the price of a Starbucks latte, with countries with high inflation rates also experiencing higher living costs. In conclusion, our research underscores the need for a comprehensive approach that considers multiple factors in understanding price differences, rather than attributing them to a single cause.</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Another external factor that we believe is a correlation between each country's HDI index and the differences in prices between the countries.
According to Klugman et al. (2011), the HDI index measures a country based on three criteria: health, knowledge, and standard of living.</p>
<p>According to the United Nations Development Programme (2020):</p>
<p><strong>Very High:</strong> HDI &gt; 0.800<br/>
<strong>High:</strong> 0.700 &lt;= HDI &lt;= 0.799<br/>
<strong>Medium:</strong> 0.550 &lt;= HDI &lt; 0.700<br/>
<strong>Low:</strong> HDI &lt; 0.550</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p><strong>Importing HDI Data</strong></p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [ ]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-python"><pre><span></span><span class="n">hdi_raw</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">"https://en.wikipedia.org/wiki/List_of_countries_by_Human_Development_Index?useskin=vector"</span><span class="p">)</span>
<span class="n">scraped_hdi</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">hdi_raw</span><span class="o">.</span><span class="n">text</span><span class="p">,</span><span class="s2">"html.parser"</span><span class="p">)</span>

<span class="n">heading_hdi</span> <span class="o">=</span> <span class="n">scraped_hdi</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">"h2"</span><span class="p">,</span> <span class="p">{</span><span class="s2">"id"</span><span class="p">:</span> <span class="s2">"List"</span><span class="p">})</span>
<span class="n">hdi_table</span> <span class="o">=</span> <span class="n">heading_hdi</span><span class="o">.</span><span class="n">find_next</span><span class="p">(</span><span class="s2">"table"</span><span class="p">,</span> <span class="p">{</span><span class="s2">"class"</span><span class="p">:</span> <span class="s2">"wikitable"</span><span class="p">})</span>
<span class="n">hdi_table</span> <span class="o">=</span> <span class="n">scrape_table</span><span class="p">(</span><span class="n">hdi_table</span><span class="p">)</span><span class="o">.</span><span class="n">select</span><span class="p">(</span><span class="mi">2</span><span class="p">,</span> <span class="mi">3</span><span class="p">)</span><span class="o">.</span><span class="n">relabel</span><span class="p">(</span><span class="s2">"Country or territory"</span><span class="p">,</span> <span class="s2">"Country"</span><span class="p">)</span>
<span class="n">hdi_table</span> <span class="o">=</span> <span class="n">hdi_table</span><span class="o">.</span><span class="n">with_column</span><span class="p">(</span><span class="s2">"Country"</span><span class="p">,</span> <span class="n">hdi_table</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="n">capitalize</span><span class="p">,</span> <span class="s1">'Country'</span><span class="p">))</span>
<span class="n">hdi_table</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child jp-OutputArea-executeResult">
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[ ]:</div>
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html" tabindex="0">
<table border="1" class="dataframe">
<thead>
<tr>
<th>Country</th> <th>HDI value</th>
</tr>
</thead>
<tbody>
<tr>
<td>SWITZERLAND</td> <td>0.967    </td>
</tr>
<tr>
<td>NORWAY     </td> <td>0.966    </td>
</tr>
<tr>
<td>ICELAND    </td> <td>0.959    </td>
</tr>
<tr>
<td>HONG KONG  </td> <td>0.956    </td>
</tr>
<tr>
<td>DENMARK    </td> <td>0.952    </td>
</tr>
<tr>
<td>SWEDEN     </td> <td>0.952    </td>
</tr>
<tr>
<td>IRELAND    </td> <td>0.95     </td>
</tr>
<tr>
<td>GERMANY    </td> <td>0.95     </td>
</tr>
<tr>
<td>SINGAPORE  </td> <td>0.949    </td>
</tr>
<tr>
<td>NETHERLANDS</td> <td>0.946    </td>
</tr>
</tbody>
</table>
<p>... (183 rows omitted)</p>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>We will join the table of the price differences and the HDI values and then display the values on a bar chart to visually see the comparison.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [ ]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-python"><pre><span></span><span class="n">price_dif_hdi</span> <span class="o">=</span> <span class="n">coffee_table_final</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">"Country"</span><span class="p">,</span> <span class="n">hdi_table</span><span class="p">,</span> <span class="s2">"Country"</span><span class="p">)</span><span class="o">.</span><span class="n">sort</span><span class="p">(</span><span class="s2">"Price Difference (CAD)"</span><span class="p">,</span> <span class="n">descending</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>

<span class="n">price_dif_hdi</span> <span class="o">=</span> <span class="n">price_dif_hdi</span><span class="o">.</span><span class="n">select</span><span class="p">(</span><span class="s2">"Country"</span><span class="p">,</span> <span class="s2">"Price Difference (CAD)"</span><span class="p">,</span> <span class="s2">"HDI value"</span><span class="p">)</span>

<span class="n">price_dif_hdi</span><span class="o">.</span><span class="n">barh</span><span class="p">(</span><span class="s2">"Country"</span><span class="p">,</span> <span class="s2">"Price Difference (CAD)"</span><span class="p">)</span>
<span class="n">plots</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">"Latte Prices Around the World"</span><span class="p">)</span>

<span class="n">price_dif_hdi</span><span class="o">.</span><span class="n">sort</span><span class="p">(</span><span class="s2">"HDI value"</span><span class="p">,</span> <span class="n">descending</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span><span class="o">.</span><span class="n">barh</span><span class="p">(</span><span class="s2">"Country"</span><span class="p">,</span> <span class="s2">"HDI value"</span><span class="p">)</span>
<span class="n">plots</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">"HDI Index Values Around the World"</span><span class="p">)</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child jp-OutputArea-executeResult">
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[ ]:</div>
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>Text(0.5, 1.0, 'HDI Index Values Around the World')</pre>
</div>
</div>
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAuUAAANlCAYAAADb/YeSAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguMCwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy81sbWrAAAACXBIWXMAAA9hAAAPYQGoP6dpAADuDklEQVR4nOzdeXhMZ/8/8PdMIguRjCAhJJIUrZKKrRJqqVBLQq1JJKFUKSWWh8dWaikNWrRF9KmlarIJIbULYo+ttRTVWkJEQ5ANSSYhM78/8pv5ZsxMkplMHEner+vKRebc55zPmXuG95y5z31EmZmZChARERERkWDEQhdARERERFTVMZQTEREREQmMoZyIiIiISGAM5UREREREAmMoJyIiIiISGEM5EREREZHAGMqJiIiIiATGUE5EREREJDCGciIiIiIigTGUExFVIklJSZBIJJBIJAgPDxe6HKoC3NzcIJFIMG7cuHLf17hx4yCRSODm5lbu+yLdTpw4ofp35sSJEwZvJyQkRLUdYignohIU/cc3JCRE6HIqJGVoefWndu3acHFxQffu3TF//nzcvXtX6FIrpb/++kvtef/tt9+ELokquV27dqlebz/88EOxbS9duqT2+izp34EFCxao2h49etR4RZPgGMqJ6I3n7e0NiUQCb2/vEtu+zrN2ZVVQUICMjAz8/vvv+P7779G+fXv88ssvQpdV6URGRqr9HhUVJVAlpE14eLgqZCYlJQldjlF06NABIpEIAJCQkFBs21OnThX7+6uU26tWrRratWtXhirpTWMqdAFERFVF/fr1ERMTo/r95cuX+Pfff7F9+3Zs3boVeXl5+M9//oMGDRrgo48+MmgfjRo1QmZmppEqrvgKCgqwdetWAICVlRWeP3+OQ4cO4cmTJ6hTp47A1VFlVbt2bbz99tv4+++/cebMGcjlcojF2s+DKkO2iYkJCgoKkJCQgMDAQK1tc3NzcfHiRQCAu7s7atSoUT4HQILgmXIiotfE1NQU7777rurnvffeQ+/evbFu3TosWrQIAKBQKPDNN98IXGnlER8fj4cPHwIoHL8qEonw4sULVVAnKi8dO3YEAGRlZeHq1as62505cwYAMGDAAADFn1n//fffkZ+fD6DwbDxVLgzlRERvgC+++AINGzYEUDjG9PHjxwJXVDkoh644ODggMDBQFWReHdJCZGxF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xIkTxd4k6a233sKxY8cwZswYODs7w8zMDLa2tujcuTM2btyIn3/++bVOjbl06VJER0fDy8sLtWrVgoWFBVxdXfH555/j+PHjJd4cprTmz5+PH3/8EZ6enqhVq5ZRp+XTxdXVFcePH8emTZswYMAAODk5wdLSEtWqVUPdunXh4eGB4OBg7N27V20IiaFeHQ/u4eFRbPtXQ3txoRwAhgwZgt9//x0TJkzAu+++i5o1a8Lc3ByOjo7w8/PDgQMH8O23376210+nTp1w+vRpjBo1Co6OjjAzM4OdnR169uyJmJgYzJ49+7XUUZGIMjMzq8a0A0REREREbyieKSciIiIiEhhDORERERGRwBjKiYiIiIgExlBORERERCQwhnIiIiIiIoExlBMRERERCYyhnIiIiIhIYAzlREREREQCYygnIiIiIhIYQzkRVQoymQyJiYmQyWRCl0IGYh9WfOzDio99KByGciKqNAoKCoQugcqIfVjxsQ8rPvahMBjKiYiIiIgExlBORERERCQwhnIiIiIiIoExlBMRERERCYyhnIiIiIhIYAzlREREREQCYygnIiIiIhIYQzkRERERkcAYyomIiIiIBMZQTkREREQkMIZyIiIiIiKBMZQTEREREQmMoZyIiIiISGAM5UREREREAmMoJyIiIiISGEM5EREREZHAGMqJiIiIiATGUE5EREREJDCGciIiIiIigTGUExEREREJjKGciIiIiEhgDOVERERERAJjKCciIiIiEhhDORERERGRwBjKiYiIiIgExlBORERERCQwhnIiIiIiIoExlBMRERERCYyhnIiIiIhIYAzlREREREQCYygnIiIiIhKYqdAFEBERUeXxUiHGjTv/Qiw2EboUMoBcXoCcnDzkVrE+rFPLGvXsbAWtgaGciIiIjCbrWS6Wb9hRpQJdZSKXFyA3VwZLS4sq1YdzgwMED+UcvkJEREREJDCGciIiIiIigTGUExEREREJjKGciIiIiEhgDOVERERERAJjKCciIiIiEhhDORERERGRwBjKqVxdunQJEyZMQOvWreHg4IB69erB3d0dY8aMwZEjR1TtQkJCIJFIEBMTo3Nb48aNg0Qiwfnz59Uel0gkaNeundpj4eHhkEgkWLlyZYk1Kvdd3E9ISIieR05ERERUerx5EJULuVyOOXPmIDQ0FKampujcuTN69+6NatWq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C7FixQpERUUhODjY4OMhIiIi0oWh/DWYM2cOZDIZQkND0a5dO3Tu3BnNmjVDtWrVkJSUhKNHjyI9PR1z5sxRraMcOuHr64uQkBBERUXBy8sL1tbWuHv3LuLi4vD8+XN88sknGjODHDx4EFOmTFFduFi/fn3VbeZPnz4NsViM5cuXa725TnG2b9+O58+fY+jQoVoDOVA4jtDf3x/Lly9HZGQkJk+erPfzpWRhYYHJkydjxowZWLZsGUJDQ4ttX7NmTcTExCAgIAArVqxAeHg4PvzwQzRo0AA5OTn4888/cfbsWZiammLRokWqmwPVqFFDNe5eG+X2pFIpQzkRERGVC4by10AsFuObb77BkCFDsGHDBiQkJCAhIQFyuRz29vbw8vJCYGAgunbtqrZe48aNcerUKWzcuBE7d+7E1q1bkZOTgzp16sDLywuffvopunTporG/BQsWwMPDA0eOHEFCQoJqWqP69etj6NCh+Pzzz+Hu7q73cSjHXpc0VCYgIADLly9HWFhYmUI5AIwYMQI//PADtmzZgv/85z9o3Lhxse2dnJxw5MgRbNmyBbGxsYiPj0dGRgYsLCxU31qMHDkSDRs2xKZNm5CTk1PshwygsB88PDxw5swZnD17Vm2GFiIiIiJjEGVmZiqELoKIqKxkMhmSk5Ph6OjIGQMqKPZhxSeTyXDp2i0s37Cj0s++Mjc4AC3edha6DKPj+1A4vNCTiIiIiEhgDOVERERERAJjKCciIiIiEhhDORERERGRwBjKiYiIiIgExlBORERERCQwzlNORERERmNT0xJzgwMq/ZSIdWpZC10CVTIM5URERGQ0piI5XFw4xzWRvjh8hYiIiIhIYAzlREREREQCYygnIiIiIhIYQzkRERERkcAYyomIiIiIBMbZV4iIiMhoXirEuHHnX6NMiVinljXq2dkaoSqiNx9DORERERlN1rNcLN+wwyihfG5wAEM5VRkcvkJEREREJDCGciIiIiIigTGUExEREREJjKGciIiIiEhgDOVERERERAJjKCciIiIiEhhDORERERGRwBjK30Djx4+HRCKBi4sL8vLytLZxc3ODRCIpdju62iQnJ2Pq1Klo3bo17O3t0aBBA7z33nvw9fXF999/j+zsbLX1S/uTlJQEABqP165dG02aNIGfnx+OHj1a4vH37dsXEokEnp6eJR6fvb19idtT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O+8gOjoaCxcuhLm5eZn3S0RERKQNQ7nAjh8/jqSkJHTs2LHYiysDAwNx7tw5SKVStGrVCl26dMHYsWPx008/oW3btujduzfs7e2Rnp6OuLg43L9/Hz4+PggKClLbzpo1a7BkyRK0atUK7u7uqFWrFtLT03HixAncunULtra2WLRoUbkdb58+feDu7o7jx4/j5MmTSExMxPPnzzF06FCdZ+rFYrFqjHdkZCQmT56sWvbixQuMGzdO5/7Wrl2r9XHlzYGGDh2qc9y9jY0NfHx8sHXrVuzZs8eod1YlIiIiKoqhXGDKIRQBAQHFthswYABmzpyJbdu2YfHixbC0tMSSJUvQoUMH/Prrr9i7dy+ysrJQo0YNNG/eHNOnT0dQUJDGRaBRUVE4ePAgTp06hX379uHJkycwNzdHo0aNEBwcjPHjx2sdQmJMM2fOhL+/PxYvXqyaQrCk4w8ICFBdeFk0lMvl8mIvStUWypXriEQiDB06tNj9BgYGYuvWrZBKpQzlREREVG5EmZmZvJc4EVV4MpkMycnJcHR05IwBFRT7sOKTyWS4dO0Wlm/YYZTZV+YGB6DF285lL4xKje9D4XD2FSIiIiIigTGUExEREREJjKGciIiIiEhgDOVERERERAJjKCciIiIiEhhDORERERGRwDhPORERERmNTU1LzA0OMMqUiHVqWRuhIqKKgaGciIiIjMZUJIeLC+e4JtIXh68QEREREQmMoZyIiIiISGAM5UREREREAmMoJyIiIiISGEM5EREREZHAOPsKERERGc1LhRg37vxb6ikR69SyRj0723KuiujNx1BORERERpP1LBfLN+wodSifGxzAUE4EDl8hIiIiIhIcQzkRERERkcAYyomIiIiIBMZQTkREREQkMIZyIiIiIiKBMZQTEREREQmMoZyIiIiISGBvfCi/dOkSJkyYgNatW8PBwQH16tWDu7s7xowZgyNHjqjanThxAhKJpFQ/bm5uqvWSkpL0al9USkoKFixYgM6dO8PJyQl169bF22+/DV9fX4SHhyM/P1+jvilTpug81vDwcEgkEqxcubJUz01ISIhGrfXr14enpye+/vprPH36VOt6pXmOivL29lZbVqtWLTRq1Ai9e/dGeHg4FAqFxnGOGzdOZ9262ry6H4lEgjp16qB58+b47LPPcO3atTI9Z8rnKyYmRutyffqTiIiI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bNiAhIQEJCQkQC6Xw97eHl5eXggMDESrVq3wzjvvoEaNGvj444+L3WZgYCDOnj0LqVRaYigHCs9Wvzpc5ObNmzh9+jQaNWqEDz74oNj6hw4diu+++w4RERGYOnWqatmlS5dw6dIlAED16tVRq1YtvPPOOxg+fDj8/f1Rr149VdujR4/i/v376Nixo8a3BUXZ2Nigb9++iI6Oxq5duzBkyJASj4+IiIhIX6LMzEzespCIKjyZTIbk5GQ4OjryG40Kin1Y8clkMmRnZ6NGjRrswwqK70PhcPYVIiIiIiKBMZQTEREREQmMoZyIiIiISGAM5UREREREAmMoJyIiIiISGEM5EREREZHAGMqJiIjIaHJycoQugahCYignIiIio5HJZEKXQFQhMZQTEREREQmMoZyIiIiISGAM5UREREREAmMoJyIiIiISGEM5EREREZHAGMqJiIiIiARmKnQBRERE9OZ4+CgdTzKeGrSuXF6AaiY830dkCIZyIiIiUnmS8RRfr4owaF25vABTRw0wckVEVQM/zhIRERERCYyhnIiIiIhIYAzlREREREQCYygnIiIiIhIYQzkRERERkcAYyomIiIiIBMZQXgElJSVBIpFo/Dg4OKBDhw5YsmQJnj9/rnP9U6dOqdaJjY3V2S48PBwSiQQrV67U2SYkJAQSiQQxMTE620RGRqr2d+HChRK3JZFIMGfOHJ3t5s2bp2oXEhKis11pjxMAkpOTMXXqVLRu3Rr29vZo0KAB3nvvPfj6+uL7779HdnZ2sesTERERlQXnKa/AXFxc4OvrCwBQKBRIS0vDwYMHsWTJEhw+fBj79++HiYmJxnpSqRQAIBKJEBYWhv79+5drnVKpFCKRCAqFAmFhYWjdunWx7U1NTREdHY358+fD1FT9Jfry5UtERUXB1NQUL1++LHG/QMnHeeXKFfj4+CArKwseHh7o3r07rKyscP/+fSQkJCAuLg79+vWDq6tr6Q+aiIiISA8M5RWYq6srZs2apfZYXl4eevTogfPnz+PkyZPo0qWL2vKnT59i586daN68Oezs7BAfH4/79++jYcOG5VLj7du3kZCQgN69e+PmzZvYtm0bFi9eDEtLS53rdO/eHfv378f+/fvh4+OjtiwuLg6pqano3bs39u3bp3Mb+hznl19+iaysLPz000/w9/fXWH7u3DnY2trqcdRERERE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ga1bt+p8mueUKVN0jldbsGABKlasWGDNAwcOxPLly3H27FkAhs1NvmPHDrx69Qr+/v5aAzkAmJiYwM/PD8uXL0dERATGjx+v9/aJiIiI9MVQTirvTolYpkwZODk5YdiwYRg/fjycnZ1V68zMzLB69Wr069cPoaGhOHv2LPbu3YuyZcuiTp06GDp0KIYNGwYrKyud+9u5c6fOdVOmTNErlFevXh1t27bFyZMnUbduXYNmh1E+fCggICDfdgEBAVi+fDmkUilDORERERULUVpaWq7QRRARvS+ZTIb79+/D2dmZMwYYqYKO4dV/7mB+SLgAlZG+FAo5Jg7rjcb1a/JzaKT4u1Q4nH2FiIiIiEhgDOVERERERAJjKCciIiIiEhhDORERERGRwBjKiYiIiIgExlBORERERCQwzlNORERGoVIFW8wck/9zBUhYCoUc5qZCV0FknBjKiYjIKDja28HR3k7oMigfyjmuichwHL5CRERERCQwhnIiIiIiIoExlBMRERERCYyhnIiIiIhIYAzlREREREQC4+wrRESk0+MnqXj2PL1E9qVQyPH6dRYyEx/CxITz6hmjvCkReb2PqDAYyomISKdnz9MxPyS8RPalUMiRmSmDlZUlQ7mRUijkmDist9BlEBklns4SEREREQmMoZyIiIiISGAM5UREREREAmMoJyIiIiISGEM5EREREZHAGMqJiIiIiATGUE5EREREJDCGclJz6dIljB49Gk2bNoWTkxMcHR3RuHFjfPXVVzh27BjWrl0LsViMb775Ruc2Tp48iQoVKuDTTz9FTk4OAEAsFqv9qVixIurUqYOAgACcPn1arX9YWJhGe0dHRzRr1gzfffcdkpOTte5XLBbD3d0939enq821a9cwYsQIuLu7w97eHi4uLmjSpAkGDhyIdevWITc3t6C3joiIiKjQ+PAgAgAoFArMmDEDa9euhZmZGdq3bw8vLy+Ym5vjzp07iImJQVRUFKZNm4a2bdsiPDwcPXv2hJeXl9p2Xr16hVGjRqFMmTL48ccfYWb274+YnZ0dhg8fDgDIysrCH3/8gf379+PAgQP49ddf4ePjo7atDh06oFWrVgCA1NRUnDhxAhs2bMD+/fsRFxeHSpUqFclrP3bsGHx9fZGTk4OOHTuiR48esLS0RGJiIk6fPo29e/di+PDhaq+FiIiIqCgxZRAAYMGCBVi7di3c3d2xefNmuLq6qq3PzMzEhg0bkJqairVr16Jt27YYN24cWrZsCTs7O1W7GTNm4N69e1i0aBHq1Kmjto2KFSti6tSpass2b96MsWPHYtasWRqhvGPHjpgwYYLq3wqFAn5+foiJicH69esxbdq0Innt3377LeRyOaKjo9G+fXu1dbm5uTh69ChMTfl0QSIiIio+HL5CuH37Nn744QfY2dlh+/btGoEcAKysrDB27FhMnToVLi4uWLRoEZ48eYJvv/1W1SY2NhahoaFo164dRo4cqde+Bw4cCGtra9y7dw/Pnj3Lt62JiQkCAgIAAJcvXzbgFer29OlTJCYmom7duhqBHABEIhE8PT0hEomKZH9ERERE2jCUE8LDwyGXyzF06FDY29vn27ZMmTIA8sK0l5cXoqOjsW3bNqSlpWHs2LGwtbXFmjVrChViDelTVFeubW1tYWZmhuTkZGRkZBTJNomIiIgMxeErhLNnzwKA1ivF+fnhhx9w7tw5TJo0Ca1bt8bDhw+xevVquLi46L2N8PBwZGRk4KOPPkLFihXzbatQKBAWFgYA8PDwMKhWXcqUKQMvLy/s2bMHXbp0weDBg9GyZUvUq1cPFhYWBm1LJpMVSU1UONnZ2Wp/U9FQKORQKOQltC+F2t9kfJTHjp9D48XfpUXH0tLSoPYM5YQnT54AAJycnAzqZ29vj5UrV2LQoEHYv38/vLy8MHDgQJ3tU1JSEBwcDCDvRs+rV6/iyJEjMDExwbx58zTaHz9+XBV0nz9/jri4OPzzzz9o2bIlvvjiC4Nqzc8PP/yAN2/e4ODBg5g8eTIAwMLCAk2aNEHv3r0xePBgWFlZFbidpKQkyOUlE15IN12z81DhvH6dhczMkj3hzMpiGDB2/BwaPx7D92Nqago3NzeD+jCU03v5/PPP0axZM/z++++YM2dOvm1TU1OxZMkSAHk/rBUrVkT37t0xevRotG7dWqN9XFwc4uLi1Ja1atUKu3btUg2jKQp2dnaIjIzErVu3cOTIEfz+++/47bffkJCQgISEBGzevBn79u1DhQoV8t2OoSc1VLSys7ORnJwMBwcHg7/lIN0yEx/Cysqwqz2FpVAokJWVjTJlLGBiwtGVxkh5pZyfQ+PF36XCYSgn2Nvb4/r160hKSkKtWrUM7q/8eqagr2lq1aqF8+fP673d2bNnY8KECVAoFLh37x6Cg4OxZcsWjB07Fj/99JNGe5FIlO984sr/Wej6n32NGjVQo0YN1b+vXLmCr7/+GteuXcPixYtVJxS6GPo1FRUPCwsLHosiZGJiChOTkp19yMTEpMT3SUWLn0Pjx2NY8ngpglRzgZ84cULgSrQzMTFB9erV8eOPP6J169bYsmUL9u7dq9HO1tYWz58/1xnMU1JSVO300bBhQ1UQP3nyZCGrJyIiIioYQzkhICAApqamCA0NLXBawqysrBKqSpNIJMLixYshEokwb948jZvB6tWrh4yMDPz5559a+587dw4AUL9+fb33aWNjU/iCiYiIiPTEUE5wc3PDuHHjkJKSgn79+uHOnTsabWQyGVavXo3FixeXfIFvadiwIby9vXH9+nVERUWprfP39weQN+zl3ZOHtLQ01U2mynYAkJGRgWXLlqmuor8tJycHq1atAvDvtwlERERExYFjyglA3pM4ZTIZ1q5dixYtWqB9+/aoW7cuzM3NcffuXRw/fhypqamYMWOG0KVi8uTJ2LdvH5YuXYp+/frBzCzvx3jgwIGIiYnB3r170axZM3z22Wews7NDcnIy9u/fj5SUFIwYMQIdOnRQbevNmzdYsGABFi9ejBYtWqBBgwawtbXFkydPcPToUTx8+BAfffSRalYWIiIiouLAUE4A8sZtL1q0CP3798fGjRsRHx+P+Ph4KBQKODg4wNPTE4GBgejYsaPQpcLd3R09e/bE7t27ERERgaCgIAB5r2Hz5s2QSqWIjIzE9u3bkZGRgfLly6Nx48YYPHgwPv/8c7Vt2draYuvWrYiNjcXZs2exa9cupKamomzZsqhRowYGDRqEESNGoHz58kK8VCIiIvqPEKWlpemeroKIyEjIZDLcv38fzs7OnDGgCF395w7mh4SXyL4UCjkyM2WwsrLk7CtGSqGQY+Kw3mhcvyY/h0aKv0uFwzHlREREREQCYygnIiIiIhIYQzkRERERkcAYyomIiIiIBMZQTkREREQkMIZyIiIiIiKBcZ5yIiLSqVIFW8wcE1Ai+1Io5Hj9OhNly1pxSkQjpVDIYc5DR1QoDOVERKSTo70dHO3tSmRf/86PXJXzIxsp5TEkIsNx+AoRERERkcAYyomIiIiIBMZQTkREREQkMIZyIiIiIiKBMZQTEREREQmMs68QEZWgx09S8ex5utBllEp5UyJmITPxIadENFJ5UyLyeh9RYTCUExGVoGfP0zE/JFzoMkolhUKOzEwZrKwsGcqNlEIhx8RhvYUug8go8XSWiIiIiEhgDOVERERERAJjKCciIiIiEhhDORERERGRwBjKiYiIiIgExlBORERERCQwhnIiIiIiIoExlBuRu3fvQiwWa/xxcnJC69atsXjxYrx69Uqtj7u7O8Ricb7b1dYmLCwMYrEYK1eu1Lu+nJwcbNmyBf7+/qhbty7s7e3h5OSEZs2a4auvvsKePXugUCh09s/NzUWTJk0gFosxYMCAfPf17ntQsWJF1KpVC76+vjh+/LjWPsHBwRCLxdi+fbvO7UZERKi2eeHCBb1eNxEREdH74sODjJCrq6sqtObm5iIlJQWHDx/G4sWLERsbi4MHD8LUtGQfvHHv3j0MHDgQV65cQcWKFdGhQwc4OztDoVDg7t27OHLkCKKiouDt7Y2wsDCt2zh58iQSExMhEokQGxuLR48eoUqVKjr3aWdnh+HDhwMAsrKy8NdffyEmJgaHDh3Czz//jH79+hn8OiQSCUQiEXJzcyGVStG0aVODt0FERERkKIZyI+Tm5oapU6eqLcvKykKXLl1w/vx5nDp1Ch06dCixetLT09G3b1/cuHED48aNw5QpU2BlZaXW5s2bN9i6dSsOHjyocztSqRQAMHr0aISEhCA8PBwTJ07U2b5ixYoa78P27dsxbNgwzJ071+BQfuvWLcTHx8PLyws3btzAtm3bsHDhQo3XQkRERFTUOHzlA1GmTBm0a9cOAJCamlqi+161ahVu3LgBf39/zJ07V2uINTc3R0BAAH755Ret20hLS8Pu3btRr149TJs2DeXKlYNUKkVubq5BtfTp0wfW1ta4f/8+UlJSDOqrPCnw8/ODr68v0tPTsWvXLoO2QURERFQYDOUfiOzsbJw6dQoikQju7u4luu/w8HAAwPfff19gWzMz7V/ObNu2DTKZDH5+frCyssLnn3+OxMREnDp1qtB1GTKERy6Xq8aTd+vWDb6+vhCJRJBIJIXePxEREZG+OHzFCN2+fRvBwcEA8saUp6amqsZgz5s3DzVr1iyxWu7fv4+kpCRUq1YNrq6uhd6ORCKBiYkJ+vfvDwDw9fVFWFgYJBKJ6hsAfWzfvh0ZGRmoW7dugTe4vi0mJgaPHz/G0KFDUaZMGbi4uMDDwwPx8fG4ffs23NzcCtyGTCbTe39U9LKzs9X+Lq0UCjkUCrnQZZRKyhvB87shnEo35bEr7Z9D0s1YfpcaA0tLS4PaM5QbocTERCxZskRjedeuXUt0LDkAPHnyBADg6Oiodf3atWvx4sULtWUjR45UC8xXrlzB5cuX8emnn6pu7GzXrh2qVauGPXv24MWLFyhfvrzGtlNSUlQnJ2/f6GljY4Ply5cb9DqUV8T9/PxUy/z8/BAfHw+pVIpZs2YVuI2kpCTI5QxbQktOTha6hHy9fp2FzEyewOUnK4thwNiV9s8hFYzH8P2YmprqdUHvbQzlRsjT01NtWr/U1FScPXsWU6ZMQbdu3bB79240b95cwAr/tW7dOty/f19tWUBAgFoo1xaIRSIRfH19sXz5cmzbtg3Dhg3T2HZqaqrGyYmNjQ127tyJFi1a6F1jcnIyYmJi4ObmhpYtW6qW+/j4YPLkyYiIiMD06dMLHA7j5OSk9z6p6GVnZyM5ORkODg6wsLAQuhydMhMfwsrKsKsn/xUKhQJZWdkoU8YCJiYcXWmMlFfKS/vnkHQzlt+lHyKG8g+AnZ0dunfvjrJly8LHxwcLFixAdHQ0AKj+x6ZQKHT+Ty43NxcikahQ+65cuTIA4PHjx1rX//HHH6r/7tu3L2JjY9XWy2QyREVFwcbGBj179lRb5+fnh+XLl0MqlWoN5bVq1cL58+cB5N0oum/fPkycOBEDBw7EsWPH9A7JERERyMnJga+vr9pyW1tbdO/eHdu3b8eRI0fQtWvXfLdj6NdUVDwsLCxK9bEwMTGFiUnJTllqbExMTPgeGbnS/jmkgvEYljxeiviANGvWDADUHnpja2sLQPeMLLm5uXj+/LmqnaFcXFzg5OSEBw8eIDEx0eD+yuEpr169gpOTk9oDgZRXuy9evIirV6/mux2xWIzAwEAsXboUycnJmDRpkt41KGddUT5c6O0/ym8keMMnERERFSdeKf+ApKWlAYDaNIL16tXDH3/8gXPnzqF79+4afa5evYqMjAy0bt260PsNCAjAsmXLsGzZMqxZs8agvsqw6+Pjg3LlymmsT0pKQmxsLCQSidZx9O8KCgrCxo0bsX//fiQkJKgNR9EmPj4eN2/ehKurK9q2bau1zYEDB3Do0CE8ffpU9c0AERERUVFiKP+AKAPx2wE7ICAAW7ZswaJFi9C6dWu1sdxZWVmYPXs2APXx3IYaO3YsoqOjERYWBnt7e0yePFnjK6+cnBy8fv1abdmdO3dw8uRJuLi44Ndff9U6hObFixf4+OOPERUVhXnz5qFMmTL51iISiTB58mQEBARg4cKF2L17d77tlScFymEv2sybNw8rVqxAZGQkxowZk+/2iIiIiAqDodwIvT0lIgA8f/4cCQkJuHz5MsRiMebMmaNa16FDB4wYMQI//vgjmjdvDi8vLzg4OCA1NRUxMTF48OABevTooTOQRkdH4/r161rXeXt7o0ePHrC1tcWOHTsQGBiIlStXYvPmzejYsSOcnZ2Rk5OD5ORkxMXF4cmTJ6hXr55qJhXlw4H8/f11jmkvX748evToga1bt2Lfvn3o06dPge9P9+7d0bhxY5w4cQKnTp3SeQVc+XAga2tr+Pj46NxeQEAAVqxYAYlEwlBORERExYKh3Ai9OyVimTJl4OTkhGHDhmH8+PFwdnZWa7948WK0bt0amzZtwv79+/HixQtYW1ujfv36+P777zFw4ECdN4FevnwZly9f1rrOxcUFPXr0UP33sWPHsG3bNuzcuROnT59GamoqzMzM4ODggHbt2qF3797w8vKCqakpFAoFIiIiIBKJ4O/vn+/rDQwMxNatWyGRSPQK5QAwZcoU+Pn5YeHChThw4IDWNjt27MDr16/h7+8PGxsbnduqWbMmWrVqhbNnz+o1JIaIiIjIUKK0tDTDnmNORFQKyWQy3L9/H87OzqV6xoCr/9zB/JBwocsolRQKOTIzZbCysuTsK0ZKoZBj4rDeaFy/Zqn+HJJuxvK79EPE2VeIiIiIiATGUE5EREREJDCGciIiIiIigTGUExEREREJjKGciIiIiEhgDOVERERERALjPOVERCWoUgVbzBwTIHQZpZJCIcfr15koW9aKUyIaKYVCDnMeOqJCYSgnIipBjvZ2cLS3E7qMUunf+ZGrcn5kI6U8hkRkOA5fISIiIiISGEM5EREREZHAGMqJiIiIiATGUE5EREREJDCGciIiIiIigTGUExEREREJjFMiEtF/0uMnqXj2PF3oMugtefOUZyEz8SHnKTdSefOU83ofUWEwlBPRf9Kz5+mYHxIudBn0FoVCjsxMGaysLBnKjZRCIcfEYb2FLoPIKPF0loiIiIhIYAzlREREREQCYygnIiIiIhIYQzkRERERkcAYyomIiIiIBMZQTkREREQkMIZyI3Dp0iWMHj0aTZs2hZOTExwdHdG4cWN89dVXOHbsmEZ7mUyGdevWwcvLC66urrC3t0e9evUwZMgQxMXFad3H3bt3IRaL0bdvX73runz5Mr755hs0atQIjo6OcHFxQceOHbFkyRK8ePFCa5+RI0dCLBZDLBZj/fr1Orc9dOhQVbuwsDC1de7u7qp1yj/29vZo2LAhxo0bh7t372psLzg4GGKxGNu3b9e5z4iICNX2Lly4oOe7QERERPT+OE95KaZQKDBjxgysXbsWZmZmaN++Pby8vGBubo47d+4gJiYGUVFRmDZtGr7//nsAwO3btzFgwADcvHkT1atXR+/evVG+fHlV++joaAwZMgTLli2DmVnhD/+SJUuwePFimJmZoVOnTujduzcyMzNx6tQpBAcH45dffkFERASaNm2qtb+ZmRmkUim++uorjXXPnz/H/v37YWZmhpycHK39TU1NMWnSJNW/X7x4gd9//x2bNm3Cnj17EBcXB2dnZ4Nek0QigUgkQm5uLqRSqc7aiYiIiIoaQ3kptmDBAqxduxbu7u7YvHkzXF1d1dZnZmZiw4YNSE1NBZAXTPv27YvExER89913mDJlCkxN/30Ax6NHjxAYGIjQ0FDY2tpi3rx5haprw4YNCA4ORvXq1REVFYXatWurrf/1118xadIk9OvXDydOnEC1atU0ttG5c2ccPHgQf/zxB9zd3dXWbdmyBVlZWfDy8sKBAwe01mBmZoapU6dqLJ80aRJ+/vlnbN68GdOnT9f7Nd26dQvx8fHw8vLCjRs3sG3bNixcuBBWVlZ6b4OIiIiosDh8pZS6ffs2fvjhB9jZ2WH79u0agRwArKysMHbsWFU4DQkJQWJiIgYMGIDp06erBXIAqFKlCiIjI1GhQgWsXr0at2/fNriutLQ0zJs3DxYWFoiMjNQI5EDe0JPx48cjNTUV8+fP17odf39/mJqaQiKRaKwLCwtDnTp18Mknnxhcn6enJwCoTlT0JZVKAQB+fn7w9fVFeno6du3aZfD+iYiIiAqDobyUCg8Ph1wux9ChQ2Fvb59v2zJlygCAauz1d999p7Otvb09Bg8eDIVCgfBwwx8xvmvXLrx8+RI9e/bExx9/rLPdmDFjYGlpiR07duD169ca652cnNCpUyds27YN2dnZquWXLl3CH3/8gcDAQINrA4CjR48CABo1aqR3H7lcrhpP3q1bN/j6+kIkEmk9YSAiIiIqDgzlpdTZs2cBAO3bt9er/b179/Do0SM4OTmhVq1a+bbt0KEDAODcuXMG15WQkKC2DV3EYjEaNWqEN2/e4NKlS1rbDBw4EKmpqdi/f79qmVQqhZmZGfz8/PLdfk5ODoKDg1V/pk2bhm7dumHjxo3o06dPgf3fFhMTg8ePH6N3794oU6YMXFxc4OHhgfj4+EJ9m0BERERkKI4pL6WePHkCIO+KsiHtq1atWmBbZZvk5ORC11UU++nevTsqVqwIqVQKHx8fyGQybNu2DZ999lmB3w7I5XIsWbJEY3m9evXQu3dvWFhYFFifkvKK+NtB3s/PD/Hx8ZBKpZg1a5Ze25HJZHrvk4qe8huXt795yY9CIYdCIS/OkshACoVC7W8yPspjp+/nkEofQ3+Xkm6WlpYGtWcoJ8GYm5tjwIAB+Omnn5CUlIT4+HikpaVh4MCBBfYtU6aMWth/9eoV/v77b8ydOxdBQUFYsmQJvv766wK3k5ycjJiYGLi5uaFly5aq5T4+Ppg8eTIiIiK0js/XJikpCXI5Q57Q9D3ZfP06C5mZPJEqjbKyGAaMXWEu+lDpwmP4fkxNTeHm5mZQH4byUsre3h7Xr19HUlJSgcNRlO0B4OHDhwW2VbZxcHAoVF1FuZ+BAwdi3bp1CA8Px6lTp+Dg4IDPPvvM4LpsbGzQvHlzSCQS1K9fHwsXLkRQUBDKli2bb7+IiAjk5OTA19dXbbmtrS26d++O7du348iRI+jatWuBNej7rQYVj+zsbCQnJ8PBwUGvb0oyEx/CysqwqxhUvBQKBbKyslGmjAVMTDi60hgpr5Tr+zmk0sfQ36VUdBjKS6lWrVrh1KlTOHHiRIHjtwHAxcUFVapUQVJSEm7cuJFvkFc+QKgws5u0bNkS4eHhiIuLw6BBg3S2S0tLw+XLl2FhYYHGjRvrbFe/fn00bdoUP//8M548eYIxY8a81/zpYrEYNWvWxOXLl3Hz5k00bNgw3/bKWVeUY9O1kUgkeoVyQ7+mouJhYWGh17EwMTGFiUnB34BQyTMxMeGxMXL6fg6p9OIxLHm8FFFKBQQEwNTUFKGhoXj27Fm+bbOyslR9AGDZsmU62z59+hSbN2+GiYmJqr0hevXqBRsbG+zZswfXr1/X2W716tWQyWTo3bt3gVerBw4ciMePH0OhUOg1dKUgaWlpAAoelxofH4+bN2/C1dUVQUFBWv9UqlQJhw4dwtOnT9+7LiIiIiJdGMpLKTc3N4wbNw4pKSno168f7ty5o9FGJpNh9erVWLx4MYC8aQg/+ugjbNmyBUuWLNEY35ycnIyAgACkpqZi9OjRBo91AvKuRM+YMQPZ2dnw8/PDzZs3Ndps3rwZK1euhJ2dHWbOnFngNgcMGACpVIpt27bpNVQnP3v27MHdu3chFotRr169fNsqb/CcOHEiQkJCtP4ZNGgQ3rx5g8jIyPeqi4iIiCg/HL5Sis2YMQMymQxr165FixYt0L59e9StWxfm5ua4e/cujh8/jtTUVMyYMQNAXmDevn07BgwYgODgYERGRsLT0xO2tra4c+cOYmJi8OrVKwwePFjnjCLXrl3DyJEjta6rXbs2JkyYgBEjRiAlJQX/+9//0Lp1a3h6eqJOnTqQyWQ4deoUrl69Cnt7e0RERGh9mue7bGxs0KNHD4PeG+WUiEqvX7/G33//jSNHjkAkEmHp0qX5joVTPhzI2toaPj4+OtsFBARgxYoVkEgkGDNmjEE1EhEREemLobwUMzExwaJFi9C/f39s3LgR8fHxiI+Ph0KhgIODAzw9PREYGIiOHTuq+tSsWROnT5/GL7/8gt27d2Pr1q14/fo1KlWqBE9PT3zxxRf5jlF/9OgRIiIitK5r06YNJkyYAACYPn06vL298eOPP+L06dM4evQoLCws4OrqiilTpmDEiBEQi8VF+XaoeXdKRDMzM1SqVAk9e/bEqFGj1GZS0Ub5UCN/f3/Y2NjobFezZk20atUKZ8+eRUJCQoHbJSIiIioMUVpaWq7QRRARvS+ZTIb79+/D2dlZr5uTrv5zB/NDDH+qLRUfhUKOzEwZrKwseaOnkVIo5Jg4rDca16/JmwSNlKG/S6nocEw5EREREZHAGMqJiIiIiATGUE5EREREJDCGciIiIiIigTGUExEREREJjKGciIiIiEhgnKeciP6TKlWwxcwxAUKXQW9RKOR4/ToTZctacUpEI6VQyGHOQ0dUKAzlRPSf5GhvB0d7O6HLoLf8Oz9yVc6PbKSUx5CIDMfhK0REREREAmMoJyIiIiISGEM5EREREZHAGMqJiIiIiATGUE5EREREJDCGciIiIiIigXFKRKJS7vGTVDx7ni50GaVe3hzXWchMfMg5ro0Uj6Hxy5unnNf7iAqDoZyolHv2PB3zQ8KFLqPUUyjkyMyUwcrKkoHOSPEYGj+FQo6Jw3oLXQaRUeLpLBERERGRwBjKiYiIiIgExlBORERERCQwhnIiIiIiIoExlBMRERERCYyhnIiIiIhIYAzlVKC7d+9CLBZr/HFyckLr1q2xePFivHr1Sq2Pt7e3WtsKFSrAxcUFXbt2xa+//gqFQpHvPpcsWQKxWIxKlSohOTlZa5uwsDCtdWn74+3trep38uRJiMViTJgwQW17I0eOhFgsxvnz5wv5ThEREREVDucpJ725urpiwIABAIDc3FykpKTg8OHDWLx4MWJjY3Hw4EGYmqrPLTx69GhYW1tDLpfj/v372Lt3LyZMmIDLly/j//7v/7TuJzc3F2FhYRCJRMjJyUFERATGjx+v0c7d3R2TJ0/Ot+aff/4ZKSkpqFu3bqFeMxEREVFJYCgnvbm5uWHq1Klqy7KystClSxecP38ep06dQocOHdTWjxkzBg4ODqp/3759G+3atcOmTZswfvx4VK9eXWM/cXFxuHfvHoYMGYIdO3ZAKpVqDeUNGzZEw4YNddYbEhKClJQUNG7cGAsWLDDsxRIRERGVIA5fofdSpkwZtGvXDgCQmppaYHs3Nze0adMGubm5uHz5stY2EokEADBkyBD06tULN2/eRHx8vEF1HT9+HHPmzEHlypUhlUphaWlpUH8iIiKiksRQTu8lOzsbp06dgkgkgru7u0F93x3qAgDPnz/H3r178fHHH6Nx48bw8/MD8G9Q18edO3cwdOhQiEQihIaGolq1agbVRURERFTSOHyF9Hb79m0EBwcDyBv3nZqaitjYWDx69Ajz5s1DzZo19drG6dOnYW5ujmbNmmmsj4qKQlZWFnx9fQEArVu3houLC3bt2oUlS5bA1tY23+1nZGQgICAAz58/x9KlS9GmTZtCvFIiIiKiksVQTnpLTEzEkiVLNJZ37dpVYyy5UkhIiOpGzwcPHmDPnj3IyMjAggULUKVKFY32EokEJiYmqhtKRSIRBgwYgGXLlmHHjh0YMmRIvjV+8803uHbtGgIDA/HVV18Z/iLfg0wmK5btKhRyKBTyYtn2h0Q5o09BM/tQ6cVjaPyUxy47O1vgSqiwlMeOx/D9GTp0lqGc9Obp6Ynt27er/p2amoqzZ89iypQp6NatG3bv3o3mzZur9Vm9erXGdpYuXao1MF+8eBFXr15Fhw4dULVqVdVyf39/LFu2DBKJJN9QvmzZMuzatQvNmzfHihUrCvEK309SUhLk8qIPz69fZyEzs3gC/4coK4v/IzF2PIbGT9dUtmQ8eAzfj6mpKdzc3Azqw1BOhWZnZ4fu3bujbNmy8PHxwYIFCxAdHa3W5p9//oGDgwMyMzPx22+/YcyYMZg2bRpq1KgBT09PtbbKcePKceRKNWrUQIsWLXD+/Hn89ddfWqc3PHToEBYtWgQHBwds3rwZZcqUKdoXqwcnJ6di2W5m4kNYWfFG1YIoFApkZWWjTBkLmJjwdhljxGNo/JRXyh0cHGBhYSFwNVQY2dnZSE5O5jEUAEM5vTfl2PALFy7obGNlZYV27dohKioKbdq0wejRo/H777+jbNmyAIDMzExs27YNQN5DfEaOHKl1OxKJBIsWLVJbdvPmTQwfPhxmZmbYtGlTsYXjghTXDC8mJqYwMdG8KZa0MzEx4ftl5HgMjZ+FhQVnvTJyPIYlj6Gc3ltaWhqAvJs/C1K7dm18+eWXWLduHdatW4eJEycCAHbt2oX09HS4u7ujcePGWvtu3boVW7ZswZw5c1Rn7+np6QgICEB6ejpWrlyJVq1aFclrIiIiIipJDOX03tasWQMgb6YUfUyYMAGhoaEICQnB8OHDYWtrqxq6snDhQrRv315rP+XV9AMHDqBXr17Izc3FV199hevXr2PIkCEYOnRo0bwgIiIiohLGUE56e3tKRCBvTvGEhARcvnwZYrEYc+bM0Ws79vb2+OKLL7BmzRqsXbsWAwYMQHx8PFxcXFQPItImMDAQ27Ztg0QiQa9evRASEoKDBw/CwsICdnZ2arVp8+7TSHX53//+h4oVK2pdN2HCBNSuXVuv7RARERHpi6Gc9PbulIhlypSBk5MThg0bhvHjx8PZ2VnvbY0bNw6//vor1q5diydPniA3Nxf+/v4QiUQ6+3To0AHVqlXD0aNH8eDBA/z1118A8m5K0We2FX1DeUxMjM51AQEBDOVERERU5ERpaWkFDwQmIsFc/ecO5oeEC11GqadQyJGZKYOVlSVvEjRSPIbGT6GQY+Kw3mhcvyZvEjRSMpkM9+/fh7OzM49hCeOcU0REREREAmMoJyIiIiISGEM5EREREZHAGMqJiIiIiATGUE5EREREJDCGciIiIiIigTGUExEREREJjA8PIirlKlWwxcwxAUKXUeopFHK8fp2JsmWtOMe1keIxNH4KhRzmPHREhcJQTlTKOdrbwdHeTugySr1/H3hRlQ+8MFI8hsZPeQyJyHAcvkJEREREJDCGciIiIiIigTGUExEREREJjKGciIiIiEhgDOVERERERAJjKCciIiIiEhhDORERERGRwBjKiYiIiIgExlBORERERCQwhnIiIiIiIoExlBMRERERCYyhnIiIiIhIYAzlREREREQCYygnIiIiIhIYQzkRERERkcAYyomIiIiIBMZQTkREREQkMIZyIiIiIiKBMZQTEREREQmMoZyIiIiISGAM5UREREREAmMoJyIiIiISGEM5EREREZHAGMqJiIiIiATGUE5EREREJDCGciIiIiIigTGUExEREREJjKGciIiIiEhgDOVERERERAJjKCciIiIiEhhDORF9MExNTYUugd4Tj6Hx4zE0fjyGwhClpaXlCl0EEREREdF/Ga+UExEREREJjKGciIiIiEhgDOVERERERAJjKCciIiIiEhhDORERERGRwBjKiYiIiIgExlBORERERCQwhnIi+qC8efMGu3btwogRI/DJJ5+gatWqqFatGjw9PbFx40bI5XKhSyQ9XLlyBfPmzUOfPn1Qo0YNiMVieHt7C10W6XDhwgX0798fLi4ucHJyQufOnbFz506hyyI9bNmyBePHj0fHjh1hb28PsViMsLAwocv6TzITugAioqKUmJiIwYMHw8bGBu3bt4eXlxfS09Nx8OBBTJw4ETExMYiMjIRIJBK6VMrHvn37sGLFClhYWKBmzZpISUkRuiTS4cSJE+jbty8sLS3Rp08f2NjYYPfu3Rg6dCgePHiAMWPGCF0i5WPBggW4f/8+KlasCAcHB9y/f1/okv6z+ERPIvqgJCUlYf/+/fD394e1tbVqeUZGBnr06IGLFy8iNDQUPj4+whVJBfrrr7+QlZWF+vXrIzU1FXXq1EGbNm2wb98+oUujt+Tk5KBFixZISkrC4cOH0bBhQwDAixcv4OnpiXv37uG3336Di4uLwJWSLsePH4ebmxtcXFywcuVKzJ07F2vWrEFgYKDQpf3ncPgKEX1QnJyc8OWXX6oFcgCwtrbGqFGjAACnT58WojQyQN26ddG4cWOYm5sLXQrl48SJE0hMTES/fv1UgRwAypcvj2+//RbZ2dmIiIgQsEIq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
"/>
</div>
</div>
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,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mzejffv2WLNmDWJiYvDHH38gOjoa//vf/zBs2DDUr19fa4WbqKgotGzZEj179sTPP/+MY8eO4fLly4iLi0N4eDj69Omjvr6iV69eGqtF5GX//v3qn3fv3r2N3k+1LGZB56MD2fOUFy5cCCB73m6nTp2wYsUKxMfHIz4+HitXrkSnTp3Uc3q///57nStPqE56ZDIZvL29ERQUhMuXL+PcuXP46aef0LFjR2RkZGjdfKoofP311+o1/BctWoRhw4ap87Vz5050794dR48eVY/oFoZq5PrixYtYvnw5rl69inv37uHevXtFMpLdpUsXjB8/HkD2lI5WrVphwYIFOHnyJP744w/ExsYiPDwc06ZNw4cffojRo0cX+g6zOQtq1UmboaJc9buYc0BC3w23hg4dqj7Wjh070LNnT+zatQuXL1/G8ePHMXbsWHz11VcAsk+uTbnylC7u7u4YMWIEgOwpXZ06dYJUKsXly5dx+vRpTJs2DaNHjzbJa6cweKEnUSmimrdqiIODA4YOHYoZM2bkucRXcdGnTx98//33+Pbbb/Hq1Sv13R1VbG1tsWnTJqxYscLgnOFRo0ahXLly+Prrr5Gamop169Zh3bp1OtuKxWKN1RGioqKwatUqAMDHH3+s8659rVq1wrRp07BkyRJER0djxYoVmDx5cgGesaZBgwZhxYoV6u8tLS0NriAzZswYnDx5EidOnMCdO3cwYcIEje02NjZYt24djhw5Uqh55YsWLcLly5dx69YtHDt2TP0JjUrHjh2xZMkSg4V52bJlsXPnTkycOBE7d+7EjRs3MGvWLL3tc6+8AmSPhuf8CF+Xdu3aqef+Gyvn9JP8rD/foUMHSCQSpKSkICwsrMD3Ihg6dChevXqF+fPnIykpCd9++61WGwsLC8yePVtdsOT20UcfYfz48Vi1ahWePn2q9XqsUKECQkND8d133+kcSTclBwcH7NixAz4+Pnj27Bl27typNTXH398f7dq1w7hx4wrVl2r+f3JyMubPn4/58+ert7Vr1w4HDhwo1PF1WbBgARwdHbF48WIkJibixx9/1PsJXtmyZQ2uP2+M3KPc1tbWBtfpbtOmDUQikcaot76RcgsLC2zduhUBAQHq6S665su7uLggLCys0DdMM8aiRYvwzz//YN++fTrf12rUqIFNmzahSZMmRR6LPhwpJyqlxGIx7O3tUa1aNbRq1QojR47Ehg0bcOPGDcyfP7/EFOQqEyZMwOHDh+Ht7Y1KlSrBysoKrq6uGDx4ME6ePKledSMvAQEB+OOPPzB79my0bdsWFStWhKWlJWxtbVGzZk10794dixYtwh9//KGeI5mSkoIvv/wSSqUSFStWxOrVq/Ue///+7//UN9xYuHBhoeavq9SvX1/jD02XLl10FqcqZcqUQXh4OJYsWYKmTZvC1tYWNjY2cHNzw7BhwxAVFQUfH59Cx1WxYkUcPXoU06ZNQ926dWFtbQ0HBwe0atUKy5cvx65du4x6HdrZ2eF///sfjh49ii+++AL16tWDvb09LCws4ODgAHd3dwwZMgSbN2/Wmk86ceJESKVSjBgxAq1atYKrqyusra1hZWWFatWqoVevXggKCsL+/fvztVbykydP1B/NN2vWLF8fzZcpU0Y9heX+/fuFuvhv4sSJiImJwbBhw1C7dm3Y2trC1tYW77//Pr744gtER0djypQpBo+xYMECBAUFoX379rC3t4eVlRVq1aqFMWPG4PTp0+pR5Xehfv36OH/+PCZNmoT3338fVlZWqFChAjw9PbFhwwasWbPGJP24uLjgxIkTGDJkCNzc3ApdABvrq6++woULFzB16lQ0b94cjo6OsLS0hJ2dHWrXro0+ffqop+EVZrUhAGjUqJHGJ6FNmzY1uIxrzruJAtn3Vsh5bYiu9vv378fGjRvRrVs3ODs7o0yZMpBIJGjVqhXmz5+PuLg49c2rilqZMmUglUrx66+/wsPDA/b29rC1tUW9evUwdepUREVFGXw+74IoJSVFmAVmiYiIiIgIAEfKiYiIiIgEx6KciIiIiEhgLMqJiIiIiATGopyIiIiISGAsyomIiIiIBMainIiIiIhIYCzKiYiIiIgExqKciIiIiEhgLMqJiIiIiATGopyISjSZTIZ79+5BJpMJHQoZwDyZP+bI/DFHxRuLciIq8eRyudAhkBGYJ/PHHJk/5qj4YlFORERERCQwFuVERERERAJjUU5EREREJDAW5UREREREAmNRTkREREQkMBblREREREQCY1FORERERCQwFuVERERERAJjUU5EREREJDAW5UREREREAmNRTkREREQkMBblREREREQCY1FORERERCQwFuVERERERAJjUU5EREREJDAW5UREREREAmNRTkREREQkMBblREREREQCY1FORERERCQwFuVERERERAJjUU5EREREJDAW5UREREREAmNRTkREREQkMBblREREREQCY1FORERERCQwFuVERERERAJjUU5EREREJDAW5UREREREAmNRTkREREQkMBblREREREQCY1FORERERCQwUUpKilLoIIhKgut3HkEuVwgdBuWiUMiRnp4BW1sbiMUWQodDejBP5o85Mn/MUf5VLG+Pyk6OQocBALAUOgCikmLZhp14nZoudBiUi0IhR0aGDDY21vwjZcaYJ/PHHJk/5ij/5kzwN5uinNNXiIiIiIgExqKciIiIiEhgLMqJiIiIiATGopyIiIiISGAsyomIiIiIBMainIiIiIhIYCzKiYiIiIgExqLcDI0bNw4SiQS1atVCZmamzjbu7u6QSCQGj6OvTUJCAqZOnYpmzZrB2dkZVatWRaNGjTBw4ED8/PPPSEtL09jf2K+HDx8CgNbjFSpUQJ06deDr64tTp07l+fy9vb0hkUjg4eGR5/NzdnbO83iqmFq2bKl3u1KpRNOmTSGRSDBw4ECjjklERERkKrx5kJl5/fo1du/eDZFIhOTkZBw4cAD9+vUz2fGvXr2KXr164eXLl2jTpg26du0KOzs7PH78GDExMYiMjETv3r3h5uaGsWPH4uXLlxr7h4aGIiEhAWPGjIGDg4PGtpzfOzo6YuTIkQCAzMxMXL9+HZGRkThy5Ag2bNiA/v3764zvwYMHiI6OhkgkwvXr1/H777+jRYsWJnv++pw5cwb379+HSCTC8ePH8fTpU1SpUqXI+yUiIiICWJSbnV27diEtLQ3jxo3D2rVrIZVKTVqUf/PNN3j58iXWrVsHPz8/re1xcXFwdMy+s9WXX36ptT06OhoJCQkYO3YsatSoobefChUqYObMmRqPRUREYPjw4Zg/f77eojw4OBhKpRITJkzAypUrIZVK30lRHhwcDAAYP348Vq5cidDQUEydOrXI+yUiIiICOH3F7EilUlhaWmLSpEnw9PREVFQUHj16ZLLjx8fHw8HBQWdBDgCtWrXKc1pMQfXr1w/lypVDQkICEhMTtbbL5XKEhobC0dERc+bMgZubG3bu3KmeTlNUUlJSsHfvXnz44YeYNWsW3nvvPfXJAREREdG7wKLcjNy4cQPx8fHo3LkznJyc4OfnB4VCgZCQEJP14ejoiLS0NDx9+tRkxywICwsL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R44cwa5du3D79m2Ym5vjpZdeQkhICL788ks0bdq0VvERERERVUWUn59v+Ec5Ej2HPp72AwoKi4QOgx6jVCpQXCyHpaUFV4wwYsyT8WOOjJ8+OZodEoC2rzg/mcBIJ1xolIiIiIhIYCzKiYiIiIgExqKciIiIiEhgLMqJiIiIiATGopyIiIiISGAsyomIiIiIBMYlEYkM5O8Ll6FQKIUOgx6jVCpQVFQMKytLLuNmxJgn48ccGT99cmTbyBpN7WyeUGSkCxblRPRMk8vlyM7OhqOjY42fVEt1j3kyfsyR8WOOnm6cvkJEREREJDAW5UREREREAmNRTkREREQkMBblREREREQCY1FORERERCQwrr5CZCBcEtE4cRm3pwPzZPyYI+P3eI647OHTxVToAIieFUvWxqOgsEjoMOgxSqUCxcVyWFpasJAwYsyT8WOOjN/jOZodEsCi/CnC6StERERERAJjUU5EREREJDAW5UREREREAmNRTkREREQkMBblREREREQCY1FORERERCQwFuVERERERAJjUf4EnTlzBmPGjEGHDh3g4OCApk2bon379vj000+xf/9+rX3kcjlWr14NLy8vuLi4wM7ODm3atMGIESNw8ODBSo91//59LFmyBD179kTz5s3V/by8vDB37lxkZmYCAEaPHg2JRKLzV2RkpMZxBg0aBIlEgi5dutToNdF2/BdffBG9evXC8uXLUVJSUqFPVlYWJBIJhg4dqnXMsrIyyGQyDB8+HK1atUKTJk3g5OSEt99+G/Pnz8fly5crjSc6Olodx6lTp2p0TkRERET64sODngClUolZs2YhPDwcpqam6NmzJ7y8vFCvXj1cunQJiYmJiI2NxYwZMzBlyhR1v4yMDPj4+ODChQtwdnbG4MGD0bBhQ3WfhIQEjBgxAmFhYTA1/TeVBQUF8PT0xJ9//glXV1f4+PjAxsYGubm5+O2337Bs2TK4uLjAxcUFAwYMgJOTk0a8KSkpOHLkCPr37w83NzeNfY/++9KlS0hJSYFIJMLff/+NkydPolOnTjV6jYKDg+Hg4IDy8nLcuHEDv/76K+bMmYNDhw4hLi5O53EuX76MgIAAnDt3DnZ2dujduzdefPFF3L9/H7///juWLVuGFStW4OjRo3B1da3QXyqVQiQSoby8HDKZDB06dKjR+RARERHpg0X5EzB//nyEh4fD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82a4u7sLcj7PIkPlSJusrCy8/vrrfHhQLRkqR2lpaejXrx9at26NXbt2qdf+z8nJwdtvv40bN27g+PHjaNGixRM/x2eBofLUuXNnpKen48cff8QHH3yg3q56Cuv58+eRkJCA3r17P9Hzo4pYlBM9Qp9HGo8ePRrR0dFYtWoVAgMD1duVSiWGDx+O5ORkdO7cGd26dUNGRga2b98OJycnJCcnw9bWVojTeybUNkd37tzBG2+8gfz8fLzzzjvo2LFjhWM0bNgQX3zxxRM7p2eNIX6OtGFRbjiGytHMmTOxatUqvPjii/D09MSDBw+wc+dO3Lp1C19//bX6gVxUM4bIU1JSEvz9/VFWVoZevXqhXbt2yM/Px65du3D79m2899576ofekbC4TjnRI3r27Indu3cjNDQUW7ZswYMHD9CmTRvMnTtX/dF5dcRiMaKiorBs2TJs3LgR4eHhaNSoEYKDgzFr1iwW5LVU2xzdu3cP+fn5AIC9e/di7969Fdo4OjqyKK8FQ/wcUd0yVI4WLFiANm3aYO3atYiKioJIJEK7du2wdOlSTi8yAEPkqW/fvkhMTMSPP/6IY8eO4ciRI7CwsECrVq0wZcoUjBo1qo7PgnTFK+VERERERALjjZ5ERERERAJjUU5EREREJDAW5UREREREAmNRTkREREQkMBblREREREQCY1FORERERCQwFuVERERERAJjUU5EREREJDAW5UREJCg3NzdIJBJERkZW2W7AgAGQSCQIDQ3V2H748GFIJBKNL1tbWzg7O6Njx4744IMPEB4ejlu3blU6dlZWlrpvVlaWQc7L0FTnf/jwYaFDIaI6YCp0AERERIbi7+8PACgvL0dBQQGuXr2KXbt2Ydu2bZgzZw7GjRuHqVOnol69egJHSkSkiUU5ERE9M1avXl1hW35+PtasWYPFixcjLCwMGRkZWLduHUQikQAREhFpx+krRET0TJNIJJg8eTKkUilEIhHi4+OxceNGocMiItLAopyIiJ4Lnp6eeP/99wEAP/74Y63H69u3LyQSCeLi4ipt89NPP0EikSAwMFC9raCgAL/88guCgoLQoUMHODg4wMHBAV27dsW3336L/Px8veKobq55aGio1rn4KmfOnMEnn3yCtm3bws7ODs7OzhgyZAgSExP1ioOIaodFORERPTd8fHwAAH/99RdycnJqNZaq0I6K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
"/>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p><strong>As a critical concept explaining the price differences in different countries, PPP is crucial in guiding investment decisions. By comparing it to the exchange rate for every currency, we can determine the potential value of the Canadian dollar. This understanding of PPP significantly enhances the sense of expertise of Starbucks executives, making them feel more knowledgeable and competent in their investment decisions, thereby boosting their confidence.</strong></p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [ ]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-python"><pre><span></span><span class="n">z</span> <span class="o">=</span> <span class="p">(</span><span class="s2">"None"</span><span class="p">)</span> <span class="o">*</span> <span class="n">coffee_table_final</span><span class="o">.</span><span class="n">num_rows</span>

<span class="n">ppp_vs_exg_rate</span> <span class="o">=</span> <span class="n">coffee_table_final</span><span class="o">.</span><span class="n">select</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">2</span><span class="p">,</span> <span class="mi">7</span><span class="p">)</span>
<span class="n">ppp_vs_exg_rate</span> <span class="o">=</span> <span class="n">ppp_vs_exg_rate</span><span class="o">.</span><span class="n">with_column</span><span class="p">(</span><span class="s2">"Exchange Rate"</span><span class="p">,</span> <span class="n">ppp_vs_exg_rate</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="n">getExchangeRateCAD</span><span class="p">,</span> <span class="s1">'Currency Code'</span><span class="p">))</span>
<span class="n">ppp_vs_exg_rate</span> <span class="o">=</span> <span class="n">ppp_vs_exg_rate</span><span class="o">.</span><span class="n">with_column</span><span class="p">(</span><span class="s2">"Invest?"</span><span class="p">,</span> <span class="n">z</span><span class="p">)</span>

<span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="n">ppp_vs_exg_rate</span><span class="o">.</span><span class="n">num_rows</span><span class="p">):</span>
  <span class="k">if</span> <span class="n">ppp_vs_exg_rate</span><span class="o">.</span><span class="n">column</span><span class="p">(</span><span class="s2">"Purchasing Power Parity"</span><span class="p">)[</span><span class="n">i</span><span class="p">]</span> <span class="o">&gt;</span> <span class="n">ppp_vs_exg_rate</span><span class="o">.</span><span class="n">column</span><span class="p">(</span><span class="s2">"Exchange Rate"</span><span class="p">)[</span><span class="n">i</span><span class="p">]:</span>
    <span class="n">ppp_vs_exg_rate</span><span class="p">[</span><span class="s2">"Invest?"</span><span class="p">][</span><span class="n">i</span><span class="p">]</span> <span class="o">=</span> <span class="s2">"Invest"</span>
  <span class="k">else</span><span class="p">:</span>
    <span class="n">ppp_vs_exg_rate</span><span class="p">[</span><span class="s2">"Invest?"</span><span class="p">][</span><span class="n">i</span><span class="p">]</span> <span class="o">=</span> <span class="s2">"Don't Invest"</span>

<span class="n">ppp_vs_exg_rate</span><span class="o">.</span><span class="n">show</span><span class="p">(</span><span class="mi">5</span><span class="p">)</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output" data-mime-type="text/html" tabindex="0">
<table border="1" class="dataframe">
<thead>
<tr>
<th>Country</th> <th>Currency Code</th> <th>Purchasing Power Parity</th> <th>Exchange Rate</th> <th>Invest?</th>
</tr>
</thead>
<tbody>
<tr>
<td>ANDORRA   </td> <td>EUR          </td> <td>0.851948               </td> <td>0.678422     </td> <td>Invest      </td>
</tr>
<tr>
<td>ARGENTINA </td> <td>ARS          </td> <td>1.21299                </td> <td>719.551      </td> <td>Don't Invest</td>
</tr>
<tr>
<td>AUSTRALIA </td> <td>AUD          </td> <td>1.03117                </td> <td>1.0998       </td> <td>Don't Invest</td>
</tr>
<tr>
<td>AUSTRIA   </td> <td>EUR          </td> <td>0.903896               </td> <td>0.678422     </td> <td>Invest      </td>
</tr>
<tr>
<td>AZERBAIJAN</td> <td>AZN          </td> <td>0.885714               </td> <td>1.21044      </td> <td>Don't Invest</td>
</tr>
</tbody>
</table>
<p>... (14 rows omitted)</p>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Now, we will map the countries where it would make sense for us to invest and display it.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [ ]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-python"><pre><span></span><span class="n">invest_map</span> <span class="o">=</span> <span class="n">ppp_vs_exg_rate</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">"Country"</span><span class="p">,</span> <span class="n">ccll</span><span class="p">,</span> <span class="s2">"Country"</span><span class="p">)</span>
<span class="n">invest_map</span> <span class="o">=</span> <span class="n">invest_map</span><span class="o">.</span><span class="n">with_column</span><span class="p">(</span><span class="s2">"color"</span><span class="p">,</span> <span class="n">invest_map</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="n">continent_colour</span><span class="p">,</span> <span class="s2">"Continent"</span><span class="p">))</span>
<span class="n">invest_map</span> <span class="o">=</span> <span class="n">invest_map</span><span class="o">.</span><span class="n">select</span><span class="p">(</span><span class="s2">"Country"</span><span class="p">,</span> <span class="s2">"Invest?"</span><span class="p">,</span> <span class="s2">"Currency Code"</span><span class="p">,</span> <span class="s2">"color"</span><span class="p">,</span> <span class="s2">"Continent"</span><span class="p">,</span> <span class="s2">"Capital"</span><span class="p">,</span> <span class="s2">"Code"</span><span class="p">,</span> <span class="s2">"Longitude"</span><span class="p">,</span> <span class="s2">"Latitude"</span><span class="p">)</span><span class="o">.</span><span class="n">relabel</span><span class="p">(</span><span class="s2">"Invest?"</span><span class="p">,</span> <span class="s2">"labels"</span><span class="p">)</span>

<span class="n">Marker</span><span class="o">.</span><span class="n">map_table</span><span class="p">(</span><span class="n">invest_map</span><span class="o">.</span><span class="n">select</span><span class="p">(</span><span class="s1">'Latitude'</span><span class="p">,</span> <span class="s1">'Longitude'</span><span class="p">,</span> <span class="s1">'labels'</span><span class="p">,</span><span class="s1">'color'</span><span class="p">))</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="application/vnd.jupyter.stderr" tabindex="0">
<pre>/usr/local/lib/python3.10/dist-packages/datascience/maps.py:548: UserWarning: color argument of Icon should be one of: {'orange', 'black', 'darkred', 'lightred', 'blue', 'cadetblue', 'darkpurple', 'lightgray', 'beige', 'darkgreen', 'red', 'white', 'purple', 'gray', 'lightgreen', 'pink', 'darkblue', 'green', 'lightblue'}.
  attrs['icon'] = folium.Icon(**icon_args)
</pre>
</div>
</div>
<div class="jp-OutputArea-child jp-OutputArea-executeResult">
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[ ]:</div>
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html" tabindex="0">
<div style="width:100%;"><div style="position:relative;width:100%;height:0;padding-bottom:60%;"><span style="color:#565656">Make this Notebook Trusted to load map: File -&gt; Trust Notebook</span><iframe allowfullscreen="" mozallowfullscreen="" srcdoc="&lt;!DOCTYPE html&gt;
&lt;html&gt;
&lt;head&gt;
    
    &lt;meta http-equiv=&quot;content-type&quot; content=&quot;text/html; charset=UTF-8&quot; /&gt;
    
        &lt;script&gt;
            L_NO_TOUCH = false;
            L_DISABLE_3D = false;
        &lt;/script&gt;
    
    &lt;style&gt;html, body {width: 100%;height: 100%;margin: 0;padding: 0;}&lt;/style&gt;
    &lt;style&gt;#map {position:absolute;top:0;bottom:0;right:0;left:0;}&lt;/style&gt;
    &lt;script src=&quot;https://cdn.jsdelivr.net/npm/leaflet@1.9.3/dist/leaflet.js&quot;&gt;&lt;/script&gt;
    &lt;script src=&quot;https://code.jquery.com/jquery-3.7.1.min.js&quot;&gt;&lt;/script&gt;
    &lt;script src=&quot;https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/js/bootstrap.bundle.min.js&quot;&gt;&lt;/script&gt;
    &lt;script src=&quot;https://cdnjs.cloudflare.com/ajax/libs/Leaflet.awesome-markers/2.0.2/leaflet.awesome-markers.js&quot;&gt;&lt;/script&gt;
    &lt;link rel=&quot;stylesheet&quot; href=&quot;https://cdn.jsdelivr.net/npm/leaflet@1.9.3/dist/leaflet.css&quot;/&gt;
    &lt;link rel=&quot;stylesheet&quot; href=&quot;https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/css/bootstrap.min.css&quot;/&gt;
    &lt;link rel=&quot;stylesheet&quot; href=&quot;https://netdna.bootstrapcdn.com/bootstrap/3.0.0/css/bootstrap-glyphicons.css&quot;/&gt;
    &lt;link rel=&quot;stylesheet&quot; href=&quot;https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.2.0/css/all.min.css&quot;/&gt;
    &lt;link rel=&quot;stylesheet&quot; href=&quot;https://cdnjs.cloudflare.com/ajax/libs/Leaflet.awesome-markers/2.0.2/leaflet.awesome-markers.css&quot;/&gt;
    &lt;link rel=&quot;stylesheet&quot; href=&quot;https://cdn.jsdelivr.net/gh/python-visualization/folium/folium/templates/leaflet.awesome.rotate.min.css&quot;/&gt;
    
            &lt;meta name=&quot;viewport&quot; content=&quot;width=device-width,
                initial-scale=1.0, maximum-scale=1.0, user-scalable=no&quot; /&gt;
            &lt;style&gt;
                #map_904a7a84203a06b4157578ba03f84fad {
                    position: relative;
                    width: 960.0px;
                    height: 500.0px;
                    left: 0.0%;
                    top: 0.0%;
                }
                .leaflet-container { font-size: 1rem; }
            &lt;/style&gt;
        
&lt;/head&gt;
&lt;body&gt;
    
    
            &lt;div class=&quot;folium-map&quot; id=&quot;map_904a7a84203a06b4157578ba03f84fad&quot; &gt;&lt;/div&gt;
        
&lt;/body&gt;
&lt;script&gt;
    
    
            var map_904a7a84203a06b4157578ba03f84fad = L.map(
                &quot;map_904a7a84203a06b4157578ba03f84fad&quot;,
                {
                    center: [7.783333330000001, 32.525],
                    crs: L.CRS.EPSG3857,
                    zoom: 1,
                    zoomControl: true,
                    preferCanvas: false,
                    clusteredMarker: false,
                    includeColorScaleOutliers: true,
                    radiusInMeters: false,
                }
            );

            

        
    
            var tile_layer_624d264b083da180a90a7c60ed24546a = L.tileLayer(
                &quot;https://tile.openstreetmap.org/{z}/{x}/{y}.png&quot;,
                {&quot;attribution&quot;: &quot;\u0026copy; \u003ca href=\&quot;https://www.openstreetmap.org/copyright\&quot;\u003eOpenStreetMap\u003c/a\u003e contributors&quot;, &quot;detectRetina&quot;: false, &quot;maxNativeZoom&quot;: 19, &quot;maxZoom&quot;: 17, &quot;minZoom&quot;: -1, &quot;noWrap&quot;: false, &quot;opacity&quot;: 1, &quot;subdomains&quot;: &quot;abc&quot;, &quot;tms&quot;: false}
            );
        
    
            tile_layer_624d264b083da180a90a7c60ed24546a.addTo(map_904a7a84203a06b4157578ba03f84fad);
        
    
            var marker_ac9c2036d181e2821d442853017c0fc7 = L.marker(
                [42.5, 1.516667],
                {}
            ).addTo(map_904a7a84203a06b4157578ba03f84fad);
        
    
            var icon_52169f7f68bf43050638ee6ae100af6e = L.AwesomeMarkers.icon(
                {&quot;extraClasses&quot;: &quot;fa-rotate-0&quot;, &quot;icon&quot;: &quot;sign-blank&quot;, &quot;iconColor&quot;: &quot;white&quot;, &quot;markerColor&quot;: &quot;red&quot;, &quot;prefix&quot;: &quot;glyphicon&quot;}
            );
            marker_ac9c2036d181e2821d442853017c0fc7.setIcon(icon_52169f7f68bf43050638ee6ae100af6e);
        
    
        var popup_2b587e0b896f62b93c61d23a267fc168 = L.popup({&quot;maxWidth&quot;: &quot;100%&quot;});

        
            
                var html_9a47bceaa9eaed566eb58dbf91aa3e23 = $(`&lt;div id=&quot;html_9a47bceaa9eaed566eb58dbf91aa3e23&quot; style=&quot;width: 100.0%; height: 100.0%;&quot;&gt;Invest&lt;/div&gt;`)[0];
                popup_2b587e0b896f62b93c61d23a267fc168.setContent(html_9a47bceaa9eaed566eb58dbf91aa3e23);
            
        

        marker_ac9c2036d181e2821d442853017c0fc7.bindPopup(popup_2b587e0b896f62b93c61d23a267fc168)
        ;

        
    
    
            var marker_96eea7cf528ab603bc73dc6fe775f84d = L.marker(
                [-34.58333333, -58.666667],
                {}
            ).addTo(map_904a7a84203a06b4157578ba03f84fad);
        
    
            var icon_7c953e92d5dc84753190eb2fddf438bc = L.AwesomeMarkers.icon(
                {&quot;extraClasses&quot;: &quot;fa-rotate-0&quot;, &quot;icon&quot;: &quot;sign-blank&quot;, &quot;iconColor&quot;: &quot;white&quot;, &quot;markerColor&quot;: &quot;orange&quot;, &quot;prefix&quot;: &quot;glyphicon&quot;}
            );
            marker_96eea7cf528ab603bc73dc6fe775f84d.setIcon(icon_7c953e92d5dc84753190eb2fddf438bc);
        
    
        var popup_acde5935e0a4ed38e84a2db8e20eeccf = L.popup({&quot;maxWidth&quot;: &quot;100%&quot;});

        
            
                var html_10c86492cdd597faa81a672847959c50 = $(`&lt;div id=&quot;html_10c86492cdd597faa81a672847959c50&quot; style=&quot;width: 100.0%; height: 100.0%;&quot;&gt;Don't Invest&lt;/div&gt;`)[0];
                popup_acde5935e0a4ed38e84a2db8e20eeccf.setContent(html_10c86492cdd597faa81a672847959c50);
            
        

        marker_96eea7cf528ab603bc73dc6fe775f84d.bindPopup(popup_acde5935e0a4ed38e84a2db8e20eeccf)
        ;

        
    
    
            var marker_4702984e030d5f7289fb989f49221e52 = L.marker(
                [-35.26666667, 149.133333],
                {}
            ).addTo(map_904a7a84203a06b4157578ba03f84fad);
        
    
            var icon_62fe2250ec70521090380aae02f6cc8b = L.AwesomeMarkers.icon(
                {&quot;extraClasses&quot;: &quot;fa-rotate-0&quot;, &quot;icon&quot;: &quot;sign-blank&quot;, &quot;iconColor&quot;: &quot;white&quot;, &quot;markerColor&quot;: &quot;black&quot;, &quot;prefix&quot;: &quot;glyphicon&quot;}
            );
            marker_4702984e030d5f7289fb989f49221e52.setIcon(icon_62fe2250ec70521090380aae02f6cc8b);
        
    
        var popup_6aa1b7e924a018efedba7b92cc4350f1 = L.popup({&quot;maxWidth&quot;: &quot;100%&quot;});

        
            
                var html_6078a1e10df2345e24d9d83599c983fe = $(`&lt;div id=&quot;html_6078a1e10df2345e24d9d83599c983fe&quot; style=&quot;width: 100.0%; height: 100.0%;&quot;&gt;Don't Invest&lt;/div&gt;`)[0];
                popup_6aa1b7e924a018efedba7b92cc4350f1.setContent(html_6078a1e10df2345e24d9d83599c983fe);
            
        

        marker_4702984e030d5f7289fb989f49221e52.bindPopup(popup_6aa1b7e924a018efedba7b92cc4350f1)
        ;

        
    
    
            var marker_b2ee24f590950b032936f1e738b5ae4f = L.marker(
                [48.2, 16.366667],
                {}
            ).addTo(map_904a7a84203a06b4157578ba03f84fad);
        
    
            var icon_7b0886a692ccc69570ed8e11a91a97e7 = L.AwesomeMarkers.icon(
                {&quot;extraClasses&quot;: &quot;fa-rotate-0&quot;, &quot;icon&quot;: &quot;sign-blank&quot;, &quot;iconColor&quot;: &quot;white&quot;, &quot;markerColor&quot;: &quot;red&quot;, &quot;prefix&quot;: &quot;glyphicon&quot;}
            );
            marker_b2ee24f590950b032936f1e738b5ae4f.setIcon(icon_7b0886a692ccc69570ed8e11a91a97e7);
        
    
        var popup_1aaeff2ea520063c2db609e687221b30 = L.popup({&quot;maxWidth&quot;: &quot;100%&quot;});

        
            
                var html_eb18ca0798c57367df3a4c2c7a2ebb85 = $(`&lt;div id=&quot;html_eb18ca0798c57367df3a4c2c7a2ebb85&quot; style=&quot;width: 100.0%; height: 100.0%;&quot;&gt;Invest&lt;/div&gt;`)[0];
                popup_1aaeff2ea520063c2db609e687221b30.setContent(html_eb18ca0798c57367df3a4c2c7a2ebb85);
            
        

        marker_b2ee24f590950b032936f1e738b5ae4f.bindPopup(popup_1aaeff2ea520063c2db609e687221b30)
        ;

        
    
    
            var marker_07455e9113812e4480bffefe70386965 = L.marker(
                [40.38333333, 49.866667],
                {}
            ).addTo(map_904a7a84203a06b4157578ba03f84fad);
        
    
            var icon_fcffa644dc6d4c34e3dea4e16711ee8a = L.AwesomeMarkers.icon(
                {&quot;extraClasses&quot;: &quot;fa-rotate-0&quot;, &quot;icon&quot;: &quot;sign-blank&quot;, &quot;iconColor&quot;: &quot;white&quot;, &quot;markerColor&quot;: &quot;red&quot;, &quot;prefix&quot;: &quot;glyphicon&quot;}
            );
            marker_07455e9113812e4480bffefe70386965.setIcon(icon_fcffa644dc6d4c34e3dea4e16711ee8a);
        
    
        var popup_f14ad88cd29bff5f7851018241bbc084 = L.popup({&quot;maxWidth&quot;: &quot;100%&quot;});

        
            
                var html_5c741aafb7b02c7325c91b2609132497 = $(`&lt;div id=&quot;html_5c741aafb7b02c7325c91b2609132497&quot; style=&quot;width: 100.0%; height: 100.0%;&quot;&gt;Don't Invest&lt;/div&gt;`)[0];
                popup_f14ad88cd29bff5f7851018241bbc084.setContent(html_5c741aafb7b02c7325c91b2609132497);
            
        

        marker_07455e9113812e4480bffefe70386965.bindPopup(popup_f14ad88cd29bff5f7851018241bbc084)
        ;

        
    
    
            var marker_5857f181841c15c00ac7b613ec82ab82 = L.marker(
                [25.08333333, -77.35],
                {}
            ).addTo(map_904a7a84203a06b4157578ba03f84fad);
        
    
            var icon_84c1fe0a33f10f5ba916761fa23ab4c1 = L.AwesomeMarkers.icon(
                {&quot;extraClasses&quot;: &quot;fa-rotate-0&quot;, &quot;icon&quot;: &quot;sign-blank&quot;, &quot;iconColor&quot;: &quot;white&quot;, &quot;markerColor&quot;: &quot;grey&quot;, &quot;prefix&quot;: &quot;glyphicon&quot;}
            );
            marker_5857f181841c15c00ac7b613ec82ab82.setIcon(icon_84c1fe0a33f10f5ba916761fa23ab4c1);
        
    
        var popup_9c737896244926561a163716ad5a58fc = L.popup({&quot;maxWidth&quot;: &quot;100%&quot;});

        
            
                var html_7fe0bbdc1233daa1dd248977745ec824 = $(`&lt;div id=&quot;html_7fe0bbdc1233daa1dd248977745ec824&quot; style=&quot;width: 100.0%; height: 100.0%;&quot;&gt;Invest&lt;/div&gt;`)[0];
                popup_9c737896244926561a163716ad5a58fc.setContent(html_7fe0bbdc1233daa1dd248977745ec824);
            
        

        marker_5857f181841c15c00ac7b613ec82ab82.bindPopup(popup_9c737896244926561a163716ad5a58fc)
        ;

        
    
    
            var marker_35deed178e88145055b231fd064cee56 = L.marker(
                [26.23333333, 50.566667],
                {}
            ).addTo(map_904a7a84203a06b4157578ba03f84fad);
        
    
            var icon_de93d365675ada405be59468fcf0886a = L.AwesomeMarkers.icon(
                {&quot;extraClasses&quot;: &quot;fa-rotate-0&quot;, &quot;icon&quot;: &quot;sign-blank&quot;, &quot;iconColor&quot;: &quot;white&quot;, &quot;markerColor&quot;: &quot;green&quot;, &quot;prefix&quot;: &quot;glyphicon&quot;}
            );
            marker_35deed178e88145055b231fd064cee56.setIcon(icon_de93d365675ada405be59468fcf0886a);
        
    
        var popup_9fa2b60db1681098afecd3326e28fec8 = L.popup({&quot;maxWidth&quot;: &quot;100%&quot;});

        
            
                var html_8f21d74f7efbc8937f3ba1c7bc559c3a = $(`&lt;div id=&quot;html_8f21d74f7efbc8937f3ba1c7bc559c3a&quot; style=&quot;width: 100.0%; height: 100.0%;&quot;&gt;Invest&lt;/div&gt;`)[0];
                popup_9fa2b60db1681098afecd3326e28fec8.setContent(html_8f21d74f7efbc8937f3ba1c7bc559c3a);
            
        

        marker_35deed178e88145055b231fd064cee56.bindPopup(popup_9fa2b60db1681098afecd3326e28fec8)
        ;

        
    
    
            var marker_475085ec7d1380d358ddcaa854bc6f75 = L.marker(
                [50.83333333, 4.333333],
                {}
            ).addTo(map_904a7a84203a06b4157578ba03f84fad);
        
    
            var icon_18a21c7fb99e23bdcb56db460353f454 = L.AwesomeMarkers.icon(
                {&quot;extraClasses&quot;: &quot;fa-rotate-0&quot;, &quot;icon&quot;: &quot;sign-blank&quot;, &quot;iconColor&quot;: &quot;white&quot;, &quot;markerColor&quot;: &quot;red&quot;, &quot;prefix&quot;: &quot;glyphicon&quot;}
            );
            marker_475085ec7d1380d358ddcaa854bc6f75.setIcon(icon_18a21c7fb99e23bdcb56db460353f454);
        
    
        var popup_4ba2e327bd28c2f3c54d1cc4771be77f = L.popup({&quot;maxWidth&quot;: &quot;100%&quot;});

        
            
                var html_d3a3e38bbb00ef023bafdc7e00afbca1 = $(`&lt;div id=&quot;html_d3a3e38bbb00ef023bafdc7e00afbca1&quot; style=&quot;width: 100.0%; height: 100.0%;&quot;&gt;Invest&lt;/div&gt;`)[0];
                popup_4ba2e327bd28c2f3c54d1cc4771be77f.setContent(html_d3a3e38bbb00ef023bafdc7e00afbca1);
            
        

        marker_475085ec7d1380d358ddcaa854bc6f75.bindPopup(popup_4ba2e327bd28c2f3c54d1cc4771be77f)
        ;

        
    
    
            var marker_0067b0f61176aa3970354a4e1188fb55 = L.marker(
                [-16.5, -68.15],
                {}
            ).addTo(map_904a7a84203a06b4157578ba03f84fad);
        
    
            var icon_615cf9142c31e8b9c64bcae12c53d3cf = L.AwesomeMarkers.icon(
                {&quot;extraClasses&quot;: &quot;fa-rotate-0&quot;, &quot;icon&quot;: &quot;sign-blank&quot;, &quot;iconColor&quot;: &quot;white&quot;, &quot;markerColor&quot;: &quot;orange&quot;, &quot;prefix&quot;: &quot;glyphicon&quot;}
            );
            marker_0067b0f61176aa3970354a4e1188fb55.setIcon(icon_615cf9142c31e8b9c64bcae12c53d3cf);
        
    
        var popup_6a196ce5d394f3b72b3b8b20f366a873 = L.popup({&quot;maxWidth&quot;: &quot;100%&quot;});

        
            
                var html_e4983a2162fe110f047aadff904ec4d3 = $(`&lt;div id=&quot;html_e4983a2162fe110f047aadff904ec4d3&quot; style=&quot;width: 100.0%; height: 100.0%;&quot;&gt;Don't Invest&lt;/div&gt;`)[0];
                popup_6a196ce5d394f3b72b3b8b20f366a873.setContent(html_e4983a2162fe110f047aadff904ec4d3);
            
        

        marker_0067b0f61176aa3970354a4e1188fb55.bindPopup(popup_6a196ce5d394f3b72b3b8b20f366a873)
        ;

        
    
    
            var marker_f96a7006750c7e56d83a3dd1096c7494 = L.marker(
                [-15.78333333, -47.916667],
                {}
            ).addTo(map_904a7a84203a06b4157578ba03f84fad);
        
    
            var icon_de0322b0869a539eef235406142670a5 = L.AwesomeMarkers.icon(
                {&quot;extraClasses&quot;: &quot;fa-rotate-0&quot;, &quot;icon&quot;: &quot;sign-blank&quot;, &quot;iconColor&quot;: &quot;white&quot;, &quot;markerColor&quot;: &quot;orange&quot;, &quot;prefix&quot;: &quot;glyphicon&quot;}
            );
            marker_f96a7006750c7e56d83a3dd1096c7494.setIcon(icon_de0322b0869a539eef235406142670a5);
        
    
        var popup_21ce6e0cfad9103b9b96f174beef0cfe = L.popup({&quot;maxWidth&quot;: &quot;100%&quot;});

        
            
                var html_03725b6c05cb2b017a49a44eb30ab057 = $(`&lt;div id=&quot;html_03725b6c05cb2b017a49a44eb30ab057&quot; style=&quot;width: 100.0%; height: 100.0%;&quot;&gt;Don't Invest&lt;/div&gt;`)[0];
                popup_21ce6e0cfad9103b9b96f174beef0cfe.setContent(html_03725b6c05cb2b017a49a44eb30ab057);
            
        

        marker_f96a7006750c7e56d83a3dd1096c7494.bindPopup(popup_21ce6e0cfad9103b9b96f174beef0cfe)
        ;

        
    
    
            var marker_89d62b00e1f1692332d2d21c66bedf3c = L.marker(
                [42.68333333, 23.316667],
                {}
            ).addTo(map_904a7a84203a06b4157578ba03f84fad);
        
    
            var icon_9bc1cffaeb20db440e2a71b0c9f19870 = L.AwesomeMarkers.icon(
                {&quot;extraClasses&quot;: &quot;fa-rotate-0&quot;, &quot;icon&quot;: &quot;sign-blank&quot;, &quot;iconColor&quot;: &quot;white&quot;, &quot;markerColor&quot;: &quot;red&quot;, &quot;prefix&quot;: &quot;glyphicon&quot;}
            );
            marker_89d62b00e1f1692332d2d21c66bedf3c.setIcon(icon_9bc1cffaeb20db440e2a71b0c9f19870);
        
    
        var popup_d3110a2bc457c282b5a9d4a631c31e4c = L.popup({&quot;maxWidth&quot;: &quot;100%&quot;});

        
            
                var html_97544fab88274431cb07c2d8aaaffdd6 = $(`&lt;div id=&quot;html_97544fab88274431cb07c2d8aaaffdd6&quot; style=&quot;width: 100.0%; height: 100.0%;&quot;&gt;Don't Invest&lt;/div&gt;`)[0];
                popup_d3110a2bc457c282b5a9d4a631c31e4c.setContent(html_97544fab88274431cb07c2d8aaaffdd6);
            
        

        marker_89d62b00e1f1692332d2d21c66bedf3c.bindPopup(popup_d3110a2bc457c282b5a9d4a631c31e4c)
        ;

        
    
    
            var marker_98918472a66a60f8d18b6fcdb55f8499 = L.marker(
                [11.55, 104.916667],
                {}
            ).addTo(map_904a7a84203a06b4157578ba03f84fad);
        
    
            var icon_559de1bf1036e4ebfce2b6e5d890e56f = L.AwesomeMarkers.icon(
                {&quot;extraClasses&quot;: &quot;fa-rotate-0&quot;, &quot;icon&quot;: &quot;sign-blank&quot;, &quot;iconColor&quot;: &quot;white&quot;, &quot;markerColor&quot;: &quot;green&quot;, &quot;prefix&quot;: &quot;glyphicon&quot;}
            );
            marker_98918472a66a60f8d18b6fcdb55f8499.setIcon(icon_559de1bf1036e4ebfce2b6e5d890e56f);
        
    
        var popup_0e3c3239f8dd59994fbc8bafe9381eb8 = L.popup({&quot;maxWidth&quot;: &quot;100%&quot;});

        
            
                var html_d15ab10db648f09ebe226fe5e4f3648c = $(`&lt;div id=&quot;html_d15ab10db648f09ebe226fe5e4f3648c&quot; style=&quot;width: 100.0%; height: 100.0%;&quot;&gt;Don't Invest&lt;/div&gt;`)[0];
                popup_0e3c3239f8dd59994fbc8bafe9381eb8.setContent(html_d15ab10db648f09ebe226fe5e4f3648c);
            
        

        marker_98918472a66a60f8d18b6fcdb55f8499.bindPopup(popup_0e3c3239f8dd59994fbc8bafe9381eb8)
        ;

        
    
    
            var marker_c08533c673528dc1026935e05329c2be = L.marker(
                [45.41666667, -75.7],
                {}
            ).addTo(map_904a7a84203a06b4157578ba03f84fad);
        
    
            var icon_3d2bb0b016583a0d13192d14cb341cb2 = L.AwesomeMarkers.icon(
                {&quot;extraClasses&quot;: &quot;fa-rotate-0&quot;, &quot;icon&quot;: &quot;sign-blank&quot;, &quot;iconColor&quot;: &quot;white&quot;, &quot;markerColor&quot;: &quot;black&quot;, &quot;prefix&quot;: &quot;glyphicon&quot;}
            );
            marker_c08533c673528dc1026935e05329c2be.setIcon(icon_3d2bb0b016583a0d13192d14cb341cb2);
        
    
        var popup_b10152c3b8bcbd16efec1aae72f90d75 = L.popup({&quot;maxWidth&quot;: &quot;100%&quot;});

        
            
                var html_dd0c2c03f3a8098e85b7ff8405ad46e3 = $(`&lt;div id=&quot;html_dd0c2c03f3a8098e85b7ff8405ad46e3&quot; style=&quot;width: 100.0%; height: 100.0%;&quot;&gt;Don't Invest&lt;/div&gt;`)[0];
                popup_b10152c3b8bcbd16efec1aae72f90d75.setContent(html_dd0c2c03f3a8098e85b7ff8405ad46e3);
            
        

        marker_c08533c673528dc1026935e05329c2be.bindPopup(popup_b10152c3b8bcbd16efec1aae72f90d75)
        ;

        
    
    
            var marker_359742ee0dc88d8c7da65ab35376e28f = L.marker(
                [-33.45, -70.666667],
                {}
            ).addTo(map_904a7a84203a06b4157578ba03f84fad);
        
    
            var icon_207d55874c5a8d3a8cd2030a4a1de5a7 = L.AwesomeMarkers.icon(
                {&quot;extraClasses&quot;: &quot;fa-rotate-0&quot;, &quot;icon&quot;: &quot;sign-blank&quot;, &quot;iconColor&quot;: &quot;white&quot;, &quot;markerColor&quot;: &quot;orange&quot;, &quot;prefix&quot;: &quot;glyphicon&quot;}
            );
            marker_359742ee0dc88d8c7da65ab35376e28f.setIcon(icon_207d55874c5a8d3a8cd2030a4a1de5a7);
        
    
        var popup_63092aff9d453f3d2d4ecb598e1253b9 = L.popup({&quot;maxWidth&quot;: &quot;100%&quot;});

        
            
                var html_6835a8b47f92cc129a58312c6b131453 = $(`&lt;div id=&quot;html_6835a8b47f92cc129a58312c6b131453&quot; style=&quot;width: 100.0%; height: 100.0%;&quot;&gt;Don't Invest&lt;/div&gt;`)[0];
                popup_63092aff9d453f3d2d4ecb598e1253b9.setContent(html_6835a8b47f92cc129a58312c6b131453);
            
        

        marker_359742ee0dc88d8c7da65ab35376e28f.bindPopup(popup_63092aff9d453f3d2d4ecb598e1253b9)
        ;

        
    
    
            var marker_a401361744b43c8b5d77a83c99afb111 = L.marker(
                [39.91666667, 116.383333],
                {}
            ).addTo(map_904a7a84203a06b4157578ba03f84fad);
        
    
            var icon_27f967eb2c23167fb6a962938d211456 = L.AwesomeMarkers.icon(
                {&quot;extraClasses&quot;: &quot;fa-rotate-0&quot;, &quot;icon&quot;: &quot;sign-blank&quot;, &quot;iconColor&quot;: &quot;white&quot;, &quot;markerColor&quot;: &quot;green&quot;, &quot;prefix&quot;: &quot;glyphicon&quot;}
            );
            marker_a401361744b43c8b5d77a83c99afb111.setIcon(icon_27f967eb2c23167fb6a962938d211456);
        
    
        var popup_0ca69d6b4d1c47912877a300adf4bd5a = L.popup({&quot;maxWidth&quot;: &quot;100%&quot;});

        
            
                var html_97d2838168bdfdc0e8617fb9001e42f5 = $(`&lt;div id=&quot;html_97d2838168bdfdc0e8617fb9001e42f5&quot; style=&quot;width: 100.0%; height: 100.0%;&quot;&gt;Don't Invest&lt;/div&gt;`)[0];
                popup_0ca69d6b4d1c47912877a300adf4bd5a.setContent(html_97d2838168bdfdc0e8617fb9001e42f5);
            
        

        marker_a401361744b43c8b5d77a83c99afb111.bindPopup(popup_0ca69d6b4d1c47912877a300adf4bd5a)
        ;

        
    
    
            var marker_b42c4d67b4e3da18edf5d733400c1cb4 = L.marker(
                [4.6, -74.083333],
                {}
            ).addTo(map_904a7a84203a06b4157578ba03f84fad);
        
    
            var icon_750923649e52cfa77c1a54461985b155 = L.AwesomeMarkers.icon(
                {&quot;extraClasses&quot;: &quot;fa-rotate-0&quot;, &quot;icon&quot;: &quot;sign-blank&quot;, &quot;iconColor&quot;: &quot;white&quot;, &quot;markerColor&quot;: &quot;orange&quot;, &quot;prefix&quot;: &quot;glyphicon&quot;}
            );
            marker_b42c4d67b4e3da18edf5d733400c1cb4.setIcon(icon_750923649e52cfa77c1a54461985b155);
        
    
        var popup_7a7075056d020821d51e1c5d83c6283f = L.popup({&quot;maxWidth&quot;: &quot;100%&quot;});

        
            
                var html_74c04e953b1608a3fda0b2053aab64b4 = $(`&lt;div id=&quot;html_74c04e953b1608a3fda0b2053aab64b4&quot; style=&quot;width: 100.0%; height: 100.0%;&quot;&gt;Don't Invest&lt;/div&gt;`)[0];
                popup_7a7075056d020821d51e1c5d83c6283f.setContent(html_74c04e953b1608a3fda0b2053aab64b4);
            
        

        marker_b42c4d67b4e3da18edf5d733400c1cb4.bindPopup(popup_7a7075056d020821d51e1c5d83c6283f)
        ;

        
    
    
            var marker_feeeb46f51164d9cf1d8465008460e6e = L.marker(
                [9.933333333, -84.083333],
                {}
            ).addTo(map_904a7a84203a06b4157578ba03f84fad);
        
    
            var icon_224a7e05dc0ff0f67798161bec850dc8 = L.AwesomeMarkers.icon(
                {&quot;extraClasses&quot;: &quot;fa-rotate-0&quot;, &quot;icon&quot;: &quot;sign-blank&quot;, &quot;iconColor&quot;: &quot;white&quot;, &quot;markerColor&quot;: &quot;black&quot;, &quot;prefix&quot;: &quot;glyphicon&quot;}
            );
            marker_feeeb46f51164d9cf1d8465008460e6e.setIcon(icon_224a7e05dc0ff0f67798161bec850dc8);
        
    
        var popup_6ed896cae31d560978ec43310c70fb55 = L.popup({&quot;maxWidth&quot;: &quot;100%&quot;});

        
            
                var html_5cd812d1d04497e39eaa48d08eba67c2 = $(`&lt;div id=&quot;html_5cd812d1d04497e39eaa48d08eba67c2&quot; style=&quot;width: 100.0%; height: 100.0%;&quot;&gt;Don't Invest&lt;/div&gt;`)[0];
                popup_6ed896cae31d560978ec43310c70fb55.setContent(html_5cd812d1d04497e39eaa48d08eba67c2);
            
        

        marker_feeeb46f51164d9cf1d8465008460e6e.bindPopup(popup_6ed896cae31d560978ec43310c70fb55)
        ;

        
    
    
            var marker_266596810e7284e5f90ea9e3c4dedceb = L.marker(
                [35.16666667, 33.366667],
                {}
            ).addTo(map_904a7a84203a06b4157578ba03f84fad);
        
    
            var icon_0a9c2dbd46ff80d8d64d8664a1e14fa2 = L.AwesomeMarkers.icon(
                {&quot;extraClasses&quot;: &quot;fa-rotate-0&quot;, &quot;icon&quot;: &quot;sign-blank&quot;, &quot;iconColor&quot;: &quot;white&quot;, &quot;markerColor&quot;: &quot;red&quot;, &quot;prefix&quot;: &quot;glyphicon&quot;}
            );
            marker_266596810e7284e5f90ea9e3c4dedceb.setIcon(icon_0a9c2dbd46ff80d8d64d8664a1e14fa2);
        
    
        var popup_06f7952ad9e8169ca042d78fdf810b40 = L.popup({&quot;maxWidth&quot;: &quot;100%&quot;});

        
            
                var html_4b1a680a78b796a34ecc4509b263ea4c = $(`&lt;div id=&quot;html_4b1a680a78b796a34ecc4509b263ea4c&quot; style=&quot;width: 100.0%; height: 100.0%;&quot;&gt;Invest&lt;/div&gt;`)[0];
                popup_06f7952ad9e8169ca042d78fdf810b40.setContent(html_4b1a680a78b796a34ecc4509b263ea4c);
            
        

        marker_266596810e7284e5f90ea9e3c4dedceb.bindPopup(popup_06f7952ad9e8169ca042d78fdf810b40)
        ;

        
    
    
            var marker_760d0d765626f6871ae88f32ba2519e0 = L.marker(
                [50.08333333, 14.466667],
                {}
            ).addTo(map_904a7a84203a06b4157578ba03f84fad);
        
    
            var icon_c30de75672c0220abc715fa878c266a4 = L.AwesomeMarkers.icon(
                {&quot;extraClasses&quot;: &quot;fa-rotate-0&quot;, &quot;icon&quot;: &quot;sign-blank&quot;, &quot;iconColor&quot;: &quot;white&quot;, &quot;markerColor&quot;: &quot;red&quot;, &quot;prefix&quot;: &quot;glyphicon&quot;}
            );
            marker_760d0d765626f6871ae88f32ba2519e0.setIcon(icon_c30de75672c0220abc715fa878c266a4);
        
    
        var popup_4ecf1ae1758610369bf80b7799f93851 = L.popup({&quot;maxWidth&quot;: &quot;100%&quot;});

        
            
                var html_000aa542e90cde66fbe9c4eac156448f = $(`&lt;div id=&quot;html_000aa542e90cde66fbe9c4eac156448f&quot; style=&quot;width: 100.0%; height: 100.0%;&quot;&gt;Don't Invest&lt;/div&gt;`)[0];
                popup_4ecf1ae1758610369bf80b7799f93851.setContent(html_000aa542e90cde66fbe9c4eac156448f);
            
        

        marker_760d0d765626f6871ae88f32ba2519e0.bindPopup(popup_4ecf1ae1758610369bf80b7799f93851)
        ;

        
    
&lt;/script&gt;
&lt;/html&gt;" style="position:absolute;width:100%;height:100%;left:0;top:0;border:none !important;" webkitallowfullscreen=""></iframe></div></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>In conclusion, Starbucks executives should consider the promising potential of investing in countries with higher PPP than exchange rates. These countries, with their lower price levels than the currency you can exchange in the bank, offer a unique opportunity. Selling coffee in these countries can yield higher returns when you convert your earnings back into Canadian dollars after the currency appreciates, presenting a hopeful outlook for your investment strategy.
However, it's crucial to exercise caution. While countries with higher PPP than exchange rates may seem attractive for investment, other factors could be at play. High inflation rates or political instability, for instance, could significantly impact the value of your investments. Considering these risks before making investment decisions and fostering a sense of prudence and responsibility in your investment approach is essential.</p>
<p>For consumers, the prospect of visiting countries with higher PPP than exchange rates is indeed exciting. Your dollar can stretch further in these countries, allowing you to purchase more goods than in countries with a lower PPP than the exchange rate. However, it's crucial to be mindful of potential political instability when planning your visit, as this could impact your travel experience.</p>
<p>Ultimately, if you are a Starbucks lattes fan looking to maximize its consumption or minimize its cost, use our maps as a guide to get more of it! Similarly, our map could guide you to the right investment location if you are a Starbucks executive looking to maximize the company's ROI, instilling a sense of guidance and confidence in your decision-making process.</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p><strong>References</strong><br/>
Aisen, A., &amp; Veiga, F. J., (2013). How does political instability affect economic growth?. <em>European Journal of Political Economy</em>, 29, 151-167.
Klugman J., Rodríguez F., Choi HJ., (2011, January). Human development index, <em>World Health Organization</em>, <a href="https://www.who.int/data/nutrition/nlis/info/human-development-index#:~:text=The%20HDI%20is%20a%20summary,knowledge%20and%20standard%20of%20living">https://www.who.int/data/nutrition/nlis/info/human-development-index#:~:text=The%20HDI%20is%20a%20summary,knowledge%20and%20standard%20of%20living</a>.<br/>
United Nations Development Programme. (2020). <em>Human Development Report 2019 – Technical notes.</em> <a href="https://web.archive.org/web/20210606201849/http://hdr.undp.org/sites/default/files/hdr2020_technical_notes.pdf">https://web.archive.org/web/20210606201849/http://hdr.undp.org/sites/default/files/hdr2020_technical_notes.pdf</a>.</p>
<p><a href="https://www.cashnetusa.com/blog/starbucks-price-every-country/">https://www.cashnetusa.com/blog/starbucks-price-every-country/</a>
<a href="https://en.wikipedia.org/wiki/Value-added_tax#Around_the_world">https://en.wikipedia.org/wiki/Value-added_tax#Around_the_world</a>
<a href="https://public.opendatasoft.com/explore/dataset/currency-codes/table/">https://public.opendatasoft.com/explore/dataset/currency-codes/table/</a>
<a href="https://unstats.un.org/unsd/snaama/Basic">https://unstats.un.org/unsd/snaama/Basic</a>
<a href="https://en.wikipedia.org/w/index.php?title=Gross_domestic_product&amp;useskin=vector#GDP_per_capita">https://en.wikipedia.org/w/index.php?title=Gross_domestic_product&amp;useskin=vector#GDP_per_capita</a></p>
</div>
</div>
</div>
</div>
</main>
</body>
</html>
