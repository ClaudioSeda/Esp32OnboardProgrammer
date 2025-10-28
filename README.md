# Esp32OnboardProgrammer
You dont need to place serial to usb converters onboard! 
An easy way to upload you binaries to wroom modules.
Simply plug the programmer in your board and upload your binaries.
Cool way to produce you esp32 boards!
here follows the schematics picture:

<img width="904" height="630" alt="image" src="https://github.com/user-attachments/assets/36d6b947-79f1-43b9-b3c0-da293d45aa82" />

the iBOM follows below:

<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Interactive BOM for KiCAD</title>
  <style type="text/css">
:root {
  --pcb-edge-color: black;
  --pad-color: #878787;
  --pad-hole-color: #CCCCCC;
  --pad-color-highlight: #D04040;
  --pad-color-highlight-both: #D0D040;
  --pad-color-highlight-marked: #44a344;
  --pin1-outline-color: #ffb629;
  --pin1-outline-color-highlight: #ffb629;
  --pin1-outline-color-highlight-both: #fcbb39;
  --pin1-outline-color-highlight-marked: #fdbe41;
  --silkscreen-edge-color: #aa4;
  --silkscreen-polygon-color: #4aa;
  --silkscreen-text-color: #4aa;
  --fabrication-edge-color: #907651;
  --fabrication-polygon-color: #907651;
  --fabrication-text-color: #a27c24;
  --track-color: #def5f1;
  --track-color-highlight: #D04040;
  --zone-color: #def5f1;
  --zone-color-highlight: #d0404080;
}

html,
body {
  margin: 0px;
  height: 100%;
  font-family: Verdana, sans-serif;
}

.dark.topmostdiv {
  --pcb-edge-color: #eee;
  --pad-color: #808080;
  --pin1-outline-color: #ffa800;
  --pin1-outline-color-highlight: #ccff00;
  --track-color: #42524f;
  --zone-color: #42524f;
  background-color: #252c30;
  color: #eee;
}

button {
  background-color: #eee;
  border: 1px solid #888;
  color: black;
  height: 44px;
  width: 44px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 14px;
  font-weight: bolder;
}

.dark button {
  /* This will be inverted */
  background-color: #c3b7b5;
}

button.depressed {
  background-color: #0a0;
  color: white;
}

.dark button.depressed {
  /* This will be inverted */
  background-color: #b3b;
}

button:focus {
  outline: 0;
}

button#tb-btn {
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 8.47 8.47'%3E%3Crect transform='translate(0 -288.53)' ry='1.17' y='288.8' x='.27' height='7.94' width='7.94' fill='%23f9f9f9'/%3E%3Cg transform='translate(0 -288.53)'%3E%3Crect width='7.94' height='7.94' x='.27' y='288.8' ry='1.17' fill='none' stroke='%23000' stroke-width='.4' stroke-linejoin='round'/%3E%3Cpath d='M1.32 290.12h5.82M1.32 291.45h5.82' fill='none' stroke='%23000' stroke-width='.4'/%3E%3Cpath d='M4.37 292.5v4.23M.26 292.63H8.2' fill='none' stroke='%23000' stroke-width='.3'/%3E%3Ctext font-weight='700' font-size='3.17' font-family='sans-serif'%3E%3Ctspan x='1.35' y='295.73'%3EF%3C/tspan%3E%3Ctspan x='5.03' y='295.68'%3EB%3C/tspan%3E%3C/text%3E%3C/g%3E%3C/svg%3E%0A");
}

button#lr-btn {
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 8.47 8.47'%3E%3Crect transform='translate(0 -288.53)' ry='1.17' y='288.8' x='.27' height='7.94' width='7.94' fill='%23f9f9f9'/%3E%3Cg transform='translate(0 -288.53)'%3E%3Crect width='7.94' height='7.94' x='.27' y='288.8' ry='1.17' fill='none' stroke='%23000' stroke-width='.4' stroke-linejoin='round'/%3E%3Cpath d='M1.06 290.12H3.7m-2.64 1.33H3.7m-2.64 1.32H3.7m-2.64 1.3H3.7m-2.64 1.33H3.7' fill='none' stroke='%23000' stroke-width='.4'/%3E%3Cpath d='M4.37 288.8v7.94m0-4.11h3.96' fill='none' stroke='%23000' stroke-width='.3'/%3E%3Ctext font-weight='700' font-size='3.17' font-family='sans-serif'%3E%3Ctspan x='5.11' y='291.96'%3EF%3C/tspan%3E%3Ctspan x='5.03' y='295.68'%3EB%3C/tspan%3E%3C/text%3E%3C/g%3E%3C/svg%3E%0A");
}

button#bom-btn {
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 8.47 8.47'%3E%3Crect transform='translate(0 -288.53)' ry='1.17' y='288.8' x='.27' height='7.94' width='7.94' fill='%23f9f9f9'/%3E%3Cg transform='translate(0 -288.53)' fill='none' stroke='%23000' stroke-width='.4'%3E%3Crect width='7.94' height='7.94' x='.27' y='288.8' ry='1.17' stroke-linejoin='round'/%3E%3Cpath d='M1.59 290.12h5.29M1.59 291.45h5.33M1.59 292.75h5.33M1.59 294.09h5.33M1.59 295.41h5.33'/%3E%3C/g%3E%3C/svg%3E");
}

button#bom-grouped-btn {
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='32' height='32'%3E%3Cg stroke='%23000' stroke-linejoin='round' class='layer'%3E%3Crect width='29' height='29' x='1.5' y='1.5' stroke-width='2' fill='%23fff' rx='5' ry='5'/%3E%3Cpath stroke-linecap='square' stroke-width='2' d='M6 10h4m4 0h5m4 0h3M6.1 22h3m3.9 0h5m4 0h4m-16-8h4m4 0h4'/%3E%3Cpath stroke-linecap='null' d='M5 17.5h22M5 26.6h22M5 5.5h22'/%3E%3C/g%3E%3C/svg%3E");
}

button#bom-ungrouped-btn {
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='32' height='32'%3E%3Cg stroke='%23000' stroke-linejoin='round' class='layer'%3E%3Crect width='29' height='29' x='1.5' y='1.5' stroke-width='2' fill='%23fff' rx='5' ry='5'/%3E%3Cpath stroke-linecap='square' stroke-width='2' d='M6 10h4m-4 8h3m-3 8h4'/%3E%3Cpath stroke-linecap='null' d='M5 13.5h22m-22 8h22M5 5.5h22'/%3E%3C/g%3E%3C/svg%3E");
}

button#bom-netlist-btn {
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='32' height='32'%3E%3Cg fill='none' stroke='%23000' class='layer'%3E%3Crect width='29' height='29' x='1.5' y='1.5' stroke-width='2' fill='%23fff' rx='5' ry='5'/%3E%3Cpath stroke-width='2' d='M6 26l6-6v-8m13.8-6.3l-6 6v8'/%3E%3Ccircle cx='11.8' cy='9.5' r='2.8' stroke-width='2'/%3E%3Ccircle cx='19.8' cy='22.8' r='2.8' stroke-width='2'/%3E%3C/g%3E%3C/svg%3E");
}

button#copy {
  background-image: url("data:image/svg+xml,%3Csvg height='48' viewBox='0 0 48 48' width='48' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M0 0h48v48h-48z' fill='none'/%3E%3Cpath d='M32 2h-24c-2.21 0-4 1.79-4 4v28h4v-28h24v-4zm6 8h-22c-2.21 0-4 1.79-4 4v28c0 2.21 1.79 4 4 4h22c2.21 0 4-1.79 4-4v-28c0-2.21-1.79-4-4-4zm0 32h-22v-28h22v28z'/%3E%3C/svg%3E");
  background-position: 6px 6px;
  background-repeat: no-repeat;
  background-size: 26px 26px;
  border-radius: 6px;
  height: 40px;
  width: 40px;
  margin: 10px 5px;
}

button#copy:active {
  box-shadow: inset 0px 0px 5px #6c6c6c;
}

textarea.clipboard-temp {
  position: fixed;
  top: 0;
  left: 0;
  width: 2em;
  height: 2em;
  padding: 0;
  border: None;
  outline: None;
  box-shadow: None;
  background: transparent;
}

.left-most-button {
  border-right: 0;
  border-top-left-radius: 6px;
  border-bottom-left-radius: 6px;
}

.middle-button {
  border-right: 0;
}

.right-most-button {
  border-top-right-radius: 6px;
  border-bottom-right-radius: 6px;
}

.button-container {
  font-size: 0;
  margin: 0.4rem 0.4rem 0.4rem 0;
}

.dark .button-container {
  filter: invert(1);
}

.button-container button {
  background-size: 32px 32px;
  background-position: 5px 5px;
  background-repeat: no-repeat;
}

@media print {
  .hideonprint {
    display: none;
  }
}

canvas {
  cursor: crosshair;
}

canvas:active {
  cursor: grabbing;
}

.fileinfo {
  width: 100%;
  max-width: 1000px;
  border: none;
  padding: 3px;
}

.fileinfo .title {
  font-size: 20pt;
  font-weight: bold;
}

.fileinfo td {
  overflow: hidden;
  white-space: nowrap;
  max-width: 1px;
  width: 50%;
  text-overflow: ellipsis;
}

.bom {
  border-collapse: collapse;
  font-family: Consolas, "DejaVu Sans Mono", Monaco, monospace;
  font-size: 10pt;
  table-layout: fixed;
  width: 100%;
  margin-top: 1px;
  position: relative;
}

.bom th,
.bom td {
  border: 1px solid black;
  padding: 5px;
  word-wrap: break-word;
  text-align: center;
  position: relative;
}

.dark .bom th,
.dark .bom td {
  border: 1px solid #777;
}

.bom th {
  background-color: #CCCCCC;
  background-clip: padding-box;
}

.dark .bom th {
  background-color: #3b4749;
}

.bom tr.highlighted:nth-child(n) {
  background-color: #cfc;
}

.dark .bom tr.highlighted:nth-child(n) {
  background-color: #226022;
}

.bom tr:nth-child(even) {
  background-color: #f2f2f2;
}

.dark .bom tr:nth-child(even) {
  background-color: #313b40;
}

.bom tr.checked {
  color: #1cb53d;
}

.dark .bom tr.checked {
  color: #2cce54;
}

.bom tr {
  transition: background-color 0.2s;
}

.bom .numCol {
  width: 30px;
}

.bom .value {
  width: 15%;
}

.bom .quantity {
  width: 65px;
}

.bom th .sortmark {
  position: absolute;
  right: 1px;
  top: 1px;
  margin-top: -5px;
  border-width: 5px;
  border-style: solid;
  border-color: transparent transparent #221 transparent;
  transform-origin: 50% 85%;
  transition: opacity 0.2s, transform 0.4s;
}

.dark .bom th .sortmark {
  filter: invert(1);
}

.bom th .sortmark.none {
  opacity: 0;
}

.bom th .sortmark.desc {
  transform: rotate(180deg);
}

.bom th:hover .sortmark.none {
  opacity: 0.5;
}

.bom .bom-checkbox {
  width: 30px;
  position: relative;
  user-select: none;
  -moz-user-select: none;
}

.bom .bom-checkbox:before {
  content: "";
  position: absolute;
  border-width: 15px;
  border-style: solid;
  border-color: #51829f transparent transparent transparent;
  visibility: hidden;
  top: -15px;
}

.bom .bom-checkbox:after {
  content: "Double click to set/unset all";
  position: absolute;
  color: white;
  top: -35px;
  left: -26px;
  background: #51829f;
  padding: 5px 15px;
  border-radius: 8px;
  white-space: nowrap;
  visibility: hidden;
}

.bom .bom-checkbox:hover:before,
.bom .bom-checkbox:hover:after {
  visibility: visible;
  transition: visibility 0.2s linear 1s;
}

.split {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
  overflow-y: auto;
  overflow-x: hidden;
  background-color: inherit;
}

.split.split-horizontal,
.gutter.gutter-horizontal {
  height: 100%;
  float: left;
}

.gutter {
  background-color: #ddd;
  background-repeat: no-repeat;
  background-position: 50%;
  transition: background-color 0.3s;
}

.dark .gutter {
  background-color: #777;
}

.gutter.gutter-horizontal {
  background-image: url('data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAUAAAAeCAYAAADkftS9AAAAIklEQVQoU2M4c+bMfxAGAgYYmwGrIIiDjrELjpo5aiZeMwF+yNnOs5KSvgAAAABJRU5ErkJggg==');
  cursor: ew-resize;
  width: 5px;
}

.gutter.gutter-vertical {
  background-image: url('data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAB4AAAAFAQMAAABo7865AAAABlBMVEVHcEzMzMzyAv2sAAAAAXRSTlMAQObYZgAAABBJREFUeF5jOAMEEAIEEFwAn3kMwcB6I2AAAAAASUVORK5CYII=');
  cursor: ns-resize;
  height: 5px;
}

.searchbox {
  float: left;
  height: 40px;
  margin: 10px 5px;
  padding: 12px 32px;
  font-family: Consolas, "DejaVu Sans Mono", Monaco, monospace;
  font-size: 18px;
  box-sizing: border-box;
  border: 1px solid #888;
  border-radius: 6px;
  outline: none;
  background-color: #eee;
  transition: background-color 0.2s, border 0.2s;
  background-image: url('data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAABNklEQVQ4T8XSMUvDQBQH8P/LElFa/AIZHcTBQSz0I/gFstTBRR2KUC4ldDxw7h0Bl3RRUATxi4iiODgoiLNrbQYp5J6cpJJqomkX33Z37/14d/dIa33MzDuYI4johOI4XhyNRteO46zNYjDzAxE1yBZprVeZ+QbAUhXEGJMA2Ox2u4+fQIa0mPmsCgCgJYQ4t7lfgF0opQYAdv9ABkKI/UnOFCClXKjX61cA1osQY8x9kiRNKeV7IWA3oyhaSdP0FkAtjxhj3hzH2RBCPOf3pzqYHCilfAAX+URm9oMguPzeWSGQvUcMYC8rOBJCHBRdqxTo9/vbRHRqi8bj8XKv1xvODbiuW2u32/bvf0SlDv4XYOY7z/Mavu+nM1+BmQ+NMc0wDF/LprP0DbTWW0T00ul0nn4b7Q87+X4Qmfiq2wAAAABJRU5ErkJggg==');
  background-position: 10px 10px;
  background-repeat: no-repeat;
}

.dark .searchbox {
  background-color: #111;
  color: #eee;
}

.searchbox::placeholder {
  color: #ccc;
}

.dark .searchbox::placeholder {
  color: #666;
}

.filter {
  width: calc(60% - 64px);
}

.reflookup {
  width: calc(40% - 10px);
}

input[type=text]:focus {
  background-color: white;
  border: 1px solid #333;
}

.dark input[type=text]:focus {
  background-color: #333;
  border: 1px solid #ccc;
}

mark.highlight {
  background-color: #5050ff;
  color: #fff;
  padding: 2px;
  border-radius: 6px;
}

.dark mark.highlight {
  background-color: #76a6da;
  color: #111;
}

.menubtn {
  background-color: white;
  border: none;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='36' height='36' viewBox='0 0 20 20'%3E%3Cpath fill='none' d='M0 0h20v20H0V0z'/%3E%3Cpath d='M15.95 10.78c.03-.25.05-.51.05-.78s-.02-.53-.06-.78l1.69-1.32c.15-.12.19-.34.1-.51l-1.6-2.77c-.1-.18-.31-.24-.49-.18l-1.99.8c-.42-.32-.86-.58-1.35-.78L12 2.34c-.03-.2-.2-.34-.4-.34H8.4c-.2 0-.36.14-.39.34l-.3 2.12c-.49.2-.94.47-1.35.78l-1.99-.8c-.18-.07-.39 0-.49.18l-1.6 2.77c-.1.18-.06.39.1.51l1.69 1.32c-.04.25-.07.52-.07.78s.02.53.06.78L2.37 12.1c-.15.12-.19.34-.1.51l1.6 2.77c.1.18.31.24.49.18l1.99-.8c.42.32.86.58 1.35.78l.3 2.12c.04.2.2.34.4.34h3.2c.2 0 .37-.14.39-.34l.3-2.12c.49-.2.94-.47 1.35-.78l1.99.8c.18.07.39 0 .49-.18l1.6-2.77c.1-.18.06-.39-.1-.51l-1.67-1.32zM10 13c-1.65 0-3-1.35-3-3s1.35-3 3-3 3 1.35 3 3-1.35 3-3 3z'/%3E%3C/svg%3E%0A");
  background-position: center;
  background-repeat: no-repeat;
}

.statsbtn {
  background-color: white;
  border: none;
  background-image: url("data:image/svg+xml,%3Csvg width='36' height='36' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M4 6h28v24H4V6zm0 8h28v8H4m9-16v24h10V5.8' fill='none' stroke='%23000' stroke-width='2'/%3E%3C/svg%3E");
  background-position: center;
  background-repeat: no-repeat;
}

.iobtn {
  background-color: white;
  border: none;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='36' height='36'%3E%3Cpath fill='none' stroke='%23000' stroke-width='2' d='M3 33v-7l6.8-7h16.5l6.7 7v7H3zM3.2 26H33M21 9l5-5.9 5 6h-2.5V15h-5V9H21zm-4.9 0l-5 6-5-6h2.5V3h5v6h2.5z'/%3E%3Cpath fill='none' stroke='%23000' d='M6.1 29.5H10'/%3E%3C/svg%3E");
  background-position: center;
  background-repeat: no-repeat;
}

.visbtn {
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24'%3E%3Cpath fill='none' stroke='%23333' d='M2.5 4.5h5v15h-5zM9.5 4.5h5v15h-5zM16.5 4.5h5v15h-5z'/%3E%3C/svg%3E");
  background-position: center;
  background-repeat: no-repeat;
  padding: 15px;
}

#vismenu-content {
  left: 0px;
  font-family: Verdana, sans-serif;
}

.dark .statsbtn,
.dark .savebtn,
.dark .menubtn,
.dark .iobtn,
.dark .visbtn {
  filter: invert(1);
}

.flexbox {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 100%;
}

.savebtn {
  background-color: #d6d6d6;
  width: auto;
  height: 30px;
  flex-grow: 1;
  margin: 5px;
  border-radius: 4px;
}

.savebtn:active {
  background-color: #0a0;
  color: white;
}

.dark .savebtn:active {
  /* This will be inverted */
  background-color: #b3b;
}

.stats {
  border-collapse: collapse;
  font-size: 12pt;
  table-layout: fixed;
  width: 100%;
  min-width: 450px;
}

.dark .stats td {
  border: 1px solid #bbb;
}

.stats td {
  border: 1px solid black;
  padding: 5px;
  word-wrap: break-word;
  text-align: center;
  position: relative;
}

#checkbox-stats div {
  position: absolute;
  left: 0;
  top: 0;
  height: 100%;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

#checkbox-stats .bar {
  background-color: rgba(28, 251, 0, 0.6);
}

.menu {
  position: relative;
  display: inline-block;
  margin: 0.4rem 0.4rem 0.4rem 0;
}

.menu-content {
  font-size: 12pt !important;
  text-align: left !important;
  font-weight: normal !important;
  display: none;
  position: absolute;
  background-color: white;
  right: 0;
  min-width: 300px;
  box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.2);
  z-index: 100;
  padding: 8px;
}

.dark .menu-content {
  background-color: #111;
}

.menu:hover .menu-content {
  display: block;
}

.menu:hover .menubtn,
.menu:hover .iobtn,
.menu:hover .statsbtn {
  background-color: #eee;
}

.menu-label {
  display: inline-block;
  padding: 8px;
  border: 1px solid #ccc;
  border-top: 0;
  width: calc(100% - 18px);
}

.menu-label-top {
  border-top: 1px solid #ccc;
}

.menu-textbox {
  float: left;
  height: 24px;
  margin: 10px 5px;
  padding: 5px 5px;
  font-family: Consolas, "DejaVu Sans Mono", Monaco, monospace;
  font-size: 14px;
  box-sizing: border-box;
  border: 1px solid #888;
  border-radius: 4px;
  outline: none;
  background-color: #eee;
  transition: background-color 0.2s, border 0.2s;
  width: calc(100% - 10px);
}

.menu-textbox.invalid,
.dark .menu-textbox.invalid {
  color: red;
}

.dark .menu-textbox {
  background-color: #222;
  color: #eee;
}

.radio-container {
  margin: 4px;
}

.topmostdiv {
  display: flex;
  flex-direction: column;
  width: 100%;
  background-color: white;
  transition: background-color 0.3s;
  min-height: 100%;
}

#top {
  display: flex;
  flex-wrap: wrap;
  justify-content: flex-end;
  align-items: center;
}

#topdivider {
  border-bottom: 2px solid black;
  display: flex;
  justify-content: center;
  align-items: center;
}

.dark #topdivider {
  border-bottom: 2px solid #ccc;
}

#topdivider>div {
  position: relative;
}

#toptoggle {
  cursor: pointer;
  user-select: none;
  position: absolute;
  padding: 0.1rem 0.3rem;
  top: -0.4rem;
  left: -1rem;
  font-size: 1.4rem;
  line-height: 60%;
  border: 1px solid black;
  border-radius: 1rem;
  background-color: #fff;
  z-index: 100;
}

.flipped {
  transform: rotate(0.5turn);
}

.dark #toptoggle {
  border: 1px solid #fff;
  background-color: #222;
}

#fileinfodiv {
  flex: 20rem 1 0;
  overflow: auto;
}

#bomcontrols {
  display: flex;
  flex-direction: row-reverse;
}

#bomcontrols>* {
  flex-shrink: 0;
}

#dbg {
  display: block;
}

::-webkit-scrollbar {
  width: 8px;
}

::-webkit-scrollbar-track {
  background: #aaa;
}

::-webkit-scrollbar-thumb {
  background: #666;
  border-radius: 3px;
}

::-webkit-scrollbar-thumb:hover {
  background: #555;
}

.slider {
  -webkit-appearance: none;
  width: 100%;
  margin: 3px 0;
  padding: 0;
  outline: none;
  opacity: 0.7;
  -webkit-transition: .2s;
  transition: opacity .2s;
  border-radius: 3px;
}

.slider:hover {
  opacity: 1;
}

.slider:focus {
  outline: none;
}

.slider::-webkit-slider-runnable-track {
  -webkit-appearance: none;
  width: 100%;
  height: 8px;
  background: #d3d3d3;
  border-radius: 3px;
  border: none;
}

.slider::-webkit-slider-thumb {
  -webkit-appearance: none;
  width: 15px;
  height: 15px;
  border-radius: 50%;
  background: #0a0;
  cursor: pointer;
  margin-top: -4px;
}

.dark .slider::-webkit-slider-thumb {
  background: #3d3;
}

.slider::-moz-range-thumb {
  width: 15px;
  height: 15px;
  border-radius: 50%;
  background: #0a0;
  cursor: pointer;
}

.slider::-moz-range-track {
  height: 8px;
  background: #d3d3d3;
  border-radius: 3px;
}

.dark .slider::-moz-range-thumb {
  background: #3d3;
}

.slider::-ms-track {
  width: 100%;
  height: 8px;
  border-width: 3px 0;
  background: transparent;
  border-color: transparent;
  color: transparent;
  transition: opacity .2s;
}

.slider::-ms-fill-lower {
  background: #d3d3d3;
  border: none;
  border-radius: 3px;
}

.slider::-ms-fill-upper {
  background: #d3d3d3;
  border: none;
  border-radius: 3px;
}

.slider::-ms-thumb {
  width: 15px;
  height: 15px;
  border-radius: 50%;
  background: #0a0;
  cursor: pointer;
  margin: 0;
}

.shameless-plug {
  font-size: 0.8em;
  text-align: center;
  display: block;
}

a {
  color: #0278a4;
}

.dark a {
  color: #00b9fd;
}

#frontcanvas,
#backcanvas {
  touch-action: none;
}

.placeholder {
  border: 1px dashed #9f9fda !important;
  background-color: #edf2f7 !important;
}

.dragging {
  z-index: 999;
}

.dark .dragging>table>tbody>tr {
  background-color: #252c30;
}

.dark .placeholder {
  filter: invert(1);
}

.column-spacer {
  top: 0;
  left: 0;
  width: calc(100% - 4px);
  position: absolute;
  cursor: pointer;
  user-select: none;
  height: 100%;
}

.column-width-handle {
  top: 0;
  right: 0;
  width: 4px;
  position: absolute;
  cursor: col-resize;
  user-select: none;
  height: 100%;
}

.column-width-handle:hover {
  background-color: #4f99bd;
}

.help-link {
  border: 1px solid #0278a4;
  padding-inline: 0.3rem;
  border-radius: 3px;
  cursor: pointer;
}

.dark .help-link {
  border: 1px solid #00b9fd;
}

.bom-color {
  width: 20%;
}

.color-column input {
  width: 1.6rem;
  height: 1rem;
  border: 1px solid black;
  cursor: pointer;
  padding: 0;
}

/* removes default styling from input color element */
::-webkit-color-swatch {
  border: none;
}

::-webkit-color-swatch-wrapper {
  padding: 0;
}

::-moz-color-swatch,
::-moz-focus-inner {
  border: none;
}

::-moz-focus-inner {
  padding: 0;
}
/* #bomhead {
    position: sticky;
    top: 0px;
    z-index: 1;
} */
  </style>
  <script type="text/javascript" >
///////////////////////////////////////////////
/*
  Split.js - v1.3.5
  MIT License
  https://github.com/nathancahill/Split.js
*/
!function(e,t){"object"==typeof exports&&"undefined"!=typeof module?module.exports=t():"function"==typeof define&&define.amd?define(t):e.Split=t()}(this,function(){"use strict";var e=window,t=e.document,n="addEventListener",i="removeEventListener",r="getBoundingClientRect",s=function(){return!1},o=e.attachEvent&&!e[n],a=["","-webkit-","-moz-","-o-"].filter(function(e){var n=t.createElement("div");return n.style.cssText="width:"+e+"calc(9px)",!!n.style.length}).shift()+"calc",l=function(e){return"string"==typeof e||e instanceof String?t.querySelector(e):e};return function(u,c){function z(e,t,n){var i=A(y,t,n);Object.keys(i).forEach(function(t){return e.style[t]=i[t]})}function h(e,t){var n=B(y,t);Object.keys(n).forEach(function(t){return e.style[t]=n[t]})}function f(e){var t=E[this.a],n=E[this.b],i=t.size+n.size;t.size=e/this.size*i,n.size=i-e/this.size*i,z(t.element,t.size,this.aGutterSize),z(n.element,n.size,this.bGutterSize)}function m(e){var t;this.dragging&&((t="touches"in e?e.touches[0][b]-this.start:e[b]-this.start)<=E[this.a].minSize+M+this.aGutterSize?t=E[this.a].minSize+this.aGutterSize:t>=this.size-(E[this.b].minSize+M+this.bGutterSize)&&(t=this.size-(E[this.b].minSize+this.bGutterSize)),f.call(this,t),c.onDrag&&c.onDrag())}function g(){var e=E[this.a].element,t=E[this.b].element;this.size=e[r]()[y]+t[r]()[y]+this.aGutterSize+this.bGutterSize,this.start=e[r]()[G]}function d(){var t=this,n=E[t.a].element,r=E[t.b].element;t.dragging&&c.onDragEnd&&c.onDragEnd(),t.dragging=!1,e[i]("mouseup",t.stop),e[i]("touchend",t.stop),e[i]("touchcancel",t.stop),t.parent[i]("mousemove",t.move),t.parent[i]("touchmove",t.move),delete t.stop,delete t.move,n[i]("selectstart",s),n[i]("dragstart",s),r[i]("selectstart",s),r[i]("dragstart",s),n.style.userSelect="",n.style.webkitUserSelect="",n.style.MozUserSelect="",n.style.pointerEvents="",r.style.userSelect="",r.style.webkitUserSelect="",r.style.MozUserSelect="",r.style.pointerEvents="",t.gutter.style.cursor="",t.parent.style.cursor=""}function S(t){var i=this,r=E[i.a].element,o=E[i.b].element;!i.dragging&&c.onDragStart&&c.onDragStart(),t.preventDefault(),i.dragging=!0,i.move=m.bind(i),i.stop=d.bind(i),e[n]("mouseup",i.stop),e[n]("touchend",i.stop),e[n]("touchcancel",i.stop),i.parent[n]("mousemove",i.move),i.parent[n]("touchmove",i.move),r[n]("selectstart",s),r[n]("dragstart",s),o[n]("selectstart",s),o[n]("dragstart",s),r.style.userSelect="none",r.style.webkitUserSelect="none",r.style.MozUserSelect="none",r.style.pointerEvents="none",o.style.userSelect="none",o.style.webkitUserSelect="none",o.style.MozUserSelect="none",o.style.pointerEvents="none",i.gutter.style.cursor=j,i.parent.style.cursor=j,g.call(i)}function v(e){e.forEach(function(t,n){if(n>0){var i=F[n-1],r=E[i.a],s=E[i.b];r.size=e[n-1],s.size=t,z(r.element,r.size,i.aGutterSize),z(s.element,s.size,i.bGutterSize)}})}function p(){F.forEach(function(e){e.parent.removeChild(e.gutter),E[e.a].element.style[y]="",E[e.b].element.style[y]=""})}void 0===c&&(c={});var y,b,G,E,w=l(u[0]).parentNode,D=e.getComputedStyle(w).flexDirection,U=c.sizes||u.map(function(){return 100/u.length}),k=void 0!==c.minSize?c.minSize:100,x=Array.isArray(k)?k:u.map(function(){return k}),L=void 0!==c.gutterSize?c.gutterSize:10,M=void 0!==c.snapOffset?c.snapOffset:30,O=c.direction||"horizontal",j=c.cursor||("horizontal"===O?"ew-resize":"ns-resize"),C=c.gutter||function(e,n){var i=t.createElement("div");return i.className="gutter gutter-"+n,i},A=c.elementStyle||function(e,t,n){var i={};return"string"==typeof t||t instanceof String?i[e]=t:i[e]=o?t+"%":a+"("+t+"% - "+n+"px)",i},B=c.gutterStyle||function(e,t){return n={},n[e]=t+"px",n;var n};"horizontal"===O?(y="width","clientWidth",b="clientX",G="left","paddingLeft"):"vertical"===O&&(y="height","clientHeight",b="clientY",G="top","paddingTop");var F=[];return E=u.map(function(e,t){var i,s={element:l(e),size:U[t],minSize:x[t]};if(t>0&&(i={a:t-1,b:t,dragging:!1,isFirst:1===t,isLast:t===u.length-1,direction:O,parent:w},i.aGutterSize=L,i.bGutterSize=L,i.isFirst&&(i.aGutterSize=L/2),i.isLast&&(i.bGutterSize=L/2),"row-reverse"===D||"column-reverse"===D)){var a=i.a;i.a=i.b,i.b=a}if(!o&&t>0){var c=C(t,O);h(c,L),c[n]("mousedown",S.bind(i)),c[n]("touchstart",S.bind(i)),w.insertBefore(c,s.element),i.gutter=c}0===t||t===u.length-1?z(s.element,s.size,L/2):z(s.element,s.size,L);var f=s.element[r]()[y];return f<s.minSize&&(s.minSize=f),t>0&&F.push(i),s}),o?{setSizes:v,destroy:p}:{setSizes:v,getSizes:function(){return E.map(function(e){return e.size})},collapse:function(e){if(e===F.length){var t=F[e-1];g.call(t),o||f.call(t,t.size-t.bGutterSize)}else{var n=F[e];g.call(n),o||f.call(n,n.aGutterSize)}},destroy:p}}});

///////////////////////////////////////////////

///////////////////////////////////////////////
// Copyright (c) 2013 Pieroxy <pieroxy@pieroxy.net>
// This work is free. You can redistribute it and/or modify it
// under the terms of the WTFPL, Version 2
// For more information see LICENSE.txt or http://www.wtfpl.net/
//
// For more information, the home page:
// http://pieroxy.net/blog/pages/lz-string/testing.html
//
// LZ-based compression algorithm, version 1.4.4
var LZString=function(){var o=String.fromCharCode,i={};var n={decompressFromBase64:function(o){return null==o?"":""==o?null:n._decompress(o.length,32,function(n){return function(o,n){if(!i[o]){i[o]={};for(var t=0;t<o.length;t++)i[o][o.charAt(t)]=t}return i[o][n]}("ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/=",o.charAt(n))})},_decompress:function(i,n,t){var r,e,a,s,p,u,l,f=[],c=4,d=4,h=3,v="",g=[],m={val:t(0),position:n,index:1};for(r=0;r<3;r+=1)f[r]=r;for(a=0,p=Math.pow(2,2),u=1;u!=p;)s=m.val&m.position,m.position>>=1,0==m.position&&(m.position=n,m.val=t(m.index++)),a|=(s>0?1:0)*u,u<<=1;switch(a){case 0:for(a=0,p=Math.pow(2,8),u=1;u!=p;)s=m.val&m.position,m.position>>=1,0==m.position&&(m.position=n,m.val=t(m.index++)),a|=(s>0?1:0)*u,u<<=1;l=o(a);break;case 1:for(a=0,p=Math.pow(2,16),u=1;u!=p;)s=m.val&m.position,m.position>>=1,0==m.position&&(m.position=n,m.val=t(m.index++)),a|=(s>0?1:0)*u,u<<=1;l=o(a);break;case 2:return""}for(f[3]=l,e=l,g.push(l);;){if(m.index>i)return"";for(a=0,p=Math.pow(2,h),u=1;u!=p;)s=m.val&m.position,m.position>>=1,0==m.position&&(m.position=n,m.val=t(m.index++)),a|=(s>0?1:0)*u,u<<=1;switch(l=a){case 0:for(a=0,p=Math.pow(2,8),u=1;u!=p;)s=m.val&m.position,m.position>>=1,0==m.position&&(m.position=n,m.val=t(m.index++)),a|=(s>0?1:0)*u,u<<=1;f[d++]=o(a),l=d-1,c--;break;case 1:for(a=0,p=Math.pow(2,16),u=1;u!=p;)s=m.val&m.position,m.position>>=1,0==m.position&&(m.position=n,m.val=t(m.index++)),a|=(s>0?1:0)*u,u<<=1;f[d++]=o(a),l=d-1,c--;break;case 2:return g.join("")}if(0==c&&(c=Math.pow(2,h),h++),f[l])v=f[l];else{if(l!==d)return null;v=e+e.charAt(0)}g.push(v),f[d++]=e+v.charAt(0),e=v,0==--c&&(c=Math.pow(2,h),h++)}}};return n}();"function"==typeof define&&define.amd?define(function(){return LZString}):"undefined"!=typeof module&&null!=module?module.exports=LZString:"undefined"!=typeof angular&&null!=angular&&angular.module("LZString",[]).factory("LZString",function(){return LZString});
///////////////////////////////////////////////

///////////////////////////////////////////////
/*!
 * PEP v0.4.3 | https://github.com/jquery/PEP
 * Copyright jQuery Foundation and other contributors | http://jquery.org/license
 */
!function(a,b){"object"==typeof exports&&"undefined"!=typeof module?module.exports=b():"function"==typeof define&&define.amd?define(b):a.PointerEventsPolyfill=b()}(this,function(){"use strict";function a(a,b){b=b||Object.create(null);var c=document.createEvent("Event");c.initEvent(a,b.bubbles||!1,b.cancelable||!1);
for(var d,e=2;e<m.length;e++)d=m[e],c[d]=b[d]||n[e];c.buttons=b.buttons||0;
var f=0;return f=b.pressure&&c.buttons?b.pressure:c.buttons?.5:0,c.x=c.clientX,c.y=c.clientY,c.pointerId=b.pointerId||0,c.width=b.width||0,c.height=b.height||0,c.pressure=f,c.tiltX=b.tiltX||0,c.tiltY=b.tiltY||0,c.twist=b.twist||0,c.tangentialPressure=b.tangentialPressure||0,c.pointerType=b.pointerType||"",c.hwTimestamp=b.hwTimestamp||0,c.isPrimary=b.isPrimary||!1,c}function b(){this.array=[],this.size=0}function c(a,b,c,d){this.addCallback=a.bind(d),this.removeCallback=b.bind(d),this.changedCallback=c.bind(d),A&&(this.observer=new A(this.mutationWatcher.bind(this)))}function d(a){return"body /shadow-deep/ "+e(a)}function e(a){return'[touch-action="'+a+'"]'}function f(a){return"{ -ms-touch-action: "+a+"; touch-action: "+a+"; }"}function g(){if(F){D.forEach(function(a){String(a)===a?(E+=e(a)+f(a)+"\n",G&&(E+=d(a)+f(a)+"\n")):(E+=a.selectors.map(e)+f(a.rule)+"\n",G&&(E+=a.selectors.map(d)+f(a.rule)+"\n"))});var a=document.createElement("style");a.textContent=E,document.head.appendChild(a)}}function h(){if(!window.PointerEvent){if(window.PointerEvent=a,window.navigator.msPointerEnabled){var b=window.navigator.msMaxTouchPoints;Object.defineProperty(window.navigator,"maxTouchPoints",{value:b,enumerable:!0}),u.registerSource("ms",_)}else Object.defineProperty(window.navigator,"maxTouchPoints",{value:0,enumerable:!0}),u.registerSource("mouse",N),void 0!==window.ontouchstart&&u.registerSource("touch",V);u.register(document)}}function i(a){if(!u.pointermap.has(a)){var b=new Error("InvalidPointerId");throw b.name="InvalidPointerId",b}}function j(a){for(var b=a.parentNode;b&&b!==a.ownerDocument;)b=b.parentNode;if(!b){var c=new Error("InvalidStateError");throw c.name="InvalidStateError",c}}function k(a){var b=u.pointermap.get(a);return 0!==b.buttons}function l(){window.Element&&!Element.prototype.setPointerCapture&&Object.defineProperties(Element.prototype,{setPointerCapture:{value:W},releasePointerCapture:{value:X},hasPointerCapture:{value:Y}})}
var m=["bubbles","cancelable","view","detail","screenX","screenY","clientX","clientY","ctrlKey","altKey","shiftKey","metaKey","button","relatedTarget","pageX","pageY"],n=[!1,!1,null,null,0,0,0,0,!1,!1,!1,!1,0,null,0,0],o=window.Map&&window.Map.prototype.forEach,p=o?Map:b;b.prototype={set:function(a,b){return void 0===b?this["delete"](a):(this.has(a)||this.size++,void(this.array[a]=b))},has:function(a){return void 0!==this.array[a]},"delete":function(a){this.has(a)&&(delete this.array[a],this.size--)},get:function(a){return this.array[a]},clear:function(){this.array.length=0,this.size=0},forEach:function(a,b){return this.array.forEach(function(c,d){a.call(b,c,d,this)},this)}};var q=["bubbles","cancelable","view","detail","screenX","screenY","clientX","clientY","ctrlKey","altKey","shiftKey","metaKey","button","relatedTarget","buttons","pointerId","width","height","pressure","tiltX","tiltY","pointerType","hwTimestamp","isPrimary","type","target","currentTarget","which","pageX","pageY","timeStamp"],r=[!1,!1,null,null,0,0,0,0,!1,!1,!1,!1,0,null,0,0,0,0,0,0,0,"",0,!1,"",null,null,0,0,0,0],s={pointerover:1,pointerout:1,pointerenter:1,pointerleave:1},t="undefined"!=typeof SVGElementInstance,u={pointermap:new p,eventMap:Object.create(null),captureInfo:Object.create(null),eventSources:Object.create(null),eventSourceList:[],registerSource:function(a,b){var c=b,d=c.events;d&&(d.forEach(function(a){c[a]&&(this.eventMap[a]=c[a].bind(c))},this),this.eventSources[a]=c,this.eventSourceList.push(c))},register:function(a){for(var b,c=this.eventSourceList.length,d=0;d<c&&(b=this.eventSourceList[d]);d++)
b.register.call(b,a)},unregister:function(a){for(var b,c=this.eventSourceList.length,d=0;d<c&&(b=this.eventSourceList[d]);d++)
b.unregister.call(b,a)},contains:function(a,b){try{return a.contains(b)}catch(c){return!1}},down:function(a){a.bubbles=!0,this.fireEvent("pointerdown",a)},move:function(a){a.bubbles=!0,this.fireEvent("pointermove",a)},up:function(a){a.bubbles=!0,this.fireEvent("pointerup",a)},enter:function(a){a.bubbles=!1,this.fireEvent("pointerenter",a)},leave:function(a){a.bubbles=!1,this.fireEvent("pointerleave",a)},over:function(a){a.bubbles=!0,this.fireEvent("pointerover",a)},out:function(a){a.bubbles=!0,this.fireEvent("pointerout",a)},cancel:function(a){a.bubbles=!0,this.fireEvent("pointercancel",a)},leaveOut:function(a){this.out(a),this.propagate(a,this.leave,!1)},enterOver:function(a){this.over(a),this.propagate(a,this.enter,!0)},eventHandler:function(a){if(!a._handledByPE){var b=a.type,c=this.eventMap&&this.eventMap[b];c&&c(a),a._handledByPE=!0}},listen:function(a,b){b.forEach(function(b){this.addEvent(a,b)},this)},unlisten:function(a,b){b.forEach(function(b){this.removeEvent(a,b)},this)},addEvent:function(a,b){a.addEventListener(b,this.boundHandler)},removeEvent:function(a,b){a.removeEventListener(b,this.boundHandler)},makeEvent:function(b,c){this.captureInfo[c.pointerId]&&(c.relatedTarget=null);var d=new a(b,c);return c.preventDefault&&(d.preventDefault=c.preventDefault),d._target=d._target||c.target,d},fireEvent:function(a,b){var c=this.makeEvent(a,b);return this.dispatchEvent(c)},cloneEvent:function(a){for(var b,c=Object.create(null),d=0;d<q.length;d++)b=q[d],c[b]=a[b]||r[d],!t||"target"!==b&&"relatedTarget"!==b||c[b]instanceof SVGElementInstance&&(c[b]=c[b].correspondingUseElement);return a.preventDefault&&(c.preventDefault=function(){a.preventDefault()}),c},getTarget:function(a){var b=this.captureInfo[a.pointerId];return b?a._target!==b&&a.type in s?void 0:b:a._target},propagate:function(a,b,c){for(var d=a.target,e=[];d!==document&&!d.contains(a.relatedTarget);) if(e.push(d),d=d.parentNode,!d)return;c&&e.reverse(),e.forEach(function(c){a.target=c,b.call(this,a)},this)},setCapture:function(b,c,d){this.captureInfo[b]&&this.releaseCapture(b,d),this.captureInfo[b]=c,this.implicitRelease=this.releaseCapture.bind(this,b,d),document.addEventListener("pointerup",this.implicitRelease),document.addEventListener("pointercancel",this.implicitRelease);var e=new a("gotpointercapture");e.pointerId=b,e._target=c,d||this.asyncDispatchEvent(e)},releaseCapture:function(b,c){var d=this.captureInfo[b];if(d){this.captureInfo[b]=void 0,document.removeEventListener("pointerup",this.implicitRelease),document.removeEventListener("pointercancel",this.implicitRelease);var e=new a("lostpointercapture");e.pointerId=b,e._target=d,c||this.asyncDispatchEvent(e)}},dispatchEvent:/*scope.external.dispatchEvent || */function(a){var b=this.getTarget(a);if(b)return b.dispatchEvent(a)},asyncDispatchEvent:function(a){requestAnimationFrame(this.dispatchEvent.bind(this,a))}};u.boundHandler=u.eventHandler.bind(u);var v={shadow:function(a){if(a)return a.shadowRoot||a.webkitShadowRoot},canTarget:function(a){return a&&Boolean(a.elementFromPoint)},targetingShadow:function(a){var b=this.shadow(a);if(this.canTarget(b))return b},olderShadow:function(a){var b=a.olderShadowRoot;if(!b){var c=a.querySelector("shadow");c&&(b=c.olderShadowRoot)}return b},allShadows:function(a){for(var b=[],c=this.shadow(a);c;)b.push(c),c=this.olderShadow(c);return b},searchRoot:function(a,b,c){if(a){var d,e,f=a.elementFromPoint(b,c);for(e=this.targetingShadow(f);e;){if(d=e.elementFromPoint(b,c)){var g=this.targetingShadow(d);return this.searchRoot(g,b,c)||d} e=this.olderShadow(e)} return f}},owner:function(a){
for(var b=a;b.parentNode;)b=b.parentNode;
return b.nodeType!==Node.DOCUMENT_NODE&&b.nodeType!==Node.DOCUMENT_FRAGMENT_NODE&&(b=document),b},findTarget:function(a){var b=a.clientX,c=a.clientY,d=this.owner(a.target);
return d.elementFromPoint(b,c)||(d=document),this.searchRoot(d,b,c)}},w=Array.prototype.forEach.call.bind(Array.prototype.forEach),x=Array.prototype.map.call.bind(Array.prototype.map),y=Array.prototype.slice.call.bind(Array.prototype.slice),z=Array.prototype.filter.call.bind(Array.prototype.filter),A=window.MutationObserver||window.WebKitMutationObserver,B="[touch-action]",C={subtree:!0,childList:!0,attributes:!0,attributeOldValue:!0,attributeFilter:["touch-action"]};c.prototype={watchSubtree:function(a){
//
this.observer&&v.canTarget(a)&&this.observer.observe(a,C)},enableOnSubtree:function(a){this.watchSubtree(a),a===document&&"complete"!==document.readyState?this.installOnLoad():this.installNewSubtree(a)},installNewSubtree:function(a){w(this.findElements(a),this.addElement,this)},findElements:function(a){return a.querySelectorAll?a.querySelectorAll(B):[]},removeElement:function(a){this.removeCallback(a)},addElement:function(a){this.addCallback(a)},elementChanged:function(a,b){this.changedCallback(a,b)},concatLists:function(a,b){return a.concat(y(b))},
installOnLoad:function(){document.addEventListener("readystatechange",function(){"complete"===document.readyState&&this.installNewSubtree(document)}.bind(this))},isElement:function(a){return a.nodeType===Node.ELEMENT_NODE},flattenMutationTree:function(a){
var b=x(a,this.findElements,this);
return b.push(z(a,this.isElement)),b.reduce(this.concatLists,[])},mutationWatcher:function(a){a.forEach(this.mutationHandler,this)},mutationHandler:function(a){if("childList"===a.type){var b=this.flattenMutationTree(a.addedNodes);b.forEach(this.addElement,this);var c=this.flattenMutationTree(a.removedNodes);c.forEach(this.removeElement,this)}else"attributes"===a.type&&this.elementChanged(a.target,a.oldValue)}};var D=["none","auto","pan-x","pan-y",{rule:"pan-x pan-y",selectors:["pan-x pan-y","pan-y pan-x"]}],E="",F=window.PointerEvent||window.MSPointerEvent,G=!window.ShadowDOMPolyfill&&document.head.createShadowRoot,H=u.pointermap,I=25,J=[1,4,2,8,16],K=!1;try{K=1===new MouseEvent("test",{buttons:1}).buttons}catch(L){}
var M,N={POINTER_ID:1,POINTER_TYPE:"mouse",events:["mousedown","mousemove","mouseup","mouseover","mouseout"],register:function(a){u.listen(a,this.events)},unregister:function(a){u.unlisten(a,this.events)},lastTouches:[],
isEventSimulatedFromTouch:function(a){for(var b,c=this.lastTouches,d=a.clientX,e=a.clientY,f=0,g=c.length;f<g&&(b=c[f]);f++){
var h=Math.abs(d-b.x),i=Math.abs(e-b.y);if(h<=I&&i<=I)return!0}},prepareEvent:function(a){var b=u.cloneEvent(a),c=b.preventDefault;return b.preventDefault=function(){a.preventDefault(),c()},b.pointerId=this.POINTER_ID,b.isPrimary=!0,b.pointerType=this.POINTER_TYPE,b},prepareButtonsForMove:function(a,b){var c=H.get(this.POINTER_ID);
0!==b.which&&c?a.buttons=c.buttons:a.buttons=0,b.buttons=a.buttons},mousedown:function(a){if(!this.isEventSimulatedFromTouch(a)){var b=H.get(this.POINTER_ID),c=this.prepareEvent(a);K||(c.buttons=J[c.button],b&&(c.buttons|=b.buttons),a.buttons=c.buttons),H.set(this.POINTER_ID,a),b&&0!==b.buttons?u.move(c):u.down(c)}},mousemove:function(a){if(!this.isEventSimulatedFromTouch(a)){var b=this.prepareEvent(a);K||this.prepareButtonsForMove(b,a),b.button=-1,H.set(this.POINTER_ID,a),u.move(b)}},mouseup:function(a){if(!this.isEventSimulatedFromTouch(a)){var b=H.get(this.POINTER_ID),c=this.prepareEvent(a);if(!K){var d=J[c.button];
c.buttons=b?b.buttons&~d:0,a.buttons=c.buttons}H.set(this.POINTER_ID,a),
c.buttons&=~J[c.button],0===c.buttons?u.up(c):u.move(c)}},mouseover:function(a){if(!this.isEventSimulatedFromTouch(a)){var b=this.prepareEvent(a);K||this.prepareButtonsForMove(b,a),b.button=-1,H.set(this.POINTER_ID,a),u.enterOver(b)}},mouseout:function(a){if(!this.isEventSimulatedFromTouch(a)){var b=this.prepareEvent(a);K||this.prepareButtonsForMove(b,a),b.button=-1,u.leaveOut(b)}},cancel:function(a){var b=this.prepareEvent(a);u.cancel(b),this.deactivateMouse()},deactivateMouse:function(){H["delete"](this.POINTER_ID)}},O=u.captureInfo,P=v.findTarget.bind(v),Q=v.allShadows.bind(v),R=u.pointermap,S=2500,T=200,U="touch-action",V={events:["touchstart","touchmove","touchend","touchcancel"],register:function(a){M.enableOnSubtree(a)},unregister:function(){},elementAdded:function(a){var b=a.getAttribute(U),c=this.touchActionToScrollType(b);c&&(a._scrollType=c,u.listen(a,this.events),
Q(a).forEach(function(a){a._scrollType=c,u.listen(a,this.events)},this))},elementRemoved:function(a){a._scrollType=void 0,u.unlisten(a,this.events),
Q(a).forEach(function(a){a._scrollType=void 0,u.unlisten(a,this.events)},this)},elementChanged:function(a,b){var c=a.getAttribute(U),d=this.touchActionToScrollType(c),e=this.touchActionToScrollType(b);
d&&e?(a._scrollType=d,Q(a).forEach(function(a){a._scrollType=d},this)):e?this.elementRemoved(a):d&&this.elementAdded(a)},scrollTypes:{EMITTER:"none",XSCROLLER:"pan-x",YSCROLLER:"pan-y",SCROLLER:/^(?:pan-x pan-y)|(?:pan-y pan-x)|auto$/},touchActionToScrollType:function(a){var b=a,c=this.scrollTypes;return"none"===b?"none":b===c.XSCROLLER?"X":b===c.YSCROLLER?"Y":c.SCROLLER.exec(b)?"XY":void 0},POINTER_TYPE:"touch",firstTouch:null,isPrimaryTouch:function(a){return this.firstTouch===a.identifier},setPrimaryTouch:function(a){
(0===R.size||1===R.size&&R.has(1))&&(this.firstTouch=a.identifier,this.firstXY={X:a.clientX,Y:a.clientY},this.scrolling=!1,this.cancelResetClickCount())},removePrimaryPointer:function(a){a.isPrimary&&(this.firstTouch=null,this.firstXY=null,this.resetClickCount())},clickCount:0,resetId:null,resetClickCount:function(){var a=function(){this.clickCount=0,this.resetId=null}.bind(this);this.resetId=setTimeout(a,T)},cancelResetClickCount:function(){this.resetId&&clearTimeout(this.resetId)},typeToButtons:function(a){var b=0;return"touchstart"!==a&&"touchmove"!==a||(b=1),b},touchToPointer:function(a){var b=this.currentTouchEvent,c=u.cloneEvent(a),d=c.pointerId=a.identifier+2;c.target=O[d]||P(c),c.bubbles=!0,c.cancelable=!0,c.detail=this.clickCount,c.button=0,c.buttons=this.typeToButtons(b.type),c.width=2*(a.radiusX||a.webkitRadiusX||0),c.height=2*(a.radiusY||a.webkitRadiusY||0),c.pressure=a.force||a.webkitForce||.5,c.isPrimary=this.isPrimaryTouch(a),c.pointerType=this.POINTER_TYPE,
c.altKey=b.altKey,c.ctrlKey=b.ctrlKey,c.metaKey=b.metaKey,c.shiftKey=b.shiftKey;
var e=this;return c.preventDefault=function(){e.scrolling=!1,e.firstXY=null,b.preventDefault()},c},processTouches:function(a,b){var c=a.changedTouches;this.currentTouchEvent=a;for(var d,e=0;e<c.length;e++)d=c[e],b.call(this,this.touchToPointer(d))},
shouldScroll:function(a){if(this.firstXY){var b,c=a.currentTarget._scrollType;if("none"===c)
b=!1;else if("XY"===c)
b=!0;else{var d=a.changedTouches[0],e=c,f="Y"===c?"X":"Y",g=Math.abs(d["client"+e]-this.firstXY[e]),h=Math.abs(d["client"+f]-this.firstXY[f]);
b=g>=h}return this.firstXY=null,b}},findTouch:function(a,b){for(var c,d=0,e=a.length;d<e&&(c=a[d]);d++)if(c.identifier===b)return!0},
vacuumTouches:function(a){var b=a.touches;
if(R.size>=b.length){var c=[];R.forEach(function(a,d){
if(1!==d&&!this.findTouch(b,d-2)){var e=a.out;c.push(e)}},this),c.forEach(this.cancelOut,this)}},touchstart:function(a){this.vacuumTouches(a),this.setPrimaryTouch(a.changedTouches[0]),this.dedupSynthMouse(a),this.scrolling||(this.clickCount++,this.processTouches(a,this.overDown))},overDown:function(a){R.set(a.pointerId,{target:a.target,out:a,outTarget:a.target}),u.enterOver(a),u.down(a)},touchmove:function(a){this.scrolling||(this.shouldScroll(a)?(this.scrolling=!0,this.touchcancel(a)):(a.preventDefault(),this.processTouches(a,this.moveOverOut)))},moveOverOut:function(a){var b=a,c=R.get(b.pointerId);
if(c){var d=c.out,e=c.outTarget;u.move(b),d&&e!==b.target&&(d.relatedTarget=b.target,b.relatedTarget=e,
d.target=e,b.target?(u.leaveOut(d),u.enterOver(b)):(
b.target=e,b.relatedTarget=null,this.cancelOut(b))),c.out=b,c.outTarget=b.target}},touchend:function(a){this.dedupSynthMouse(a),this.processTouches(a,this.upOut)},upOut:function(a){this.scrolling||(u.up(a),u.leaveOut(a)),this.cleanUpPointer(a)},touchcancel:function(a){this.processTouches(a,this.cancelOut)},cancelOut:function(a){u.cancel(a),u.leaveOut(a),this.cleanUpPointer(a)},cleanUpPointer:function(a){R["delete"](a.pointerId),this.removePrimaryPointer(a)},
dedupSynthMouse:function(a){var b=N.lastTouches,c=a.changedTouches[0];
if(this.isPrimaryTouch(c)){
var d={x:c.clientX,y:c.clientY};b.push(d);var e=function(a,b){var c=a.indexOf(b);c>-1&&a.splice(c,1)}.bind(null,b,d);setTimeout(e,S)}}};M=new c(V.elementAdded,V.elementRemoved,V.elementChanged,V);var W,X,Y,Z=u.pointermap,$=window.MSPointerEvent&&"number"==typeof window.MSPointerEvent.MSPOINTER_TYPE_MOUSE,_={events:["MSPointerDown","MSPointerMove","MSPointerUp","MSPointerOut","MSPointerOver","MSPointerCancel","MSGotPointerCapture","MSLostPointerCapture"],register:function(a){u.listen(a,this.events)},unregister:function(a){u.unlisten(a,this.events)},POINTER_TYPES:["","unavailable","touch","pen","mouse"],prepareEvent:function(a){var b=a;return $&&(b=u.cloneEvent(a),b.pointerType=this.POINTER_TYPES[a.pointerType]),b},cleanup:function(a){Z["delete"](a)},MSPointerDown:function(a){Z.set(a.pointerId,a);var b=this.prepareEvent(a);u.down(b)},MSPointerMove:function(a){var b=this.prepareEvent(a);u.move(b)},MSPointerUp:function(a){var b=this.prepareEvent(a);u.up(b),this.cleanup(a.pointerId)},MSPointerOut:function(a){var b=this.prepareEvent(a);u.leaveOut(b)},MSPointerOver:function(a){var b=this.prepareEvent(a);u.enterOver(b)},MSPointerCancel:function(a){var b=this.prepareEvent(a);u.cancel(b),this.cleanup(a.pointerId)},MSLostPointerCapture:function(a){var b=u.makeEvent("lostpointercapture",a);u.dispatchEvent(b)},MSGotPointerCapture:function(a){var b=u.makeEvent("gotpointercapture",a);u.dispatchEvent(b)}},aa=window.navigator;aa.msPointerEnabled?(W=function(a){i(a),j(this),k(a)&&(u.setCapture(a,this,!0),this.msSetPointerCapture(a))},X=function(a){i(a),u.releaseCapture(a,!0),this.msReleasePointerCapture(a)}):(W=function(a){i(a),j(this),k(a)&&u.setCapture(a,this)},X=function(a){i(a),u.releaseCapture(a)}),Y=function(a){return!!u.captureInfo[a]},g(),h(),l();var ba={dispatcher:u,Installer:c,PointerEvent:a,PointerMap:p,targetFinding:v};return ba});

///////////////////////////////////////////////

///////////////////////////////////////////////
var config = {"dark_mode": true, "show_pads": true, "show_fabrication": false, "show_silkscreen": true, "highlight_pin1": "none", "redraw_on_drag": true, "board_rotation": 0, "checkboxes": "Sourced,Placed", "bom_view": "left-right", "layer_view": "FB", "offset_back_rotation": false, "kicad_text_formatting": true, "fields": ["Value", "Footprint"]}
///////////////////////////////////////////////

///////////////////////////////////////////////
var pcbdata = JSON.parse(LZString.decompressFromBase64("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J0/OybzI8ctJzYHNTszizrHMQcwByXoh7ZBJzTHKSc4pyurNScvmz0nIZso0ye7P4cyFU6nIKcjricuPcclpyBDLacruyOnNns3uzc1z64+py3DMKcuIBhLPfs3KyhnPKcyxyg7KYcmJy7JU9+fdklTLIcvHTJwHMc+iyNHJTwQxy6HN0c4xyzjICcrxy/HJMc8KyvjOuM6+zK7Kqc6JzxnPKAcJ4+uIWs0YzasOwACfY5nPOcwsVjnN8c0Ez9HL+Mo5yAXJCc8KyFIFVMiJz7nNFs9LTHnP4c3LVpuNVM84yPnK+c9Ry17OYAYFzeeROc4Jz5nIxc05yobPBcpxlIXKsc6FybHJAAOxy1nJs1W6t0BRDM3Zyk2X2ctFzPHN+cqSysXP8coFzAnMuc0FzHLJWM25y4HJWch5zbHNkMo6yWHJqM06ycrJ/0rhytDNustoz77JQJPWU4yhes47TvQw006PZnHKZKIoA1ZC4M7vSgbOZMyOkAOM+wkMzeYBCgTVzSnNac4toWXMBcw4yLnJBcqGzggE+UpKzGHP5cslzJrOycilzeTE2MeHCDXKM0n9lLLKoczRymXMxc/5y9HLOctlyrXKDcm1yjNMZ2Ily+XJJckxhyXKeculDJwA9c7Zzh9MNc71zw9N9cw5z2XOZcwNy8XJ+c44zsXJds21zMIijctOzb7NhcmVy32GNlOMoobNTc41zKbIxcnxygnNZcy1z/XLxcwtyI3J5cipyUrJjc8tzq9K8pCrDIbJds2tznLNPsxlzSsMbcjlycXKzcsNz23IJ0yNy7nOJcr3Te3IN07uD9XOTcw/Th3MisjNz0XOncidzrXLzcqEy23PCsotz53N5c0tyonIFc5hy39JFcthyGzOtMzhzLrMlcvhyZXLXJZfdV6h6MhvSIULeskGID9PFDJgAbBnHMsfTAbNkc4Gz9AGr0kmUfbXfchyy9AA+cmXZvnJbspGyL7KKgqSzYABks5Zzz3KqcrJzcbJyclkyIPPanKDzibKiAWDzujIGcg5zIHPHsiSz8jOGcyJzMPNdcnyhHzSCQjLkkXPoYA3B4PLHsjyzBGG/s+hy8HPac98yxnP4c8iU0vEPFJjz3nPoYODzUXPmc4uyKPPisqjylnOns0Zy0rKFc69zzTNFc9hymzM4c5syn3LusmVz0cRwlGXYezIqsykz2oK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"))
///////////////////////////////////////////////

///////////////////////////////////////////////
/* Utility functions */

var storagePrefix = 'KiCad_HTML_BOM__' + pcbdata.metadata.title + '__' +
  pcbdata.metadata.revision + '__#';
var storage;

function initStorage(key) {
  try {
    window.localStorage.getItem("blank");
    storage = window.localStorage;
  } catch (e) {
    // localStorage not available
  }
  if (!storage) {
    try {
      window.sessionStorage.getItem("blank");
      storage = window.sessionStorage;
    } catch (e) {
      // sessionStorage also not available
    }
  }
}

function readStorage(key) {
  if (storage) {
    return storage.getItem(storagePrefix + key);
  } else {
    return null;
  }
}

function writeStorage(key, value) {
  if (storage) {
    storage.setItem(storagePrefix + key, value);
  }
}

function fancyDblClickHandler(el, onsingle, ondouble) {
  return function () {
    if (el.getAttribute("data-dblclick") == null) {
      el.setAttribute("data-dblclick", 1);
      setTimeout(function () {
        if (el.getAttribute("data-dblclick") == 1) {
          onsingle();
        }
        el.removeAttribute("data-dblclick");
      }, 200);
    } else {
      el.removeAttribute("data-dblclick");
      ondouble();
    }
  }
}

function smoothScrollToRow(rowid) {
  document.getElementById(rowid).scrollIntoView({
    behavior: "smooth",
    block: "center",
    inline: "nearest"
  });
}

function focusInputField(input) {
  input.scrollIntoView(false);
  input.focus();
  input.select();
}

function saveBomTable(output) {
  var text = '';
  for (var node of bomhead.childNodes[0].childNodes) {
    if (node.firstChild) {
      var name = node.firstChild.nodeValue ?? "";
      text += (output == 'csv' ? `"${name}"` : name);
    }
    if (node != bomhead.childNodes[0].lastChild) {
      text += (output == 'csv' ? ',' : '\t');
    }
  }
  text += '\n';
  for (var row of bombody.childNodes) {
    for (var cell of row.childNodes) {
      let val = '';
      for (var node of cell.childNodes) {
        if (node.nodeName == "INPUT") {
          if (node.checked) {
            val += '✓';
          }
        } else if ((node.nodeName == "MARK") || (node.nodeName == "A")) {
          val += node.firstChild.nodeValue;
        } else {
          val += node.nodeValue;
        }
      }
      if (output == 'csv') {
        val = val.replace(/\"/g, '\"\"'); // pair of double-quote characters
        if (isNumeric(val)) {
          val = +val;                     // use number
        } else {
          val = `"${val}"`;               // enclosed within double-quote
        }
      }
      text += val;
      if (cell != row.lastChild) {
        text += (output == 'csv' ? ',' : '\t');
      }
    }
    text += '\n';
  }

  if (output != 'clipboard') {
    // To file: csv or txt
    var blob = new Blob([text], {
      type: `text/${output}`
    });
    saveFile(`${pcbdata.metadata.title}.${output}`, blob);
  } else {
    // To clipboard
    var textArea = document.createElement("textarea");
    textArea.classList.add('clipboard-temp');
    textArea.value = text;

    document.body.appendChild(textArea);
    textArea.focus();
    textArea.select();

    try {
      if (document.execCommand('copy')) {
        console.log('Bom copied to clipboard.');
      }
    } catch (err) {
      console.log('Can not copy to clipboard.');
    }

    document.body.removeChild(textArea);
  }
}

function isNumeric(str) {
  /* https://stackoverflow.com/a/175787 */
  return (typeof str != "string" ? false : !isNaN(str) && !isNaN(parseFloat(str)));
}

function removeGutterNode(node) {
  for (var i = 0; i < node.childNodes.length; i++) {
    if (node.childNodes[i].classList &&
      node.childNodes[i].classList.contains("gutter")) {
      node.removeChild(node.childNodes[i]);
      break;
    }
  }
}

function cleanGutters() {
  removeGutterNode(document.getElementById("bot"));
  removeGutterNode(document.getElementById("canvasdiv"));
}

var units = {
  prefixes: {
    giga: ["G", "g", "giga", "Giga", "GIGA"],
    mega: ["M", "mega", "Mega", "MEGA"],
    kilo: ["K", "k", "kilo", "Kilo", "KILO"],
    milli: ["m", "milli", "Milli", "MILLI"],
    micro: ["U", "u", "micro", "Micro", "MICRO", "μ", "µ"], // different utf8 μ
    nano: ["N", "n", "nano", "Nano", "NANO"],
    pico: ["P", "p", "pico", "Pico", "PICO"],
  },
  unitsShort: ["R", "r", "Ω", "F", "f", "H", "h"],
  unitsLong: [
    "OHM", "Ohm", "ohm", "ohms",
    "FARAD", "Farad", "farad",
    "HENRY", "Henry", "henry"
  ],
  getMultiplier: function (s) {
    if (this.prefixes.giga.includes(s)) return 1e9;
    if (this.prefixes.mega.includes(s)) return 1e6;
    if (this.prefixes.kilo.includes(s)) return 1e3;
    if (this.prefixes.milli.includes(s)) return 1e-3;
    if (this.prefixes.micro.includes(s)) return 1e-6;
    if (this.prefixes.nano.includes(s)) return 1e-9;
    if (this.prefixes.pico.includes(s)) return 1e-12;
    return 1;
  },
  valueRegex: null,
  valueAltRegex: null,
}

function initUtils() {
  var allPrefixes = units.prefixes.giga
    .concat(units.prefixes.mega)
    .concat(units.prefixes.kilo)
    .concat(units.prefixes.milli)
    .concat(units.prefixes.micro)
    .concat(units.prefixes.nano)
    .concat(units.prefixes.pico);
  var allUnits = units.unitsShort.concat(units.unitsLong);
  units.valueRegex = new RegExp("^([0-9\.]+)" +
    "\\s*(" + allPrefixes.join("|") + ")?" +
    "(" + allUnits.join("|") + ")?" +
    "(\\b.*)?$", "");
  units.valueAltRegex = new RegExp("^([0-9]*)" +
    "(" + units.unitsShort.join("|") + ")?" +
    "([GgMmKkUuNnPp])?" +
    "([0-9]*)" +
    "(\\b.*)?$", "");
  if (config.fields.includes("Value")) {
    var index = config.fields.indexOf("Value");
    pcbdata.bom["parsedValues"] = {};
    var allList = getBomListByLayer('FB').flat();
    for (var id in pcbdata.bom.fields) {
      var ref_key = allList.find(item => item[1] == Number(id)) || [];
      pcbdata.bom.parsedValues[id] = parseValue(pcbdata.bom.fields[id][index], ref_key[0] || '');
    }
  }
}

function parseValue(val, ref) {
  var inferUnit = (unit, ref) => {
    if (unit) {
      unit = unit.toLowerCase();
      if (unit == 'Ω' || unit == "ohm" || unit == "ohms") {
        unit = 'r';
      }
      return unit[0];
    }

    var resarr = /^([a-z]+)\d+$/i.exec(ref);
    switch (Array.isArray(resarr) && resarr[1].toLowerCase()) {
      case "c": return 'f';
      case "l": return 'h';
      case "r":
      case "rv": return 'r';
    }
    return null;
  };
  val = val.replace(/,/g, "");
  var match = units.valueRegex.exec(val);
  if (Array.isArray(match)) {
    var unit = inferUnit(match[3], ref);
    var val_i = parseFloat(match[1]);
    if (!unit) return null;
    if (match[2]) {
      val_i = val_i * units.getMultiplier(match[2]);
    }
    return {
      val: val_i,
      unit: unit,
      extra: match[4],
    }
  }

  match = units.valueAltRegex.exec(val);
  if (Array.isArray(match) && (match[1] || match[4])) {
    var unit = inferUnit(match[2], ref);
    var val_i = parseFloat(match[1] + "." + match[4]);
    if (!unit) return null;
    if (match[3]) {
      val_i = val_i * units.getMultiplier(match[3]);
    }
    return {
      val: val_i,
      unit: unit,
      extra: match[5],
    }
  }
  return null;
}

function valueCompare(a, b, stra, strb) {
  if (a === null && b === null) {
    // Failed to parse both values, compare them as strings.
    if (stra != strb) return stra > strb ? 1 : -1;
    else return 0;
  } else if (a === null) {
    return 1;
  } else if (b === null) {
    return -1;
  } else {
    if (a.unit != b.unit) return a.unit > b.unit ? 1 : -1;
    else if (a.val != b.val) return a.val > b.val ? 1 : -1;
    else if (a.extra != b.extra) return a.extra > b.extra ? 1 : -1;
    else return 0;
  }
}

function validateSaveImgDimension(element) {
  var valid = false;
  var intValue = 0;
  if (/^[1-9]\d*$/.test(element.value)) {
    intValue = parseInt(element.value);
    if (intValue <= 16000) {
      valid = true;
    }
  }
  if (valid) {
    element.classList.remove("invalid");
  } else {
    element.classList.add("invalid");
  }
  return intValue;
}

function saveImage(layer) {
  var width = validateSaveImgDimension(document.getElementById("render-save-width"));
  var height = validateSaveImgDimension(document.getElementById("render-save-height"));
  var bgcolor = null;
  if (!document.getElementById("render-save-transparent").checked) {
    var style = getComputedStyle(topmostdiv);
    bgcolor = style.getPropertyValue("background-color");
  }
  if (!width || !height) return;

  // Prepare image
  var canvas = document.createElement("canvas");
  var layerdict = {
    transform: {
      x: 0,
      y: 0,
      s: 1,
      panx: 0,
      pany: 0,
      zoom: 1,
    },
    bg: canvas,
    fab: canvas,
    silk: canvas,
    highlight: canvas,
    layer: layer,
  }
  // Do the rendering
  recalcLayerScale(layerdict, width, height);
  prepareLayer(layerdict);
  clearCanvas(canvas, bgcolor);
  drawBackground(layerdict, false);
  drawHighlightsOnLayer(layerdict, false);

  // Save image
  var imgdata = canvas.toDataURL("image/png");

  var filename = pcbdata.metadata.title;
  if (pcbdata.metadata.revision) {
    filename += `.${pcbdata.metadata.revision}`;
  }
  filename += `.${layer}.png`;
  saveFile(filename, dataURLtoBlob(imgdata));
}

function saveSettings() {
  var data = {
    type: "InteractiveHtmlBom settings",
    version: 1,
    pcbmetadata: pcbdata.metadata,
    settings: settings,
  }
  var blob = new Blob([JSON.stringify(data, null, 4)], {
    type: "application/json"
  });
  saveFile(`${pcbdata.metadata.title}.settings.json`, blob);
}

function loadSettings() {
  var input = document.createElement("input");
  input.type = "file";
  input.accept = ".settings.json";
  input.onchange = function (e) {
    var file = e.target.files[0];
    var reader = new FileReader();
    reader.onload = readerEvent => {
      var content = readerEvent.target.result;
      var newSettings;
      try {
        newSettings = JSON.parse(content);
      } catch (e) {
        alert("Selected file is not InteractiveHtmlBom settings file.");
        return;
      }
      if (newSettings.type != "InteractiveHtmlBom settings") {
        alert("Selected file is not InteractiveHtmlBom settings file.");
        return;
      }
      var metadataMatches = newSettings.hasOwnProperty("pcbmetadata");
      if (metadataMatches) {
        for (var k in pcbdata.metadata) {
          if (!newSettings.pcbmetadata.hasOwnProperty(k) || newSettings.pcbmetadata[k] != pcbdata.metadata[k]) {
            metadataMatches = false;
          }
        }
      }
      if (!metadataMatches) {
        var currentMetadata = JSON.stringify(pcbdata.metadata, null, 4);
        var fileMetadata = JSON.stringify(newSettings.pcbmetadata, null, 4);
        if (!confirm(
          `Settins file metadata does not match current metadata.\n\n` +
          `Page metadata:\n${currentMetadata}\n\n` +
          `Settings file metadata:\n${fileMetadata}\n\n` +
          `Press OK if you would like to import settings anyway.`)) {
          return;
        }
      }
      overwriteSettings(newSettings.settings);
    }
    reader.readAsText(file, 'UTF-8');
  }
  input.click();
}

function resetSettings() {
  if (!confirm(
    `This will reset all checkbox states and other settings.\n\n` +
    `Press OK if you want to continue.`)) {
    return;
  }
  if (storage) {
    var keys = [];
    for (var i = 0; i < storage.length; i++) {
      var key = storage.key(i);
      if (key.startsWith(storagePrefix)) keys.push(key);
    }
    for (var key of keys) storage.removeItem(key);
  }
  location.reload();
}

function overwriteSettings(newSettings) {
  initDone = false;
  Object.assign(settings, newSettings);
  writeStorage("bomlayout", settings.bomlayout);
  writeStorage("bommode", settings.bommode);
  writeStorage("canvaslayout", settings.canvaslayout);
  writeStorage("bomCheckboxes", settings.checkboxes.join(","));
  document.getElementById("bomCheckboxes").value = settings.checkboxes.join(",");
  for (var checkbox of settings.checkboxes) {
    writeStorage("checkbox_" + checkbox, settings.checkboxStoredRefs[checkbox]);
  }
  writeStorage("markWhenChecked", settings.markWhenChecked);
  padsVisible(settings.renderPads);
  document.getElementById("padsCheckbox").checked = settings.renderPads;
  fabricationVisible(settings.renderFabrication);
  document.getElementById("fabricationCheckbox").checked = settings.renderFabrication;
  silkscreenVisible(settings.renderSilkscreen);
  document.getElementById("silkscreenCheckbox").checked = settings.renderSilkscreen;
  referencesVisible(settings.renderReferences);
  document.getElementById("referencesCheckbox").checked = settings.renderReferences;
  valuesVisible(settings.renderValues);
  document.getElementById("valuesCheckbox").checked = settings.renderValues;
  tracksVisible(settings.renderTracks);
  document.getElementById("tracksCheckbox").checked = settings.renderTracks;
  zonesVisible(settings.renderZones);
  document.getElementById("zonesCheckbox").checked = settings.renderZones;
  dnpOutline(settings.renderDnpOutline);
  document.getElementById("dnpOutlineCheckbox").checked = settings.renderDnpOutline;
  setRedrawOnDrag(settings.redrawOnDrag);
  document.getElementById("dragCheckbox").checked = settings.redrawOnDrag;
  setHighlightRowOnClick(settings.highlightRowOnClick);
  document.getElementById("highlightRowOnClickCheckbox").checked = settings.highlightRowOnClick;
  setDarkMode(settings.darkMode);
  document.getElementById("darkmodeCheckbox").checked = settings.darkMode;
  setHighlightPin1(settings.highlightpin1);
  document.forms.highlightpin1.highlightpin1.value = settings.highlightpin1;
  writeStorage("boardRotation", settings.boardRotation);
  document.getElementById("boardRotation").value = settings.boardRotation / 5;
  document.getElementById("rotationDegree").textContent = settings.boardRotation;
  setOffsetBackRotation(settings.offsetBackRotation);
  document.getElementById("offsetBackRotationCheckbox").checked = settings.offsetBackRotation;
  initDone = true;
  prepCheckboxes();
  changeBomLayout(settings.bomlayout);
}

function saveFile(filename, blob) {
  var link = document.createElement("a");
  var objurl = URL.createObjectURL(blob);
  link.download = filename;
  link.href = objurl;
  link.click();
}

function dataURLtoBlob(dataurl) {
  var arr = dataurl.split(','),
    mime = arr[0].match(/:(.*?);/)[1],
    bstr = atob(arr[1]),
    n = bstr.length,
    u8arr = new Uint8Array(n);
  while (n--) {
    u8arr[n] = bstr.charCodeAt(n);
  }
  return new Blob([u8arr], {
    type: mime
  });
}

var settings = {
  canvaslayout: "FB",
  bomlayout: "left-right",
  bommode: "grouped",
  checkboxes: [],
  checkboxStoredRefs: {},
  darkMode: false,
  highlightpin1: "none",
  redrawOnDrag: true,
  boardRotation: 0,
  offsetBackRotation: false,
  renderPads: true,
  renderReferences: true,
  renderValues: true,
  renderSilkscreen: true,
  renderFabrication: true,
  renderDnpOutline: false,
  renderTracks: true,
  renderZones: true,
  columnOrder: [],
  hiddenColumns: [],
  netColors: {},
}

function initDefaults() {
  settings.bomlayout = readStorage("bomlayout");
  if (settings.bomlayout === null) {
    settings.bomlayout = config.bom_view;
  }
  if (!['bom-only', 'left-right', 'top-bottom'].includes(settings.bomlayout)) {
    settings.bomlayout = config.bom_view;
  }
  settings.bommode = readStorage("bommode");
  if (settings.bommode === null) {
    settings.bommode = "grouped";
  }
  if (settings.bommode == "netlist" && !pcbdata.nets) {
    settings.bommode = "grouped";
  }
  if (!["grouped", "ungrouped", "netlist"].includes(settings.bommode)) {
    settings.bommode = "grouped";
  }
  settings.canvaslayout = readStorage("canvaslayout");
  if (settings.canvaslayout === null) {
    settings.canvaslayout = config.layer_view;
  }
  var bomCheckboxes = readStorage("bomCheckboxes");
  if (bomCheckboxes === null) {
    bomCheckboxes = config.checkboxes;
  }
  settings.checkboxes = bomCheckboxes.split(",").filter((e) => e);
  document.getElementById("bomCheckboxes").value = bomCheckboxes;

  var highlightpin1 = readStorage("highlightpin1") || config.highlight_pin1;
  if (highlightpin1 === "false") highlightpin1 = "none";
  if (highlightpin1 === "true") highlightpin1 = "all";
  setHighlightPin1(highlightpin1);
  document.forms.highlightpin1.highlightpin1.value = highlightpin1;

  settings.markWhenChecked = readStorage("markWhenChecked") || "";
  populateMarkWhenCheckedOptions();

  function initBooleanSetting(storageString, def, elementId, func) {
    var b = readStorage(storageString);
    if (b === null) {
      b = def;
    } else {
      b = (b == "true");
    }
    document.getElementById(elementId).checked = b;
    func(b);
  }

  initBooleanSetting("padsVisible", config.show_pads, "padsCheckbox", padsVisible);
  initBooleanSetting("fabricationVisible", config.show_fabrication, "fabricationCheckbox", fabricationVisible);
  initBooleanSetting("silkscreenVisible", config.show_silkscreen, "silkscreenCheckbox", silkscreenVisible);
  initBooleanSetting("referencesVisible", true, "referencesCheckbox", referencesVisible);
  initBooleanSetting("valuesVisible", true, "valuesCheckbox", valuesVisible);
  if ("tracks" in pcbdata) {
    initBooleanSetting("tracksVisible", true, "tracksCheckbox", tracksVisible);
    initBooleanSetting("zonesVisible", true, "zonesCheckbox", zonesVisible);
  } else {
    document.getElementById("tracksAndZonesCheckboxes").style.display = "none";
    tracksVisible(false);
    zonesVisible(false);
  }
  initBooleanSetting("dnpOutline", false, "dnpOutlineCheckbox", dnpOutline);
  initBooleanSetting("redrawOnDrag", config.redraw_on_drag, "dragCheckbox", setRedrawOnDrag);
  initBooleanSetting("highlightRowOnClick", false, "highlightRowOnClickCheckbox", setHighlightRowOnClick);
  initBooleanSetting("darkmode", config.dark_mode, "darkmodeCheckbox", setDarkMode);

  var fields = ["checkboxes", "References"].concat(config.fields).concat(["Quantity"]);
  var hcols = JSON.parse(readStorage("hiddenColumns"));
  if (hcols === null) {
    hcols = [];
  }
  settings.hiddenColumns = hcols.filter(e => fields.includes(e));

  var cord = JSON.parse(readStorage("columnOrder"));
  if (cord === null) {
    cord = fields;
  } else {
    cord = cord.filter(e => fields.includes(e));
    if (cord.length != fields.length)
      cord = fields;
  }
  settings.columnOrder = cord;

  settings.boardRotation = readStorage("boardRotation");
  if (settings.boardRotation === null) {
    settings.boardRotation = config.board_rotation * 5;
  } else {
    settings.boardRotation = parseInt(settings.boardRotation);
  }
  document.getElementById("boardRotation").value = settings.boardRotation / 5;
  document.getElementById("rotationDegree").textContent = settings.boardRotation;
  initBooleanSetting("offsetBackRotation", config.offset_back_rotation, "offsetBackRotationCheckbox", setOffsetBackRotation);

  settings.netColors = JSON.parse(readStorage("netColors")) || {};
}

// Helper classes for user js callbacks.

const IBOM_EVENT_TYPES = {
  ALL: "all",
  HIGHLIGHT_EVENT: "highlightEvent",
  CHECKBOX_CHANGE_EVENT: "checkboxChangeEvent",
  BOM_BODY_CHANGE_EVENT: "bomBodyChangeEvent",
}

const EventHandler = {
  callbacks: {},
  init: function () {
    for (eventType of Object.values(IBOM_EVENT_TYPES))
      this.callbacks[eventType] = [];
  },
  registerCallback: function (eventType, callback) {
    this.callbacks[eventType].push(callback);
  },
  emitEvent: function (eventType, eventArgs) {
    event = {
      eventType: eventType,
      args: eventArgs,
    }
    var callback;
    for (callback of this.callbacks[eventType])
      callback(event);
    for (callback of this.callbacks[IBOM_EVENT_TYPES.ALL])
      callback(event);
  }
}
EventHandler.init();

///////////////////////////////////////////////

///////////////////////////////////////////////
/* PCB rendering code */

var emptyContext2d = document.createElement("canvas").getContext("2d");

function deg2rad(deg) {
  return deg * Math.PI / 180;
}

function calcFontPoint(linepoint, text, offsetx, offsety, tilt) {
  var point = [
    linepoint[0] * text.width + offsetx,
    linepoint[1] * text.height + offsety
  ];
  // This approximates pcbnew behavior with how text tilts depending on horizontal justification
  point[0] -= (linepoint[1] + 0.5 * (1 + text.justify[0])) * text.height * tilt;
  return point;
}

function drawText(ctx, text, color) {
  if ("ref" in text && !settings.renderReferences) return;
  if ("val" in text && !settings.renderValues) return;
  ctx.save();
  ctx.fillStyle = color;
  ctx.strokeStyle = color;
  ctx.lineCap = "round";
  ctx.lineJoin = "round";
  ctx.lineWidth = text.thickness;
  if ("svgpath" in text) {
    ctx.stroke(new Path2D(text.svgpath));
    ctx.restore();
    return;
  }
  if ("polygons" in text) {
    ctx.fill(getPolygonsPath(text));
    ctx.restore();
    return;
  }
  ctx.translate(...text.pos);
  ctx.translate(text.thickness * 0.5, 0);
  var angle = -text.angle;
  if (text.attr.includes("mirrored")) {
    ctx.scale(-1, 1);
    angle = -angle;
  }
  var tilt = 0;
  if (text.attr.includes("italic")) {
    tilt = 0.125;
  }
  var interline = text.height * 1.5 + text.thickness;
  var txt = text.text.split("\n");
  // KiCad ignores last empty line.
  if (txt[txt.length - 1] == '') txt.pop();
  ctx.rotate(deg2rad(angle));
  var offsety = (1 - text.justify[1]) / 2 * text.height; // One line offset
  offsety -= (txt.length - 1) * (text.justify[1] + 1) / 2 * interline; // Multiline offset
  for (var i in txt) {
    var lineWidth = text.thickness + interline / 2 * tilt;
    for (var j = 0; j < txt[i].length; j++) {
      if (txt[i][j] == '\t') {
        var fourSpaces = 4 * pcbdata.font_data[' '].w * text.width;
        lineWidth += fourSpaces - lineWidth % fourSpaces;
      } else {
        if (txt[i][j] == '~') {
          j++;
          if (j == txt[i].length)
            break;
        }
        lineWidth += pcbdata.font_data[txt[i][j]].w * text.width;
      }
    }
    var offsetx = -lineWidth * (text.justify[0] + 1) / 2;
    var inOverbar = false;
    for (var j = 0; j < txt[i].length; j++) {
      if (config.kicad_text_formatting) {
        if (txt[i][j] == '\t') {
          var fourSpaces = 4 * pcbdata.font_data[' '].w * text.width;
          offsetx += fourSpaces - offsetx % fourSpaces;
          continue;
        } else if (txt[i][j] == '~') {
          j++;
          if (j == txt[i].length)
            break;
          if (txt[i][j] != '~') {
            inOverbar = !inOverbar;
          }
        }
      }
      var glyph = pcbdata.font_data[txt[i][j]];
      if (inOverbar) {
        var overbarStart = [offsetx, -text.height * 1.4 + offsety];
        var overbarEnd = [offsetx + text.width * glyph.w, overbarStart[1]];

        if (!lastHadOverbar) {
          overbarStart[0] += text.height * 1.4 * tilt;
          lastHadOverbar = true;
        }
        ctx.beginPath();
        ctx.moveTo(...overbarStart);
        ctx.lineTo(...overbarEnd);
        ctx.stroke();
      } else {
        lastHadOverbar = false;
      }
      for (var line of glyph.l) {
        ctx.beginPath();
        ctx.moveTo(...calcFontPoint(line[0], text, offsetx, offsety, tilt));
        for (var k = 1; k < line.length; k++) {
          ctx.lineTo(...calcFontPoint(line[k], text, offsetx, offsety, tilt));
        }
        ctx.stroke();
      }
      offsetx += glyph.w * text.width;
    }
    offsety += interline;
  }
  ctx.restore();
}

function drawedge(ctx, scalefactor, edge, color) {
  ctx.strokeStyle = color;
  ctx.fillStyle = color;
  ctx.lineWidth = Math.max(1 / scalefactor, edge.width);
  ctx.lineCap = "round";
  ctx.lineJoin = "round";
  if ("svgpath" in edge) {
    ctx.stroke(new Path2D(edge.svgpath));
  } else {
    ctx.beginPath();
    if (edge.type == "segment") {
      ctx.moveTo(...edge.start);
      ctx.lineTo(...edge.end);
    }
    if (edge.type == "rect") {
      ctx.moveTo(...edge.start);
      ctx.lineTo(edge.start[0], edge.end[1]);
      ctx.lineTo(...edge.end);
      ctx.lineTo(edge.end[0], edge.start[1]);
      ctx.lineTo(...edge.start);
    }
    if (edge.type == "arc") {
      ctx.arc(
        ...edge.start,
        edge.radius,
        deg2rad(edge.startangle),
        deg2rad(edge.endangle));
    }
    if (edge.type == "circle") {
      ctx.arc(
        ...edge.start,
        edge.radius,
        0, 2 * Math.PI);
      ctx.closePath();
    }
    if (edge.type == "curve") {
      ctx.moveTo(...edge.start);
      ctx.bezierCurveTo(...edge.cpa, ...edge.cpb, ...edge.end);
    }
    if("filled" in edge && edge.filled)
      ctx.fill();
    else
      ctx.stroke();
  }
}

function getChamferedRectPath(size, radius, chamfpos, chamfratio) {
  // chamfpos is a bitmask, left = 1, right = 2, bottom left = 4, bottom right = 8
  var path = new Path2D();
  var width = size[0];
  var height = size[1];
  var x = width * -0.5;
  var y = height * -0.5;
  var chamfOffset = Math.min(width, height) * chamfratio;
  path.moveTo(x, 0);
  if (chamfpos & 4) {
    path.lineTo(x, y + height - chamfOffset);
    path.lineTo(x + chamfOffset, y + height);
    path.lineTo(0, y + height);
  } else {
    path.arcTo(x, y + height, x + width, y + height, radius);
  }
  if (chamfpos & 8) {
    path.lineTo(x + width - chamfOffset, y + height);
    path.lineTo(x + width, y + height - chamfOffset);
    path.lineTo(x + width, 0);
  } else {
    path.arcTo(x + width, y + height, x + width, y, radius);
  }
  if (chamfpos & 2) {
    path.lineTo(x + width, y + chamfOffset);
    path.lineTo(x + width - chamfOffset, y);
    path.lineTo(0, y);
  } else {
    path.arcTo(x + width, y, x, y, radius);
  }
  if (chamfpos & 1) {
    path.lineTo(x + chamfOffset, y);
    path.lineTo(x, y + chamfOffset);
    path.lineTo(x, 0);
  } else {
    path.arcTo(x, y, x, y + height, radius);
  }
  path.closePath();
  return path;
}

function getOblongPath(size) {
  return getChamferedRectPath(size, Math.min(size[0], size[1]) / 2, 0, 0);
}

function getPolygonsPath(shape) {
  if (shape.path2d) {
    return shape.path2d;
  }
  if ("svgpath" in shape) {
    shape.path2d = new Path2D(shape.svgpath);
  } else {
    var path = new Path2D();
    for (var polygon of shape.polygons) {
      path.moveTo(...polygon[0]);
      for (var i = 1; i < polygon.length; i++) {
        path.lineTo(...polygon[i]);
      }
      path.closePath();
    }
    shape.path2d = path;
  }
  return shape.path2d;
}

function drawPolygonShape(ctx, scalefactor, shape, color) {
  ctx.save();
  if (!("svgpath" in shape)) {
    ctx.translate(...shape.pos);
    ctx.rotate(deg2rad(-shape.angle));
  }
  if("filled" in shape && !shape.filled) {
    ctx.strokeStyle = color;
    ctx.lineWidth = Math.max(1 / scalefactor, shape.width);
    ctx.lineCap = "round";
    ctx.lineJoin = "round";
    ctx.stroke(getPolygonsPath(shape));
  } else {
    ctx.fillStyle = color;
    ctx.fill(getPolygonsPath(shape));
  }
  ctx.restore();
}

function drawDrawing(ctx, scalefactor, drawing, color) {
  if (["segment", "arc", "circle", "curve", "rect"].includes(drawing.type)) {
    drawedge(ctx, scalefactor, drawing, color);
  } else if (drawing.type == "polygon") {
    drawPolygonShape(ctx, scalefactor, drawing, color);
  } else {
    drawText(ctx, drawing, color);
  }
}

function getCirclePath(radius) {
  var path = new Path2D();
  path.arc(0, 0, radius, 0, 2 * Math.PI);
  path.closePath();
  return path;
}

function getCachedPadPath(pad) {
  if (!pad.path2d) {
    // if path2d is not set, build one and cache it on pad object
    if (pad.shape == "rect") {
      pad.path2d = new Path2D();
      pad.path2d.rect(...pad.size.map(c => -c * 0.5), ...pad.size);
    } else if (pad.shape == "oval") {
      pad.path2d = getOblongPath(pad.size);
    } else if (pad.shape == "circle") {
      pad.path2d = getCirclePath(pad.size[0] / 2);
    } else if (pad.shape == "roundrect") {
      pad.path2d = getChamferedRectPath(pad.size, pad.radius, 0, 0);
    } else if (pad.shape == "chamfrect") {
      pad.path2d = getChamferedRectPath(pad.size, pad.radius, pad.chamfpos, pad.chamfratio)
    } else if (pad.shape == "custom") {
      pad.path2d = getPolygonsPath(pad);
    }
  }
  return pad.path2d;
}

function drawPad(ctx, pad, color, outline) {
  ctx.save();
  ctx.translate(...pad.pos);
  ctx.rotate(-deg2rad(pad.angle));
  if (pad.offset) {
    ctx.translate(...pad.offset);
  }
  ctx.fillStyle = color;
  ctx.strokeStyle = color;
  var path = getCachedPadPath(pad);
  if (outline) {
    ctx.stroke(path);
  } else {
    ctx.fill(path);
  }
  ctx.restore();
}

function drawPadHole(ctx, pad, padHoleColor) {
  if (pad.type != "th") return;
  ctx.save();
  ctx.translate(...pad.pos);
  ctx.rotate(-deg2rad(pad.angle));
  ctx.fillStyle = padHoleColor;
  if (pad.drillshape == "oblong") {
    ctx.fill(getOblongPath(pad.drillsize));
  } else if (pad.drillshape == "rect") {
    ctx.fill(getChamferedRectPath(pad.drillsize, 0, 0, 0));
  } else {
    ctx.fill(getCirclePath(pad.drillsize[0] / 2));
  }
  ctx.restore();
}

function drawFootprint(ctx, layer, scalefactor, footprint, colors, highlight, outline) {
  if (highlight) {
    // draw bounding box
    if (footprint.layer == layer) {
      ctx.save();
      ctx.globalAlpha = 0.2;
      ctx.translate(...footprint.bbox.pos);
      ctx.rotate(deg2rad(-footprint.bbox.angle));
      ctx.translate(...footprint.bbox.relpos);
      ctx.fillStyle = colors.pad;
      ctx.fillRect(0, 0, ...footprint.bbox.size);
      ctx.globalAlpha = 1;
      ctx.strokeStyle = colors.pad;
      ctx.lineWidth = 3 / scalefactor;
      ctx.strokeRect(0, 0, ...footprint.bbox.size);
      ctx.restore();
    }
  }
  // draw drawings
  for (var drawing of footprint.drawings) {
    if (drawing.layer == layer) {
      drawDrawing(ctx, scalefactor, drawing.drawing, colors.pad);
    }
  }
  ctx.lineWidth = 3 / scalefactor;
  // draw pads
  if (settings.renderPads) {
    for (var pad of footprint.pads) {
      if (pad.layers.includes(layer)) {
        drawPad(ctx, pad, colors.pad, outline);
        if (pad.pin1 &&
          (settings.highlightpin1 == "all" ||
            settings.highlightpin1 == "selected" && highlight)) {
          drawPad(ctx, pad, colors.outline, true);
        }
      }
    }
    for (var pad of footprint.pads) {
      drawPadHole(ctx, pad, colors.padHole);
    }
  }
}

function drawEdgeCuts(canvas, scalefactor) {
  var ctx = canvas.getContext("2d");
  var edgecolor = getComputedStyle(topmostdiv).getPropertyValue('--pcb-edge-color');
  for (var edge of pcbdata.edges) {
    drawDrawing(ctx, scalefactor, edge, edgecolor);
  }
}

function drawFootprints(canvas, layer, scalefactor, highlight) {
  var ctx = canvas.getContext("2d");
  ctx.lineWidth = 3 / scalefactor;
  var style = getComputedStyle(topmostdiv);

  var colors = {
    pad: style.getPropertyValue('--pad-color'),
    padHole: style.getPropertyValue('--pad-hole-color'),
    outline: style.getPropertyValue('--pin1-outline-color'),
  }

  for (var i = 0; i < pcbdata.footprints.length; i++) {
    var mod = pcbdata.footprints[i];
    var outline = settings.renderDnpOutline && pcbdata.bom.skipped.includes(i);
    var h = highlightedFootprints.includes(i);
    var d = markedFootprints.has(i);
    if (highlight) {
      if(h && d) {
        colors.pad = style.getPropertyValue('--pad-color-highlight-both');
        colors.outline = style.getPropertyValue('--pin1-outline-color-highlight-both');
      } else if (h) {
        colors.pad = style.getPropertyValue('--pad-color-highlight');
        colors.outline = style.getPropertyValue('--pin1-outline-color-highlight');
      } else if (d) {
        colors.pad = style.getPropertyValue('--pad-color-highlight-marked');
        colors.outline = style.getPropertyValue('--pin1-outline-color-highlight-marked');
      }
    }
    if( h || d || !highlight) {
      drawFootprint(ctx, layer, scalefactor, mod, colors, highlight, outline);
    }
  }
}

function drawBgLayer(layername, canvas, layer, scalefactor, edgeColor, polygonColor, textColor) {
  var ctx = canvas.getContext("2d");
  for (var d of pcbdata.drawings[layername][layer]) {
    if (["segment", "arc", "circle", "curve", "rect"].includes(d.type)) {
      drawedge(ctx, scalefactor, d, edgeColor);
    } else if (d.type == "polygon") {
      drawPolygonShape(ctx, scalefactor, d, polygonColor);
    } else {
      drawText(ctx, d, textColor);
    }
  }
}

function drawTracks(canvas, layer, defaultColor, highlight) {
  ctx = canvas.getContext("2d");
  ctx.lineCap = "round";

  var hasHole = (track) => (
    'drillsize' in track &&
    track.start[0] == track.end[0] &&
    track.start[1] == track.end[1]);

  // First draw tracks and tented vias
  for (var track of pcbdata.tracks[layer]) {
    if (highlight && highlightedNet != track.net) continue;
    if (!hasHole(track)) {
      ctx.strokeStyle = highlight ? defaultColor : settings.netColors[track.net] || defaultColor;
      ctx.lineWidth = track.width;
      ctx.beginPath();
      if ('radius' in track) {
        ctx.arc(
          ...track.center,
          track.radius,
          deg2rad(track.startangle),
          deg2rad(track.endangle));
      } else {
        ctx.moveTo(...track.start);
        ctx.lineTo(...track.end);
      }
      ctx.stroke();
    }
  }
  // Second pass to draw untented vias
  var style = getComputedStyle(topmostdiv);
  var holeColor = style.getPropertyValue('--pad-hole-color')

  for (var track of pcbdata.tracks[layer]) {
    if (highlight && highlightedNet != track.net) continue;
    if (hasHole(track)) {
      ctx.strokeStyle = highlight ? defaultColor : settings.netColors[track.net] || defaultColor;
      ctx.lineWidth = track.width;
      ctx.beginPath();
      ctx.moveTo(...track.start);
      ctx.lineTo(...track.end);
      ctx.stroke();
      ctx.strokeStyle = holeColor;
      ctx.lineWidth = track.drillsize;
      ctx.lineTo(...track.end);
      ctx.stroke();
    }
  }
}

function drawZones(canvas, layer, defaultColor, highlight) {
  ctx = canvas.getContext("2d");
  ctx.lineJoin = "round";
  for (var zone of pcbdata.zones[layer]) {
    if (highlight && highlightedNet != zone.net) continue;
    ctx.strokeStyle = highlight ? defaultColor : settings.netColors[zone.net] || defaultColor;
    ctx.fillStyle = highlight ? defaultColor : settings.netColors[zone.net] || defaultColor;
    if (!zone.path2d) {
      zone.path2d = getPolygonsPath(zone);
    }
    ctx.fill(zone.path2d, zone.fillrule || "nonzero");
    if (zone.width > 0) {
      ctx.lineWidth = zone.width;
      ctx.stroke(zone.path2d);
    }
  }
}

function clearCanvas(canvas, color = null) {
  var ctx = canvas.getContext("2d");
  ctx.save();
  ctx.setTransform(1, 0, 0, 1, 0, 0);
  if (color) {
    ctx.fillStyle = color;
    ctx.fillRect(0, 0, canvas.width, canvas.height);
  } else {
    if (!window.matchMedia("print").matches)
      ctx.clearRect(0, 0, canvas.width, canvas.height);
  }
  ctx.restore();
}

function drawNets(canvas, layer, highlight) {
  var style = getComputedStyle(topmostdiv);
  if (settings.renderZones) {
    var zoneColor = style.getPropertyValue(highlight ? '--zone-color-highlight' : '--zone-color');
    drawZones(canvas, layer, zoneColor, highlight);
  }
  if (settings.renderTracks) {
    var trackColor = style.getPropertyValue(highlight ? '--track-color-highlight' : '--track-color');
    drawTracks(canvas, layer, trackColor, highlight);
  }
  if (highlight && settings.renderPads) {
    var padColor = style.getPropertyValue('--pad-color-highlight');
    var padHoleColor = style.getPropertyValue('--pad-hole-color');
    var ctx = canvas.getContext("2d");
    for (var footprint of pcbdata.footprints) {
      // draw pads
      var padDrawn = false;
      for (var pad of footprint.pads) {
        if (highlightedNet != pad.net) continue;
        if (pad.layers.includes(layer)) {
          drawPad(ctx, pad, padColor, false);
          padDrawn = true;
        }
      }
      if (padDrawn) {
        // redraw all pad holes because some pads may overlap
        for (var pad of footprint.pads) {
          drawPadHole(ctx, pad, padHoleColor);
        }
      }
    }
  }
}

function drawHighlightsOnLayer(canvasdict, clear = true) {
  if (clear) {
    clearCanvas(canvasdict.highlight);
  }
  if (markedFootprints.size > 0 || highlightedFootprints.length > 0) {
    drawFootprints(canvasdict.highlight, canvasdict.layer,
      canvasdict.transform.s * canvasdict.transform.zoom, true);
  }
  if (highlightedNet !== null) {
    drawNets(canvasdict.highlight, canvasdict.layer, true);
  }
}

function drawHighlights() {
  drawHighlightsOnLayer(allcanvas.front);
  drawHighlightsOnLayer(allcanvas.back);
}

function drawBackground(canvasdict, clear = true) {
  if (clear) {
    clearCanvas(canvasdict.bg);
    clearCanvas(canvasdict.fab);
    clearCanvas(canvasdict.silk);
  }

  drawNets(canvasdict.bg, canvasdict.layer, false);
  drawFootprints(canvasdict.bg, canvasdict.layer,
    canvasdict.transform.s * canvasdict.transform.zoom, false);

  drawEdgeCuts(canvasdict.bg, canvasdict.transform.s * canvasdict.transform.zoom);

  var style = getComputedStyle(topmostdiv);
  var edgeColor = style.getPropertyValue('--silkscreen-edge-color');
  var polygonColor = style.getPropertyValue('--silkscreen-polygon-color');
  var textColor = style.getPropertyValue('--silkscreen-text-color');
  if (settings.renderSilkscreen) {
    drawBgLayer(
      "silkscreen", canvasdict.silk, canvasdict.layer,
      canvasdict.transform.s * canvasdict.transform.zoom,
      edgeColor, polygonColor, textColor);
  }
  edgeColor = style.getPropertyValue('--fabrication-edge-color');
  polygonColor = style.getPropertyValue('--fabrication-polygon-color');
  textColor = style.getPropertyValue('--fabrication-text-color');
  if (settings.renderFabrication) {
    drawBgLayer(
      "fabrication", canvasdict.fab, canvasdict.layer,
      canvasdict.transform.s * canvasdict.transform.zoom,
      edgeColor, polygonColor, textColor);
  }
}

function prepareCanvas(canvas, flip, transform) {
  var ctx = canvas.getContext("2d");
  ctx.setTransform(1, 0, 0, 1, 0, 0);
  ctx.scale(transform.zoom, transform.zoom);
  ctx.translate(transform.panx, transform.pany);
  if (flip) {
    ctx.scale(-1, 1);
  }
  ctx.translate(transform.x, transform.y);
  ctx.rotate(deg2rad(settings.boardRotation + (flip && settings.offsetBackRotation ? - 180 : 0)));
  ctx.scale(transform.s, transform.s);
}

function prepareLayer(canvasdict) {
  var flip = (canvasdict.layer === "B");
  for (var c of ["bg", "fab", "silk", "highlight"]) {
    prepareCanvas(canvasdict[c], flip, canvasdict.transform);
  }
}

function rotateVector(v, angle) {
  angle = deg2rad(angle);
  return [
    v[0] * Math.cos(angle) - v[1] * Math.sin(angle),
    v[0] * Math.sin(angle) + v[1] * Math.cos(angle)
  ];
}

function applyRotation(bbox, flip) {
  var corners = [
    [bbox.minx, bbox.miny],
    [bbox.minx, bbox.maxy],
    [bbox.maxx, bbox.miny],
    [bbox.maxx, bbox.maxy],
  ];
  corners = corners.map((v) => rotateVector(v, settings.boardRotation + (flip && settings.offsetBackRotation ? - 180 : 0)));
  return {
    minx: corners.reduce((a, v) => Math.min(a, v[0]), Infinity),
    miny: corners.reduce((a, v) => Math.min(a, v[1]), Infinity),
    maxx: corners.reduce((a, v) => Math.max(a, v[0]), -Infinity),
    maxy: corners.reduce((a, v) => Math.max(a, v[1]), -Infinity),
  }
}

function recalcLayerScale(layerdict, width, height) {
  var flip = (layerdict.layer === "B");
  var bbox = applyRotation(pcbdata.edges_bbox, flip);
  var scalefactor = 0.98 * Math.min(
    width / (bbox.maxx - bbox.minx),
    height / (bbox.maxy - bbox.miny)
  );
  if (scalefactor < 0.1) {
    scalefactor = 1;
  }
  layerdict.transform.s = scalefactor;
  if (flip) {
    layerdict.transform.x = -((bbox.maxx + bbox.minx) * scalefactor + width) * 0.5;
  } else {
    layerdict.transform.x = -((bbox.maxx + bbox.minx) * scalefactor - width) * 0.5;
  }
  layerdict.transform.y = -((bbox.maxy + bbox.miny) * scalefactor - height) * 0.5;
  for (var c of ["bg", "fab", "silk", "highlight"]) {
    canvas = layerdict[c];
    canvas.width = width;
    canvas.height = height;
    canvas.style.width = (width / devicePixelRatio) + "px";
    canvas.style.height = (height / devicePixelRatio) + "px";
  }
}

function redrawCanvas(layerdict) {
  prepareLayer(layerdict);
  drawBackground(layerdict);
  drawHighlightsOnLayer(layerdict);
}

function resizeCanvas(layerdict) {
  var canvasdivid = {
    "F": "frontcanvas",
    "B": "backcanvas"
  } [layerdict.layer];
  var width = document.getElementById(canvasdivid).clientWidth * devicePixelRatio;
  var height = document.getElementById(canvasdivid).clientHeight * devicePixelRatio;
  recalcLayerScale(layerdict, width, height);
  redrawCanvas(layerdict);
}

function resizeAll() {
  resizeCanvas(allcanvas.front);
  resizeCanvas(allcanvas.back);
}

function pointWithinDistanceToSegment(x, y, x1, y1, x2, y2, d) {
  var A = x - x1;
  var B = y - y1;
  var C = x2 - x1;
  var D = y2 - y1;

  var dot = A * C + B * D;
  var len_sq = C * C + D * D;
  var dx, dy;
  if (len_sq == 0) {
    // start and end of the segment coincide
    dx = x - x1;
    dy = y - y1;
  } else {
    var param = dot / len_sq;
    var xx, yy;
    if (param < 0) {
      xx = x1;
      yy = y1;
    } else if (param > 1) {
      xx = x2;
      yy = y2;
    } else {
      xx = x1 + param * C;
      yy = y1 + param * D;
    }
    dx = x - xx;
    dy = y - yy;
  }
  return dx * dx + dy * dy <= d * d;
}

function modulo(n, mod) {
  return ((n % mod) + mod) % mod;
}

function pointWithinDistanceToArc(x, y, xc, yc, radius, startangle, endangle, d) {
  var dx = x - xc;
  var dy = y - yc;
  var r_sq = dx * dx + dy * dy;
  var rmin = Math.max(0, radius - d);
  var rmax = radius + d;

  if (r_sq < rmin * rmin || r_sq > rmax * rmax)
    return false;

  var angle1 = modulo(deg2rad(startangle), 2 * Math.PI);
  var dx1 = xc + radius * Math.cos(angle1) - x;
  var dy1 = yc + radius * Math.sin(angle1) - y;
  if (dx1 * dx1 + dy1 * dy1 <= d * d)
    return true;

  var angle2 = modulo(deg2rad(endangle), 2 * Math.PI);
  var dx2 = xc + radius * Math.cos(angle2) - x;
  var dy2 = yc + radius * Math.sin(angle2) - y;
  if (dx2 * dx2 + dy2 * dy2 <= d * d)
    return true;

  var angle = modulo(Math.atan2(dy, dx), 2 * Math.PI);
  if (angle1 > angle2)
    return (angle >= angle2 || angle <= angle1);
  else
    return (angle >= angle1 && angle <= angle2);
}

function pointWithinPad(x, y, pad) {
  var v = [x - pad.pos[0], y - pad.pos[1]];
  v = rotateVector(v, pad.angle);
  if (pad.offset) {
    v[0] -= pad.offset[0];
    v[1] -= pad.offset[1];
  }
  return emptyContext2d.isPointInPath(getCachedPadPath(pad), ...v);
}

function netHitScan(layer, x, y) {
  // Check track segments
  if (settings.renderTracks && pcbdata.tracks) {
    for (var track of pcbdata.tracks[layer]) {
      if ('radius' in track) {
        if (pointWithinDistanceToArc(x, y, ...track.center, track.radius, track.startangle, track.endangle, track.width / 2)) {
          return track.net;
        }
      } else {
        if (pointWithinDistanceToSegment(x, y, ...track.start, ...track.end, track.width / 2)) {
          return track.net;
        }
      }
    }
  }
  // Check pads
  if (settings.renderPads) {
    for (var footprint of pcbdata.footprints) {
      for (var pad of footprint.pads) {
        if (pad.layers.includes(layer) && pointWithinPad(x, y, pad)) {
          return pad.net;
        }
      }
    }
  }
  return null;
}

function pointWithinFootprintBbox(x, y, bbox) {
  var v = [x - bbox.pos[0], y - bbox.pos[1]];
  v = rotateVector(v, bbox.angle);
  return bbox.relpos[0] <= v[0] && v[0] <= bbox.relpos[0] + bbox.size[0] &&
    bbox.relpos[1] <= v[1] && v[1] <= bbox.relpos[1] + bbox.size[1];
}

function bboxHitScan(layer, x, y) {
  var result = [];
  for (var i = 0; i < pcbdata.footprints.length; i++) {
    var footprint = pcbdata.footprints[i];
    if (footprint.layer == layer) {
      if (pointWithinFootprintBbox(x, y, footprint.bbox)) {
        result.push(i);
      }
    }
  }
  return result;
}

function handlePointerDown(e, layerdict) {
  if (e.button != 0 && e.button != 1) {
    return;
  }
  e.preventDefault();
  e.stopPropagation();

  if (!e.hasOwnProperty("offsetX")) {
    // The polyfill doesn't set this properly
    e.offsetX = e.pageX - e.currentTarget.offsetLeft;
    e.offsetY = e.pageY - e.currentTarget.offsetTop;
  }

  layerdict.pointerStates[e.pointerId] = {
    distanceTravelled: 0,
    lastX: e.offsetX,
    lastY: e.offsetY,
    downTime: Date.now(),
  };
}

function handleMouseClick(e, layerdict) {
  if (!e.hasOwnProperty("offsetX")) {
    // The polyfill doesn't set this properly
    e.offsetX = e.pageX - e.currentTarget.offsetLeft;
    e.offsetY = e.pageY - e.currentTarget.offsetTop;
  }

  var x = e.offsetX;
  var y = e.offsetY;
  var t = layerdict.transform;
  var flip = layerdict.layer === "B";
  if (flip) {
    x = (devicePixelRatio * x / t.zoom - t.panx + t.x) / -t.s;
  } else {
    x = (devicePixelRatio * x / t.zoom - t.panx - t.x) / t.s;
  }
  y = (devicePixelRatio * y / t.zoom - t.y - t.pany) / t.s;
  var v = rotateVector([x, y], -settings.boardRotation + (flip && settings.offsetBackRotation ? - 180 : 0));
  if ("nets" in pcbdata) {
    var net = netHitScan(layerdict.layer, ...v);
    if (net !== highlightedNet) {
      netClicked(net);
    }
  }
  if (highlightedNet === null) {
    var footprints = bboxHitScan(layerdict.layer, ...v);
    if (footprints.length > 0) {
      footprintsClicked(footprints);
    }
  }
}

function handlePointerLeave(e, layerdict) {
  e.preventDefault();
  e.stopPropagation();

  if (!settings.redrawOnDrag) {
    redrawCanvas(layerdict);
  }

  delete layerdict.pointerStates[e.pointerId];
}

function resetTransform(layerdict) {
  layerdict.transform.panx = 0;
  layerdict.transform.pany = 0;
  layerdict.transform.zoom = 1;
  redrawCanvas(layerdict);
}

function handlePointerUp(e, layerdict) {
  if (!e.hasOwnProperty("offsetX")) {
    // The polyfill doesn't set this properly
    e.offsetX = e.pageX - e.currentTarget.offsetLeft;
    e.offsetY = e.pageY - e.currentTarget.offsetTop;
  }

  e.preventDefault();
  e.stopPropagation();

  if (e.button == 2) {
    // Reset pan and zoom on right click.
    resetTransform(layerdict);
    layerdict.anotherPointerTapped = false;
    return;
  }

  // We haven't necessarily had a pointermove event since the interaction started, so make sure we update this now
  var ptr = layerdict.pointerStates[e.pointerId];
  ptr.distanceTravelled += Math.abs(e.offsetX - ptr.lastX) + Math.abs(e.offsetY - ptr.lastY);

  if (e.button == 0 && ptr.distanceTravelled < 10 && Date.now() - ptr.downTime <= 500) {
    if (Object.keys(layerdict.pointerStates).length == 1) {
      if (layerdict.anotherPointerTapped) {
        // This is the second pointer coming off of a two-finger tap
        resetTransform(layerdict);
      } else {
        // This is just a regular tap
        handleMouseClick(e, layerdict);
      }
      layerdict.anotherPointerTapped = false;
    } else {
      // This is the first finger coming off of what could become a two-finger tap
      layerdict.anotherPointerTapped = true;
    }
  } else {
    if (!settings.redrawOnDrag) {
      redrawCanvas(layerdict);
    }
    layerdict.anotherPointerTapped = false;
  }

  delete layerdict.pointerStates[e.pointerId];
}

function handlePointerMove(e, layerdict) {
  if (!layerdict.pointerStates.hasOwnProperty(e.pointerId)) {
    return;
  }
  e.preventDefault();
  e.stopPropagation();

  if (!e.hasOwnProperty("offsetX")) {
    // The polyfill doesn't set this properly
    e.offsetX = e.pageX - e.currentTarget.offsetLeft;
    e.offsetY = e.pageY - e.currentTarget.offsetTop;
  }

  var thisPtr = layerdict.pointerStates[e.pointerId];

  var dx = e.offsetX - thisPtr.lastX;
  var dy = e.offsetY - thisPtr.lastY;

  // If this number is low on pointer up, we count the action as a click
  thisPtr.distanceTravelled += Math.abs(dx) + Math.abs(dy);

  if (Object.keys(layerdict.pointerStates).length == 1) {
    // This is a simple drag
    layerdict.transform.panx += devicePixelRatio * dx / layerdict.transform.zoom;
    layerdict.transform.pany += devicePixelRatio * dy / layerdict.transform.zoom;
  } else if (Object.keys(layerdict.pointerStates).length == 2) {
    var otherPtr = Object.values(layerdict.pointerStates).filter((ptr) => ptr != thisPtr)[0];

    var oldDist = Math.sqrt(Math.pow(thisPtr.lastX - otherPtr.lastX, 2) + Math.pow(thisPtr.lastY - otherPtr.lastY, 2));
    var newDist = Math.sqrt(Math.pow(e.offsetX - otherPtr.lastX, 2) + Math.pow(e.offsetY - otherPtr.lastY, 2));

    var scaleFactor = newDist / oldDist;

    if (scaleFactor != NaN) {
      layerdict.transform.zoom *= scaleFactor;

      var zoomd = (1 - scaleFactor) / layerdict.transform.zoom;
      layerdict.transform.panx += devicePixelRatio * otherPtr.lastX * zoomd;
      layerdict.transform.pany += devicePixelRatio * otherPtr.lastY * zoomd;
    }
  }

  thisPtr.lastX = e.offsetX;
  thisPtr.lastY = e.offsetY;

  if (settings.redrawOnDrag) {
    redrawCanvas(layerdict);
  }
}

function handleMouseWheel(e, layerdict) {
  e.preventDefault();
  e.stopPropagation();
  var t = layerdict.transform;
  var wheeldelta = e.deltaY;
  if (e.deltaMode == 1) {
    // FF only, scroll by lines
    wheeldelta *= 30;
  } else if (e.deltaMode == 2) {
    wheeldelta *= 300;
  }
  var m = Math.pow(1.1, -wheeldelta / 40);
  // Limit amount of zoom per tick.
  if (m > 2) {
    m = 2;
  } else if (m < 0.5) {
    m = 0.5;
  }
  t.zoom *= m;
  var zoomd = (1 - m) / t.zoom;
  t.panx += devicePixelRatio * e.offsetX * zoomd;
  t.pany += devicePixelRatio * e.offsetY * zoomd;
  redrawCanvas(layerdict);
}

function addMouseHandlers(div, layerdict) {
  div.addEventListener("pointerdown", function(e) {
    handlePointerDown(e, layerdict);
  });
  div.addEventListener("pointermove", function(e) {
    handlePointerMove(e, layerdict);
  });
  div.addEventListener("pointerup", function(e) {
    handlePointerUp(e, layerdict);
  });
  var pointerleave = function(e) {
    handlePointerLeave(e, layerdict);
  }
  div.addEventListener("pointercancel", pointerleave);
  div.addEventListener("pointerleave", pointerleave);
  div.addEventListener("pointerout", pointerleave);

  div.onwheel = function(e) {
    handleMouseWheel(e, layerdict);
  }
  for (var element of [div, layerdict.bg, layerdict.fab, layerdict.silk, layerdict.highlight]) {
    element.addEventListener("contextmenu", function(e) {
      e.preventDefault();
    }, false);
  }
}

function setRedrawOnDrag(value) {
  settings.redrawOnDrag = value;
  writeStorage("redrawOnDrag", value);
}

function setBoardRotation(value) {
  settings.boardRotation = value * 5;
  writeStorage("boardRotation", settings.boardRotation);
  document.getElementById("rotationDegree").textContent = settings.boardRotation;
  resizeAll();
}

function setOffsetBackRotation(value) {
  settings.offsetBackRotation = value;
  writeStorage("offsetBackRotation", value);
  resizeAll();
}

function initRender() {
  allcanvas = {
    front: {
      transform: {
        x: 0,
        y: 0,
        s: 1,
        panx: 0,
        pany: 0,
        zoom: 1,
      },
      pointerStates: {},
      anotherPointerTapped: false,
      bg: document.getElementById("F_bg"),
      fab: document.getElementById("F_fab"),
      silk: document.getElementById("F_slk"),
      highlight: document.getElementById("F_hl"),
      layer: "F",
    },
    back: {
      transform: {
        x: 0,
        y: 0,
        s: 1,
        panx: 0,
        pany: 0,
        zoom: 1,
      },
      pointerStates: {},
      anotherPointerTapped: false,
      bg: document.getElementById("B_bg"),
      fab: document.getElementById("B_fab"),
      silk: document.getElementById("B_slk"),
      highlight: document.getElementById("B_hl"),
      layer: "B",
    }
  };
  addMouseHandlers(document.getElementById("frontcanvas"), allcanvas.front);
  addMouseHandlers(document.getElementById("backcanvas"), allcanvas.back);
}

///////////////////////////////////////////////

///////////////////////////////////////////////
/*
 * Table reordering via Drag'n'Drop
 * Inspired by: https://htmldom.dev/drag-and-drop-table-column
 */

function setBomHandlers() {

  const bom = document.getElementById('bomtable');

  let dragName;
  let placeHolderElements;
  let draggingElement;
  let forcePopulation;
  let xOffset;
  let yOffset;
  let wasDragged;

  const mouseUpHandler = function(e) {
    // Delete dragging element
    draggingElement.remove();

    // Make BOM selectable again
    bom.style.removeProperty("userSelect");

    // Remove listeners
    document.removeEventListener('mousemove', mouseMoveHandler);
    document.removeEventListener('mouseup', mouseUpHandler);

    if (wasDragged) {
      // Redraw whole BOM
      populateBomTable();
    }
  }

  const mouseMoveHandler = function(e) {
    // Notice the dragging
    wasDragged = true;

    // Make the dragged element visible
    draggingElement.style.removeProperty("display");

    // Set elements position to mouse position
    draggingElement.style.left = `${e.screenX - xOffset}px`;
    draggingElement.style.top = `${e.screenY - yOffset}px`;

    // Forced redrawing of BOM table
    if (forcePopulation) {
      forcePopulation = false;
      // Copy array
      phe = Array.from(placeHolderElements);
      // populate BOM table again
      populateBomHeader(dragName, phe);
      populateBomBody(dragName, phe);
    }

    // Set up array of hidden columns
    var hiddenColumns = Array.from(settings.hiddenColumns);
    // In the ungrouped mode, quantity don't exist
    if (settings.bommode === "ungrouped")
      hiddenColumns.push("Quantity");
    // If no checkbox fields can be found, we consider them hidden
    if (settings.checkboxes.length == 0)
      hiddenColumns.push("checkboxes");

    // Get table headers and group them into checkboxes, extrafields and normal headers
    const bh = document.getElementById("bomhead");
    headers = Array.from(bh.querySelectorAll("th"))
    headers.shift() // numCol is not part of the columnOrder
    headerGroups = []
    lastCompoundClass = null;
    for (i = 0; i < settings.columnOrder.length; i++) {
      cElem = settings.columnOrder[i];
      if (hiddenColumns.includes(cElem)) {
        // Hidden columns appear as a dummy element
        headerGroups.push([]);
        continue;
      }
      elem = headers.filter(e => getColumnOrderName(e) === cElem)[0];
      if (elem.classList.contains("bom-checkbox")) {
        if (lastCompoundClass === "bom-checkbox") {
          cbGroup = headerGroups.pop();
          cbGroup.push(elem);
          headerGroups.push(cbGroup);
        } else {
          lastCompoundClass = "bom-checkbox";
          headerGroups.push([elem])
        }
      } else {
        headerGroups.push([elem])
      }
    }

    // Copy settings.columnOrder
    var columns = Array.from(settings.columnOrder)

    // Set up array with indices of hidden columns
    var hiddenIndices = hiddenColumns.map(e => settings.columnOrder.indexOf(e));
    var dragIndex = columns.indexOf(dragName);
    var swapIndex = dragIndex;
    var swapDone = false;

    // Check if the current dragged element is swapable with the left or right element
    if (dragIndex > 0) {
      // Get left headers boundingbox
      swapIndex = dragIndex - 1;
      while (hiddenIndices.includes(swapIndex) && swapIndex > 0)
        swapIndex--;
      if (!hiddenIndices.includes(swapIndex)) {
        box = getBoundingClientRectFromMultiple(headerGroups[swapIndex]);
        if (e.clientX < box.left + window.scrollX + (box.width / 2)) {
          swapElement = columns[dragIndex];
          columns.splice(dragIndex, 1);
          columns.splice(swapIndex, 0, swapElement);
          forcePopulation = true;
          swapDone = true;
        }
      }
    }
    if ((!swapDone) && dragIndex < headerGroups.length - 1) {
      // Get right headers boundingbox
      swapIndex = dragIndex + 1;
      while (hiddenIndices.includes(swapIndex))
        swapIndex++;
      if (swapIndex < headerGroups.length) {
        box = getBoundingClientRectFromMultiple(headerGroups[swapIndex]);
        if (e.clientX > box.left + window.scrollX + (box.width / 2)) {
          swapElement = columns[dragIndex];
          columns.splice(dragIndex, 1);
          columns.splice(swapIndex, 0, swapElement);
          forcePopulation = true;
          swapDone = true;
        }
      }
    }

    // Write back change to storage
    if (swapDone) {
      settings.columnOrder = columns
      writeStorage("columnOrder", JSON.stringify(columns));
    }

  }

  const mouseDownHandler = function(e) {
    var target = e.target;
    if (target.tagName.toLowerCase() != "td")
      target = target.parentElement;

    // Used to check if a dragging has ever happened
    wasDragged = false;

    // Create new element which will be displayed as the dragged column
    draggingElement = document.createElement("div")
    draggingElement.classList.add("dragging");
    draggingElement.style.display = "none";
    draggingElement.style.position = "absolute";
    draggingElement.style.overflow = "hidden";

    // Get bomhead and bombody elements
    const bh = document.getElementById("bomhead");
    const bb = document.getElementById("bombody");

    // Get all compound headers for the current column
    var compoundHeaders;
    if (target.classList.contains("bom-checkbox")) {
      compoundHeaders = Array.from(bh.querySelectorAll("th.bom-checkbox"));
    } else {
      compoundHeaders = [target];
    }

    // Create new table which will display the column
    var newTable = document.createElement("table");
    newTable.classList.add("bom");
    newTable.style.background = "white";
    draggingElement.append(newTable);

    // Create new header element
    var newHeader = document.createElement("thead");
    newTable.append(newHeader);

    // Set up array for storing all placeholder elements
    placeHolderElements = [];

    // Add all compound headers to the new thead element and placeholders
    compoundHeaders.forEach(function(h) {
      clone = cloneElementWithDimensions(h);
      newHeader.append(clone);
      placeHolderElements.push(clone);
    });

    // Create new body element
    var newBody = document.createElement("tbody");
    newTable.append(newBody);

    // Get indices for compound headers
    var idxs = compoundHeaders.map(e => getBomTableHeaderIndex(e));

    // For each row in the BOM body...
    var rows = bb.querySelectorAll("tr");
    rows.forEach(function(row) {
      // ..get the cells for the compound column
      const tds = row.querySelectorAll("td");
      var copytds = idxs.map(i => tds[i]);
      // Add them to the new element and the placeholders
      var newRow = document.createElement("tr");
      copytds.forEach(function(td) {
        clone = cloneElementWithDimensions(td);
        newRow.append(clone);
        placeHolderElements.push(clone);
      });
      newBody.append(newRow);
    });

    // Compute width for compound header
    var width = compoundHeaders.reduce((acc, x) => acc + x.clientWidth, 0);
    draggingElement.style.width = `${width}px`;

    // Insert the new dragging element and disable selection on BOM
    bom.insertBefore(draggingElement, null);
    bom.style.userSelect = "none";

    // Determine the mouse position offset
    xOffset = e.screenX - compoundHeaders.reduce((acc, x) => Math.min(acc, x.offsetLeft), compoundHeaders[0].offsetLeft);
    yOffset = e.screenY - compoundHeaders[0].offsetTop;

    // Get name for the column in settings.columnOrder
    dragName = getColumnOrderName(target);

    // Change text and class for placeholder elements
    placeHolderElements = placeHolderElements.map(function(e) {
      newElem = cloneElementWithDimensions(e);
      newElem.textContent = "";
      newElem.classList.add("placeholder");
      return newElem;
    });

    // On next mouse move, the whole BOM needs to be redrawn to show the placeholders
    forcePopulation = true;

    // Add listeners for move and up on mouse
    document.addEventListener('mousemove', mouseMoveHandler);
    document.addEventListener('mouseup', mouseUpHandler);
  }

  // In netlist mode, there is nothing to reorder
  if (settings.bommode === "netlist")
    return;

  // Add mouseDownHandler to every column except the numCol
  bom.querySelectorAll("th")
    .forEach(function(head) {
      if (!head.classList.contains("numCol")) {
        head.onmousedown = mouseDownHandler;
      }
    });

}

function getBoundingClientRectFromMultiple(elements) {
  var elems = Array.from(elements);

  if (elems.length == 0)
    return null;

  var box = elems.shift()
    .getBoundingClientRect();

  elems.forEach(function(elem) {
    var elembox = elem.getBoundingClientRect();
    box.left = Math.min(elembox.left, box.left);
    box.top = Math.min(elembox.top, box.top);
    box.width += elembox.width;
    box.height = Math.max(elembox.height, box.height);
  });

  return box;
}

function cloneElementWithDimensions(elem) {
  var newElem = elem.cloneNode(true);
  newElem.style.height = window.getComputedStyle(elem).height;
  newElem.style.width = window.getComputedStyle(elem).width;
  return newElem;
}

function getBomTableHeaderIndex(elem) {
  const bh = document.getElementById('bomhead');
  const ths = Array.from(bh.querySelectorAll("th"));
  return ths.indexOf(elem);
}

function getColumnOrderName(elem) {
  var cname = elem.getAttribute("col_name");
  if (cname === "bom-checkbox")
    return "checkboxes";
  else
    return cname;
}

function resizableGrid(tablehead) {
  var cols = tablehead.firstElementChild.children;
  var rowWidth = tablehead.offsetWidth;

  for (var i = 1; i < cols.length; i++) {
    if (cols[i].classList.contains("bom-checkbox"))
      continue;
    cols[i].style.width = ((cols[i].clientWidth - paddingDiff(cols[i])) * 100 / rowWidth) + '%';
  }

  for (var i = 1; i < cols.length - 1; i++) {
    var div = document.createElement('div');
    div.className = "column-width-handle";
    cols[i].appendChild(div);
    setListeners(div);
  }

  function setListeners(div) {
    var startX, curCol, nxtCol, curColWidth, nxtColWidth, rowWidth;

    div.addEventListener('mousedown', function(e) {
      e.preventDefault();
      e.stopPropagation();

      curCol = e.target.parentElement;
      nxtCol = curCol.nextElementSibling;
      startX = e.pageX;

      var padding = paddingDiff(curCol);

      rowWidth = curCol.parentElement.offsetWidth;
      curColWidth = curCol.clientWidth - padding;
      nxtColWidth = nxtCol.clientWidth - padding;
    });

    document.addEventListener('mousemove', function(e) {
      if (startX) {
        var diffX = e.pageX - startX;
        diffX = -Math.min(-diffX, curColWidth - 20);
        diffX = Math.min(diffX, nxtColWidth - 20);

        curCol.style.width = ((curColWidth + diffX) * 100 / rowWidth) + '%';
        nxtCol.style.width = ((nxtColWidth - diffX) * 100 / rowWidth) + '%';
        console.log(`${curColWidth + nxtColWidth} ${(curColWidth + diffX) * 100 / rowWidth + (nxtColWidth - diffX) * 100 / rowWidth}`);
      }
    });

    document.addEventListener('mouseup', function(e) {
      curCol = undefined;
      nxtCol = undefined;
      startX = undefined;
      nxtColWidth = undefined;
      curColWidth = undefined
    });
  }

  function paddingDiff(col) {

    if (getStyleVal(col, 'box-sizing') == 'border-box') {
      return 0;
    }

    var padLeft = getStyleVal(col, 'padding-left');
    var padRight = getStyleVal(col, 'padding-right');
    return (parseInt(padLeft) + parseInt(padRight));

  }

  function getStyleVal(elm, css) {
    return (window.getComputedStyle(elm, null).getPropertyValue(css))
  }
}

///////////////////////////////////////////////

///////////////////////////////////////////////
/* DOM manipulation and misc code */

var bomsplit;
var canvassplit;
var initDone = false;
var bomSortFunction = null;
var currentSortColumn = null;
var currentSortOrder = null;
var currentHighlightedRowId;
var highlightHandlers = [];
var footprintIndexToHandler = {};
var netsToHandler = {};
var markedFootprints = new Set();
var highlightedFootprints = [];
var highlightedNet = null;
var lastClicked;

function dbg(html) {
  dbgdiv.innerHTML = html;
}

function redrawIfInitDone() {
  if (initDone) {
    redrawCanvas(allcanvas.front);
    redrawCanvas(allcanvas.back);
  }
}

function padsVisible(value) {
  writeStorage("padsVisible", value);
  settings.renderPads = value;
  redrawIfInitDone();
}

function referencesVisible(value) {
  writeStorage("referencesVisible", value);
  settings.renderReferences = value;
  redrawIfInitDone();
}

function valuesVisible(value) {
  writeStorage("valuesVisible", value);
  settings.renderValues = value;
  redrawIfInitDone();
}

function tracksVisible(value) {
  writeStorage("tracksVisible", value);
  settings.renderTracks = value;
  redrawIfInitDone();
}

function zonesVisible(value) {
  writeStorage("zonesVisible", value);
  settings.renderZones = value;
  redrawIfInitDone();
}

function dnpOutline(value) {
  writeStorage("dnpOutline", value);
  settings.renderDnpOutline = value;
  redrawIfInitDone();
}

function setDarkMode(value) {
  if (value) {
    topmostdiv.classList.add("dark");
  } else {
    topmostdiv.classList.remove("dark");
  }
  writeStorage("darkmode", value);
  settings.darkMode = value;
  redrawIfInitDone();
  if (initDone) {
    populateBomTable();
  }
}

function setShowBOMColumn(field, value) {
  if (field === "references") {
    var rl = document.getElementById("reflookup");
    rl.disabled = !value;
    if (!value) {
      rl.value = "";
      updateRefLookup("");
    }
  }

  var n = settings.hiddenColumns.indexOf(field);
  if (value) {
    if (n != -1) {
      settings.hiddenColumns.splice(n, 1);
    }
  } else {
    if (n == -1) {
      settings.hiddenColumns.push(field);
    }
  }

  writeStorage("hiddenColumns", JSON.stringify(settings.hiddenColumns));

  if (initDone) {
    populateBomTable();
  }

  redrawIfInitDone();
}


function setFullscreen(value) {
  if (value) {
    document.documentElement.requestFullscreen();
  } else {
    document.exitFullscreen();
  }
}

function fabricationVisible(value) {
  writeStorage("fabricationVisible", value);
  settings.renderFabrication = value;
  redrawIfInitDone();
}

function silkscreenVisible(value) {
  writeStorage("silkscreenVisible", value);
  settings.renderSilkscreen = value;
  redrawIfInitDone();
}

function setHighlightPin1(value) {
  writeStorage("highlightpin1", value);
  settings.highlightpin1 = value;
  redrawIfInitDone();
}

function setHighlightRowOnClick(value) {
  settings.highlightRowOnClick = value;
  writeStorage("highlightRowOnClick", value);
  if (initDone) {
    populateBomTable();
  }
}

function getStoredCheckboxRefs(checkbox) {
  function convert(ref) {
    var intref = parseInt(ref);
    if (isNaN(intref)) {
      for (var i = 0; i < pcbdata.footprints.length; i++) {
        if (pcbdata.footprints[i].ref == ref) {
          return i;
        }
      }
      return -1;
    } else {
      return intref;
    }
  }
  if (!(checkbox in settings.checkboxStoredRefs)) {
    var val = readStorage("checkbox_" + checkbox);
    settings.checkboxStoredRefs[checkbox] = val ? val : "";
  }
  if (!settings.checkboxStoredRefs[checkbox]) {
    return new Set();
  } else {
    return new Set(settings.checkboxStoredRefs[checkbox].split(",").map(r => convert(r)).filter(a => a >= 0));
  }
}

function getCheckboxState(checkbox, references) {
  var storedRefsSet = getStoredCheckboxRefs(checkbox);
  var currentRefsSet = new Set(references.map(r => r[1]));
  // Get difference of current - stored
  var difference = new Set(currentRefsSet);
  for (ref of storedRefsSet) {
    difference.delete(ref);
  }
  if (difference.size == 0) {
    // All the current refs are stored
    return "checked";
  } else if (difference.size == currentRefsSet.size) {
    // None of the current refs are stored
    return "unchecked";
  } else {
    // Some of the refs are stored
    return "indeterminate";
  }
}

function setBomCheckboxState(checkbox, element, references) {
  var state = getCheckboxState(checkbox, references);
  element.checked = (state == "checked");
  element.indeterminate = (state == "indeterminate");
}

function createCheckboxHandlers(input, checkbox, references, row) {
  var clickHandler = () => {
    refsSet = getStoredCheckboxRefs(checkbox);
    var markWhenChecked = settings.markWhenChecked == checkbox;
    eventArgs = {
      checkbox: checkbox,
      refs: references,
    }
    if (input.checked) {
      // checkbox ticked
      for (var ref of references) {
        refsSet.add(ref[1]);
      }
      if (markWhenChecked) {
        row.classList.add("checked");
        for (var ref of references) {
          markedFootprints.add(ref[1]);
        }
        drawHighlights();
      }
      eventArgs.state = 'checked';
    } else {
      // checkbox unticked
      for (var ref of references) {
        refsSet.delete(ref[1]);
      }
      if (markWhenChecked) {
        row.classList.remove("checked");
        for (var ref of references) {
          markedFootprints.delete(ref[1]);
        }
        drawHighlights();
      }
      eventArgs.state = 'unchecked';
    }
    settings.checkboxStoredRefs[checkbox] = [...refsSet].join(",");
    writeStorage("checkbox_" + checkbox, settings.checkboxStoredRefs[checkbox]);
    updateCheckboxStats(checkbox);
    EventHandler.emitEvent(IBOM_EVENT_TYPES.CHECKBOX_CHANGE_EVENT, eventArgs);
  }

  return [
    (e) => {
      clickHandler();
    },
    (e) => {
      e.preventDefault();
      if (row.onmousemove) row.onmousemove();
    },
    (e) => {
      e.preventDefault();
      input.checked = !input.checked;
      input.indeterminate = false;
      clickHandler();
    }
  ];
}

function clearHighlightedFootprints() {
  if (currentHighlightedRowId) {
    document.getElementById(currentHighlightedRowId).classList.remove("highlighted");
    currentHighlightedRowId = null;
    highlightedFootprints = [];
    highlightedNet = null;
  }
}

function createRowHighlightHandler(rowid, refs, net) {
  return function () {
    if (currentHighlightedRowId) {
      if (currentHighlightedRowId == rowid) {
        return;
      }
      document.getElementById(currentHighlightedRowId).classList.remove("highlighted");
    }
    document.getElementById(rowid).classList.add("highlighted");
    currentHighlightedRowId = rowid;
    highlightedFootprints = refs ? refs.map(r => r[1]) : [];
    highlightedNet = net;
    drawHighlights();
    EventHandler.emitEvent(
      IBOM_EVENT_TYPES.HIGHLIGHT_EVENT, {
      rowid: rowid,
      refs: refs,
      net: net
    });
  }
}

function updateNetColors() {
  writeStorage("netColors", JSON.stringify(settings.netColors));
  redrawIfInitDone();
}

function netColorChangeHandler(net) {
  return (event) => {
    settings.netColors[net] = event.target.value;
    updateNetColors();
  }
}

function netColorRightClick(net) {
  return (event) => {
    if (event.button == 2) {
      event.preventDefault();
      event.stopPropagation();

      var style = getComputedStyle(topmostdiv);
      var defaultNetColor = style.getPropertyValue('--track-color').trim();
      event.target.value = defaultNetColor;
      delete settings.netColors[net];
      updateNetColors();
    }
  }
}

function entryMatches(entry) {
  if (settings.bommode == "netlist") {
    // entry is just a net name
    return entry.toLowerCase().indexOf(filter) >= 0;
  }
  // check refs
  if (!settings.hiddenColumns.includes("References")) {
    for (var ref of entry) {
      if (ref[0].toLowerCase().indexOf(filter) >= 0) {
        return true;
      }
    }
  }
  // check fields
  for (var i in config.fields) {
    var f = config.fields[i];
    if (!settings.hiddenColumns.includes(f)) {
      for (var ref of entry) {
        if (String(pcbdata.bom.fields[ref[1]][i]).toLowerCase().indexOf(filter) >= 0) {
          return true;
        }
      }
    }
  }
  return false;
}

function findRefInEntry(entry) {
  return entry.filter(r => r[0].toLowerCase() == reflookup);
}

function highlightFilter(s) {
  if (!filter) {
    return s;
  }
  var parts = s.toLowerCase().split(filter);
  if (parts.length == 1) {
    return s;
  }
  var r = "";
  var pos = 0;
  for (var i in parts) {
    if (i > 0) {
      r += '<mark class="highlight">' +
        s.substring(pos, pos + filter.length) +
        '</mark>';
      pos += filter.length;
    }
    r += s.substring(pos, pos + parts[i].length);
    pos += parts[i].length;
  }
  return r;
}

function getBomListByLayer(layer) {
  switch (layer) {
    case 'F': return pcbdata.bom.F.slice();
    case 'B': return pcbdata.bom.B.slice();
    case 'FB': return pcbdata.bom.both.slice();
  }
  return [];
}

function getSelectedBomList() {
  if (settings.bommode == "netlist") {
    return pcbdata.nets.slice();
  }
  var out = getBomListByLayer(settings.canvaslayout);

  if (settings.bommode == "ungrouped") {
    // expand bom table
    var expandedTable = [];
    for (var bomentry of out) {
      for (var ref of bomentry) {
        expandedTable.push([ref]);
      }
    }
    return expandedTable;
  }

  return out;
}

function checkboxSetUnsetAllHandler(checkboxname) {
  return function () {
    var checkboxnum = 0;
    while (checkboxnum < settings.checkboxes.length &&
      settings.checkboxes[checkboxnum].toLowerCase() != checkboxname.toLowerCase()) {
      checkboxnum++;
    }
    if (checkboxnum >= settings.checkboxes.length) {
      return;
    }
    var allset = true;
    var checkbox;
    var row;
    for (row of bombody.childNodes) {
      checkbox = row.childNodes[checkboxnum + 1].childNodes[0];
      if (!checkbox.checked || checkbox.indeterminate) {
        allset = false;
        break;
      }
    }
    for (row of bombody.childNodes) {
      checkbox = row.childNodes[checkboxnum + 1].childNodes[0];
      checkbox.checked = !allset;
      checkbox.indeterminate = false;
      checkbox.onchange();
    }
  }
}

function createColumnHeader(name, cls, comparator, is_checkbox = false) {
  var th = document.createElement("TH");
  th.innerHTML = name;
  th.classList.add(cls);
  if (is_checkbox)
    th.setAttribute("col_name", "bom-checkbox");
  else
    th.setAttribute("col_name", name);
  var span = document.createElement("SPAN");
  span.classList.add("sortmark");
  span.classList.add("none");
  th.appendChild(span);
  var spacer = document.createElement("div");
  spacer.className = "column-spacer";
  th.appendChild(spacer);
  spacer.onclick = function () {
    if (currentSortColumn && th !== currentSortColumn) {
      // Currently sorted by another column
      currentSortColumn.childNodes[1].classList.remove(currentSortOrder);
      currentSortColumn.childNodes[1].classList.add("none");
      currentSortColumn = null;
      currentSortOrder = null;
    }
    if (currentSortColumn && th === currentSortColumn) {
      // Already sorted by this column
      if (currentSortOrder == "asc") {
        // Sort by this column, descending order
        bomSortFunction = function (a, b) {
          return -comparator(a, b);
        }
        currentSortColumn.childNodes[1].classList.remove("asc");
        currentSortColumn.childNodes[1].classList.add("desc");
        currentSortOrder = "desc";
      } else {
        // Unsort
        bomSortFunction = null;
        currentSortColumn.childNodes[1].classList.remove("desc");
        currentSortColumn.childNodes[1].classList.add("none");
        currentSortColumn = null;
        currentSortOrder = null;
      }
    } else {
      // Sort by this column, ascending order
      bomSortFunction = comparator;
      currentSortColumn = th;
      currentSortColumn.childNodes[1].classList.remove("none");
      currentSortColumn.childNodes[1].classList.add("asc");
      currentSortOrder = "asc";
    }
    populateBomBody();
  }
  if (is_checkbox) {
    spacer.onclick = fancyDblClickHandler(
      spacer, spacer.onclick, checkboxSetUnsetAllHandler(name));
  }
  return th;
}

function populateBomHeader(placeHolderColumn = null, placeHolderElements = null) {
  while (bomhead.firstChild) {
    bomhead.removeChild(bomhead.firstChild);
  }
  var tr = document.createElement("TR");
  var th = document.createElement("TH");
  th.classList.add("numCol");

  var vismenu = document.createElement("div");
  vismenu.id = "vismenu";
  vismenu.classList.add("menu");

  var visbutton = document.createElement("div");
  visbutton.classList.add("visbtn");
  visbutton.classList.add("hideonprint");

  var viscontent = document.createElement("div");
  viscontent.classList.add("menu-content");
  viscontent.id = "vismenu-content";

  settings.columnOrder.forEach(column => {
    if (typeof column !== "string")
      return;

    // Skip empty columns
    if (column === "checkboxes" && settings.checkboxes.length == 0)
      return;
    else if (column === "Quantity" && settings.bommode == "ungrouped")
      return;

    var label = document.createElement("label");
    label.classList.add("menu-label");

    var input = document.createElement("input");
    input.classList.add("visibility_checkbox");
    input.type = "checkbox";
    input.onchange = function (e) {
      setShowBOMColumn(column, e.target.checked)
    };
    input.checked = !(settings.hiddenColumns.includes(column));

    label.appendChild(input);
    if (column.length > 0)
      label.append(column[0].toUpperCase() + column.slice(1));

    viscontent.appendChild(label);
  });

  viscontent.childNodes[0].classList.add("menu-label-top");

  vismenu.appendChild(visbutton);
  if (settings.bommode != "netlist") {
    vismenu.appendChild(viscontent);
    th.appendChild(vismenu);
  }
  tr.appendChild(th);

  var checkboxCompareClosure = function (checkbox) {
    return (a, b) => {
      var stateA = getCheckboxState(checkbox, a);
      var stateB = getCheckboxState(checkbox, b);
      if (stateA > stateB) return -1;
      if (stateA < stateB) return 1;
      return 0;
    }
  }
  var stringFieldCompareClosure = function (fieldIndex) {
    return (a, b) => {
      var fa = pcbdata.bom.fields[a[0][1]][fieldIndex];
      var fb = pcbdata.bom.fields[b[0][1]][fieldIndex];
      if (fa != fb) return fa > fb ? 1 : -1;
      else return 0;
    }
  }
  var referenceRegex = /(?<prefix>[^0-9]+)(?<number>[0-9]+)/;
  var compareRefs = (a, b) => {
    var ra = referenceRegex.exec(a);
    var rb = referenceRegex.exec(b);
    if (ra === null || rb === null) {
      if (a != b) return a > b ? 1 : -1;
      return 0;
    } else {
      if (ra.groups.prefix != rb.groups.prefix) {
        return ra.groups.prefix > rb.groups.prefix ? 1 : -1;
      }
      if (ra.groups.number != rb.groups.number) {
        return parseInt(ra.groups.number) > parseInt(rb.groups.number) ? 1 : -1;
      }
      return 0;
    }
  }
  if (settings.bommode == "netlist") {
    tr.appendChild(createColumnHeader("Net name", "bom-netname", (a, b) => {
      if (a > b) return -1;
      if (a < b) return 1;
      return 0;
    }));
    tr.appendChild(createColumnHeader("Color", "bom-color", (a, b) => {
      return 0;
    }));
  } else {
    // Filter hidden columns
    var columns = settings.columnOrder.filter(e => !settings.hiddenColumns.includes(e));
    var valueIndex = config.fields.indexOf("Value");
    var footprintIndex = config.fields.indexOf("Footprint");
    columns.forEach((column) => {
      if (column === placeHolderColumn) {
        var n = 1;
        if (column === "checkboxes")
          n = settings.checkboxes.length;
        for (i = 0; i < n; i++) {
          td = placeHolderElements.shift();
          tr.appendChild(td);
        }
        return;
      } else if (column === "checkboxes") {
        for (var checkbox of settings.checkboxes) {
          th = createColumnHeader(
            checkbox, "bom-checkbox", checkboxCompareClosure(checkbox), true);
          tr.appendChild(th);
        }
      } else if (column === "References") {
        tr.appendChild(createColumnHeader("References", "references", (a, b) => {
          var i = 0;
          while (i < a.length && i < b.length) {
            if (a[i][0] != b[i][0]) return compareRefs(a[i][0], b[i][0]);
            i++;
          }
          return a.length - b.length;
        }));
      } else if (column === "Value") {
        tr.appendChild(createColumnHeader("Value", "value", (a, b) => {
          var ra = a[0][1], rb = b[0][1];
          return valueCompare(
            pcbdata.bom.parsedValues[ra], pcbdata.bom.parsedValues[rb],
            pcbdata.bom.fields[ra][valueIndex], pcbdata.bom.fields[rb][valueIndex]);
        }));
        return;
      } else if (column === "Footprint") {
        tr.appendChild(createColumnHeader(
          "Footprint", "footprint", stringFieldCompareClosure(footprintIndex)));
      } else if (column === "Quantity" && settings.bommode == "grouped") {
        tr.appendChild(createColumnHeader("Quantity", "quantity", (a, b) => {
          return a.length - b.length;
        }));
      } else {
        // Other fields
        var i = config.fields.indexOf(column);
        if (i < 0)
          return;
        tr.appendChild(createColumnHeader(
          column, `field${i + 1}`, stringFieldCompareClosure(i)));
      }
    });
  }
  bomhead.appendChild(tr);
}

function populateBomBody(placeholderColumn = null, placeHolderElements = null) {
  const urlRegex = /^(https?:\/\/[^\s\/$.?#][^\s]*|file:\/\/([a-zA-Z]:|\/)[^\x00]+)$/;
  while (bom.firstChild) {
    bom.removeChild(bom.firstChild);
  }
  highlightHandlers = [];
  footprintIndexToHandler = {};
  netsToHandler = {};
  currentHighlightedRowId = null;
  var first = true;
  var style = getComputedStyle(topmostdiv);
  var defaultNetColor = style.getPropertyValue('--track-color').trim();

  bomtable = getSelectedBomList();

  if (bomSortFunction) {
    bomtable = bomtable.sort(bomSortFunction);
  }
  for (var i in bomtable) {
    var bomentry = bomtable[i];
    if (filter && !entryMatches(bomentry)) {
      continue;
    }
    var references = null;
    var netname = null;
    var tr = document.createElement("TR");
    var td = document.createElement("TD");
    var rownum = +i + 1;
    tr.id = "bomrow" + rownum;
    td.textContent = rownum;
    tr.appendChild(td);
    if (settings.bommode == "netlist") {
      netname = bomentry;
      td = document.createElement("TD");
      td.innerHTML = highlightFilter(netname ? netname : "&lt;no net&gt;");
      tr.appendChild(td);
      var color = settings.netColors[netname] || defaultNetColor;
      td = document.createElement("TD");
      var colorBox = document.createElement("INPUT");
      colorBox.type = "color";
      colorBox.value = color;
      colorBox.onchange = netColorChangeHandler(netname);
      colorBox.onmouseup = netColorRightClick(netname);
      colorBox.oncontextmenu = (e) => e.preventDefault();
      td.appendChild(colorBox);
      td.classList.add("color-column");
      tr.appendChild(td);
    } else {
      if (reflookup) {
        references = findRefInEntry(bomentry);
        if (references.length == 0) {
          continue;
        }
      } else {
        references = bomentry;
      }
      // Filter hidden columns
      var columns = settings.columnOrder.filter(e => !settings.hiddenColumns.includes(e));
      columns.forEach((column) => {
        if (column === placeholderColumn) {
          var n = 1;
          if (column === "checkboxes")
            n = settings.checkboxes.length;
          for (i = 0; i < n; i++) {
            td = placeHolderElements.shift();
            tr.appendChild(td);
          }
          return;
        } else if (column === "checkboxes") {
          for (var checkbox of settings.checkboxes) {
            if (checkbox) {
              td = document.createElement("TD");
              var input = document.createElement("input");
              input.type = "checkbox";
              [input.onchange, td.ontouchstart, td.ontouchend] = createCheckboxHandlers(input, checkbox, references, tr);
              setBomCheckboxState(checkbox, input, references);
              if (input.checked && settings.markWhenChecked == checkbox) {
                tr.classList.add("checked");
              }
              td.appendChild(input);
              tr.appendChild(td);
            }
          }
        } else if (column === "References") {
          td = document.createElement("TD");
          td.innerHTML = highlightFilter(references.map(r => r[0]).join(", "));
          tr.appendChild(td);
        } else if (column === "Quantity" && settings.bommode == "grouped") {
          // Quantity
          td = document.createElement("TD");
          td.textContent = references.length;
          tr.appendChild(td);
        } else {
          // All the other fields
          var field_index = config.fields.indexOf(column)
          if (field_index < 0)
            return;
          var valueSet = new Set();
          references.map(r => r[1]).forEach((id) => valueSet.add(pcbdata.bom.fields[id][field_index]));
          td = document.createElement("TD");
          var output = new Array();
          for (let item of valueSet) {
            const visible = highlightFilter(String(item));
            if (typeof item === 'string' && item.match(urlRegex)) {
              output.push(`<a href="${item}" target="_blank">${visible}</a>`);
            } else {
              output.push(visible);
            }
          }
          td.innerHTML = output.join(", ");
          tr.appendChild(td);
        }
      });
    }
    bom.appendChild(tr);
    var handler = createRowHighlightHandler(tr.id, references, netname);
    if (settings.highlightRowOnClick) {
      tr.onmousedown = handler;
    } else {
      tr.onmousemove = handler;
    }
    highlightHandlers.push({
      id: tr.id,
      handler: handler,
    });
    if (references !== null) {
      for (var refIndex of references.map(r => r[1])) {
        footprintIndexToHandler[refIndex] = handler;
      }
    }
    if (netname !== null) {
      netsToHandler[netname] = handler;
    }
    if ((filter || reflookup) && first) {
      handler();
      first = false;
    }
  }
  EventHandler.emitEvent(
    IBOM_EVENT_TYPES.BOM_BODY_CHANGE_EVENT, {
    filter: filter,
    reflookup: reflookup,
    checkboxes: settings.checkboxes,
    bommode: settings.bommode,
  });
}

function highlightPreviousRow() {
  if (!currentHighlightedRowId) {
    highlightHandlers[highlightHandlers.length - 1].handler();
  } else {
    if (highlightHandlers.length > 1 &&
      highlightHandlers[0].id == currentHighlightedRowId) {
      highlightHandlers[highlightHandlers.length - 1].handler();
    } else {
      for (var i = 0; i < highlightHandlers.length - 1; i++) {
        if (highlightHandlers[i + 1].id == currentHighlightedRowId) {
          highlightHandlers[i].handler();
          break;
        }
      }
    }
  }
  smoothScrollToRow(currentHighlightedRowId);
}

function highlightNextRow() {
  if (!currentHighlightedRowId) {
    highlightHandlers[0].handler();
  } else {
    if (highlightHandlers.length > 1 &&
      highlightHandlers[highlightHandlers.length - 1].id == currentHighlightedRowId) {
      highlightHandlers[0].handler();
    } else {
      for (var i = 1; i < highlightHandlers.length; i++) {
        if (highlightHandlers[i - 1].id == currentHighlightedRowId) {
          highlightHandlers[i].handler();
          break;
        }
      }
    }
  }
  smoothScrollToRow(currentHighlightedRowId);
}

function populateBomTable() {
  populateBomHeader();
  populateBomBody();
  setBomHandlers();
  resizableGrid(bomhead);
}

function footprintsClicked(footprintIndexes) {
  var lastClickedIndex = footprintIndexes.indexOf(lastClicked);
  for (var i = 1; i <= footprintIndexes.length; i++) {
    var refIndex = footprintIndexes[(lastClickedIndex + i) % footprintIndexes.length];
    if (refIndex in footprintIndexToHandler) {
      lastClicked = refIndex;
      footprintIndexToHandler[refIndex]();
      smoothScrollToRow(currentHighlightedRowId);
      break;
    }
  }
}

function netClicked(net) {
  if (net in netsToHandler) {
    netsToHandler[net]();
    smoothScrollToRow(currentHighlightedRowId);
  } else {
    clearHighlightedFootprints();
    highlightedNet = net;
    drawHighlights();
  }
}

function updateFilter(input) {
  filter = input.toLowerCase();
  populateBomTable();
}

function updateRefLookup(input) {
  reflookup = input.toLowerCase();
  populateBomTable();
}

function changeCanvasLayout(layout) {
  document.getElementById("fl-btn").classList.remove("depressed");
  document.getElementById("fb-btn").classList.remove("depressed");
  document.getElementById("bl-btn").classList.remove("depressed");
  switch (layout) {
    case 'F':
      document.getElementById("fl-btn").classList.add("depressed");
      if (settings.bomlayout != "bom-only") {
        canvassplit.collapse(1);
      }
      break;
    case 'B':
      document.getElementById("bl-btn").classList.add("depressed");
      if (settings.bomlayout != "bom-only") {
        canvassplit.collapse(0);
      }
      break;
    default:
      document.getElementById("fb-btn").classList.add("depressed");
      if (settings.bomlayout != "bom-only") {
        canvassplit.setSizes([50, 50]);
      }
  }
  settings.canvaslayout = layout;
  writeStorage("canvaslayout", layout);
  resizeAll();
  changeBomMode(settings.bommode);
}

function populateMetadata() {
  document.getElementById("title").innerHTML = pcbdata.metadata.title;
  document.getElementById("revision").innerHTML = "Rev: " + pcbdata.metadata.revision;
  document.getElementById("company").innerHTML = pcbdata.metadata.company;
  document.getElementById("filedate").innerHTML = pcbdata.metadata.date;
  if (pcbdata.metadata.title != "") {
    document.title = pcbdata.metadata.title + " BOM";
  }
  // Calculate board stats
  var fp_f = 0,
    fp_b = 0,
    pads_f = 0,
    pads_b = 0,
    pads_th = 0;
  for (var i = 0; i < pcbdata.footprints.length; i++) {
    if (pcbdata.bom.skipped.includes(i)) continue;
    var mod = pcbdata.footprints[i];
    if (mod.layer == "F") {
      fp_f++;
    } else {
      fp_b++;
    }
    for (var pad of mod.pads) {
      if (pad.type == "th") {
        pads_th++;
      } else {
        if (pad.layers.includes("F")) {
          pads_f++;
        }
        if (pad.layers.includes("B")) {
          pads_b++;
        }
      }
    }
  }
  document.getElementById("stats-components-front").innerHTML = fp_f;
  document.getElementById("stats-components-back").innerHTML = fp_b;
  document.getElementById("stats-components-total").innerHTML = fp_f + fp_b;
  document.getElementById("stats-groups-front").innerHTML = pcbdata.bom.F.length;
  document.getElementById("stats-groups-back").innerHTML = pcbdata.bom.B.length;
  document.getElementById("stats-groups-total").innerHTML = pcbdata.bom.both.length;
  document.getElementById("stats-smd-pads-front").innerHTML = pads_f;
  document.getElementById("stats-smd-pads-back").innerHTML = pads_b;
  document.getElementById("stats-smd-pads-total").innerHTML = pads_f + pads_b;
  document.getElementById("stats-th-pads").innerHTML = pads_th;
  // Update version string
  document.getElementById("github-link").innerHTML = "InteractiveHtmlBom&nbsp;" +
    /^v\d+\.\d+/.exec(pcbdata.ibom_version)[0];
}

function changeBomLayout(layout) {
  document.getElementById("bom-btn").classList.remove("depressed");
  document.getElementById("lr-btn").classList.remove("depressed");
  document.getElementById("tb-btn").classList.remove("depressed");
  switch (layout) {
    case 'bom-only':
      document.getElementById("bom-btn").classList.add("depressed");
      if (bomsplit) {
        bomsplit.destroy();
        bomsplit = null;
        canvassplit.destroy();
        canvassplit = null;
      }
      document.getElementById("frontcanvas").style.display = "none";
      document.getElementById("backcanvas").style.display = "none";
      document.getElementById("topmostdiv").style.height = "";
      document.getElementById("topmostdiv").style.display = "block";
      break;
    case 'top-bottom':
      document.getElementById("tb-btn").classList.add("depressed");
      document.getElementById("frontcanvas").style.display = "";
      document.getElementById("backcanvas").style.display = "";
      document.getElementById("topmostdiv").style.height = "100%";
      document.getElementById("topmostdiv").style.display = "flex";
      document.getElementById("bomdiv").classList.remove("split-horizontal");
      document.getElementById("canvasdiv").classList.remove("split-horizontal");
      document.getElementById("frontcanvas").classList.add("split-horizontal");
      document.getElementById("backcanvas").classList.add("split-horizontal");
      if (bomsplit) {
        bomsplit.destroy();
        bomsplit = null;
        canvassplit.destroy();
        canvassplit = null;
      }
      bomsplit = Split(['#bomdiv', '#canvasdiv'], {
        sizes: [50, 50],
        onDragEnd: resizeAll,
        direction: "vertical",
        gutterSize: 5
      });
      canvassplit = Split(['#frontcanvas', '#backcanvas'], {
        sizes: [50, 50],
        gutterSize: 5,
        onDragEnd: resizeAll
      });
      break;
    case 'left-right':
      document.getElementById("lr-btn").classList.add("depressed");
      document.getElementById("frontcanvas").style.display = "";
      document.getElementById("backcanvas").style.display = "";
      document.getElementById("topmostdiv").style.height = "100%";
      document.getElementById("topmostdiv").style.display = "flex";
      document.getElementById("bomdiv").classList.add("split-horizontal");
      document.getElementById("canvasdiv").classList.add("split-horizontal");
      document.getElementById("frontcanvas").classList.remove("split-horizontal");
      document.getElementById("backcanvas").classList.remove("split-horizontal");
      if (bomsplit) {
        bomsplit.destroy();
        bomsplit = null;
        canvassplit.destroy();
        canvassplit = null;
      }
      bomsplit = Split(['#bomdiv', '#canvasdiv'], {
        sizes: [50, 50],
        onDragEnd: resizeAll,
        gutterSize: 5
      });
      canvassplit = Split(['#frontcanvas', '#backcanvas'], {
        sizes: [50, 50],
        gutterSize: 5,
        direction: "vertical",
        onDragEnd: resizeAll
      });
  }
  settings.bomlayout = layout;
  writeStorage("bomlayout", layout);
  changeCanvasLayout(settings.canvaslayout);
}

function changeBomMode(mode) {
  document.getElementById("bom-grouped-btn").classList.remove("depressed");
  document.getElementById("bom-ungrouped-btn").classList.remove("depressed");
  document.getElementById("bom-netlist-btn").classList.remove("depressed");
  var chkbxs = document.getElementsByClassName("visibility_checkbox");

  switch (mode) {
    case 'grouped':
      document.getElementById("bom-grouped-btn").classList.add("depressed");
      for (var i = 0; i < chkbxs.length; i++) {
        chkbxs[i].disabled = false;
      }
      break;
    case 'ungrouped':
      document.getElementById("bom-ungrouped-btn").classList.add("depressed");
      for (var i = 0; i < chkbxs.length; i++) {
        chkbxs[i].disabled = false;
      }
      break;
    case 'netlist':
      document.getElementById("bom-netlist-btn").classList.add("depressed");
      for (var i = 0; i < chkbxs.length; i++) {
        chkbxs[i].disabled = true;
      }
  }

  writeStorage("bommode", mode);
  if (mode != settings.bommode) {
    settings.bommode = mode;
    bomSortFunction = null;
    currentSortColumn = null;
    currentSortOrder = null;
    clearHighlightedFootprints();
  }
  populateBomTable();
}

function focusFilterField() {
  focusInputField(document.getElementById("filter"));
}

function focusRefLookupField() {
  focusInputField(document.getElementById("reflookup"));
}

function toggleBomCheckbox(bomrowid, checkboxnum) {
  if (!bomrowid || checkboxnum > settings.checkboxes.length) {
    return;
  }
  var bomrow = document.getElementById(bomrowid);
  var childNum = checkboxnum + settings.columnOrder.indexOf("checkboxes");
  var checkbox = bomrow.childNodes[childNum].childNodes[0];
  checkbox.checked = !checkbox.checked;
  checkbox.indeterminate = false;
  checkbox.onchange();
}

function checkBomCheckbox(bomrowid, checkboxname) {
  var checkboxnum = 0;
  while (checkboxnum < settings.checkboxes.length &&
    settings.checkboxes[checkboxnum].toLowerCase() != checkboxname.toLowerCase()) {
    checkboxnum++;
  }
  if (!bomrowid || checkboxnum >= settings.checkboxes.length) {
    return;
  }
  var bomrow = document.getElementById(bomrowid);
  var childNum = checkboxnum + 1 + settings.columnOrder.indexOf("checkboxes");
  var checkbox = bomrow.childNodes[childNum].childNodes[0];
  checkbox.checked = true;
  checkbox.indeterminate = false;
  checkbox.onchange();
}

function setBomCheckboxes(value) {
  writeStorage("bomCheckboxes", value);
  settings.checkboxes = value.split(",").map((e) => e.trim()).filter((e) => e);
  prepCheckboxes();
  populateMarkWhenCheckedOptions();
  setMarkWhenChecked(settings.markWhenChecked);
}

function setMarkWhenChecked(value) {
  writeStorage("markWhenChecked", value);
  settings.markWhenChecked = value;
  markedFootprints.clear();
  for (var ref of (value ? getStoredCheckboxRefs(value) : [])) {
    markedFootprints.add(ref);
  }
  populateBomTable();
  drawHighlights();
}

function prepCheckboxes() {
  var table = document.getElementById("checkbox-stats");
  while (table.childElementCount > 1) {
    table.removeChild(table.lastChild);
  }
  if (settings.checkboxes.length) {
    table.style.display = "";
  } else {
    table.style.display = "none";
  }
  for (var checkbox of settings.checkboxes) {
    var tr = document.createElement("TR");
    var td = document.createElement("TD");
    td.innerHTML = checkbox;
    tr.appendChild(td);
    td = document.createElement("TD");
    td.id = "checkbox-stats-" + checkbox;
    var progressbar = document.createElement("div");
    progressbar.classList.add("bar");
    td.appendChild(progressbar);
    var text = document.createElement("div");
    text.classList.add("text");
    td.appendChild(text);
    tr.appendChild(td);
    table.appendChild(tr);
    updateCheckboxStats(checkbox);
  }
}

function populateMarkWhenCheckedOptions() {
  var container = document.getElementById("markWhenCheckedContainer");

  if (settings.checkboxes.length == 0) {
    container.parentElement.style.display = "none";
    return;
  }

  container.innerHTML = '';
  container.parentElement.style.display = "inline-block";

  function createOption(name, displayName) {
    var id = "markWhenChecked-" + name;

    var div = document.createElement("div");
    div.classList.add("radio-container");

    var input = document.createElement("input");
    input.type = "radio";
    input.name = "markWhenChecked";
    input.value = name;
    input.id = id;
    input.onchange = () => setMarkWhenChecked(name);
    div.appendChild(input);

    // Preserve the selected element when the checkboxes change
    if (name == settings.markWhenChecked) {
      input.checked = true;
    }

    var label = document.createElement("label");
    label.innerHTML = displayName;
    label.htmlFor = id;
    div.appendChild(label);

    container.appendChild(div);
  }
  createOption("", "None");
  for (var checkbox of settings.checkboxes) {
    createOption(checkbox, checkbox);
  }
}

function updateCheckboxStats(checkbox) {
  var checked = getStoredCheckboxRefs(checkbox).size;
  var total = pcbdata.footprints.length - pcbdata.bom.skipped.length;
  var percent = checked * 100.0 / total;
  var td = document.getElementById("checkbox-stats-" + checkbox);
  td.firstChild.style.width = percent + "%";
  td.lastChild.innerHTML = checked + "/" + total + " (" + Math.round(percent) + "%)";
}

function constrain(number, min, max) {
  return Math.min(Math.max(parseInt(number), min), max);
}

document.onkeydown = function (e) {
  switch (e.key) {
    case "n":
      if (document.activeElement.type == "text") {
        return;
      }
      if (currentHighlightedRowId !== null) {
        checkBomCheckbox(currentHighlightedRowId, "placed");
        highlightNextRow();
        e.preventDefault();
      }
      break;
    case "ArrowUp":
      highlightPreviousRow();
      e.preventDefault();
      break;
    case "ArrowDown":
      highlightNextRow();
      e.preventDefault();
      break;
    case "ArrowLeft":
    case "ArrowRight":
      if (document.activeElement.type != "text") {
        e.preventDefault();
        let boardRotationElement = document.getElementById("boardRotation")
        settings.boardRotation = parseInt(boardRotationElement.value);  // degrees / 5
        if (e.key == "ArrowLeft") {
          settings.boardRotation += 3;  // 15 degrees
        }
        else {
          settings.boardRotation -= 3;
        }
        settings.boardRotation = constrain(settings.boardRotation, boardRotationElement.min, boardRotationElement.max);
        boardRotationElement.value = settings.boardRotation
        setBoardRotation(settings.boardRotation);
      }
      break;
    default:
      break;
  }
  if (e.altKey) {
    switch (e.key) {
      case "f":
        focusFilterField();
        e.preventDefault();
        break;
      case "r":
        focusRefLookupField();
        e.preventDefault();
        break;
      case "z":
        changeBomLayout("bom-only");
        e.preventDefault();
        break;
      case "x":
        changeBomLayout("left-right");
        e.preventDefault();
        break;
      case "c":
        changeBomLayout("top-bottom");
        e.preventDefault();
        break;
      case "v":
        changeCanvasLayout("F");
        e.preventDefault();
        break;
      case "b":
        changeCanvasLayout("FB");
        e.preventDefault();
        break;
      case "n":
        changeCanvasLayout("B");
        e.preventDefault();
        break;
      default:
        break;
    }
    if (e.key >= '1' && e.key <= '9') {
      toggleBomCheckbox(currentHighlightedRowId, parseInt(e.key));
      e.preventDefault();
    }
  }
}

function hideNetlistButton() {
  document.getElementById("bom-ungrouped-btn").classList.remove("middle-button");
  document.getElementById("bom-ungrouped-btn").classList.add("right-most-button");
  document.getElementById("bom-netlist-btn").style.display = "none";
}

function topToggle() {
  var top = document.getElementById("top");
  var toptoggle = document.getElementById("toptoggle");
  if (top.style.display === "none") {
    top.style.display = "flex";
    toptoggle.classList.remove("flipped");
  } else {
    top.style.display = "none";
    toptoggle.classList.add("flipped");
  }
}

window.onload = function (e) {
  initRender();
  initStorage();
  initDefaults();
  initUtils();
  cleanGutters();
  populateMetadata();
  dbgdiv = document.getElementById("dbg");
  bom = document.getElementById("bombody");
  bomhead = document.getElementById("bomhead");
  filter = "";
  reflookup = "";
  if (!("nets" in pcbdata)) {
    hideNetlistButton();
  }
  initDone = true;
  setBomCheckboxes(document.getElementById("bomCheckboxes").value);
  // Triggers render
  changeBomLayout(settings.bomlayout);

  // Users may leave fullscreen without touching the checkbox. Uncheck.
  document.addEventListener('fullscreenchange', () => {
    if (!document.fullscreenElement)
      document.getElementById('fullscreenCheckbox').checked = false;
  });
}

window.onresize = resizeAll;
window.matchMedia("print").addListener(resizeAll);

///////////////////////////////////////////////

///////////////////////////////////////////////
// EventHandler.registerCallback(IBOM_EVENT_TYPES.BOM_BODY_CHANGE_EVENT, () => {
//     for(var tr of bom.childNodes) {
//         tr.onclick = tr.onmousemove;
//         tr.onmousemove = null;
//     };
// });

///////////////////////////////////////////////
  </script>
</head>

<body>

<div id="topmostdiv" class="topmostdiv">
  <div id="top">
    <div id="fileinfodiv">
      <table class="fileinfo">
        <tbody>
          <tr>
            <td id="title" class="title" style="width: 70%">
              Title
            </td>
            <td id="revision" class="title" style="width: 30%">
              Revision
            </td>
          </tr>
          <tr>
            <td id="company">
              Company
            </td>
            <td id="filedate">
              Date
            </td>
          </tr>
        </tbody>
      </table>
    </div>
    <div id="bomcontrols">
      <div class="hideonprint menu">
        <button class="menubtn"></button>
        <div class="menu-content">
          <label class="menu-label menu-label-top" style="width: calc(50% - 18px)">
            <input id="darkmodeCheckbox" type="checkbox" onchange="setDarkMode(this.checked)">
            Dark mode
          </label><!-- This comment eats space! All of it!
          --><label class="menu-label menu-label-top" style="width: calc(50% - 17px); border-left: 0;">
            <input id="fullscreenCheckbox" type="checkbox" onchange="setFullscreen(this.checked)">
            Full Screen
          </label>
          <label class="menu-label" style="width: calc(50% - 18px)">
            <input id="fabricationCheckbox" type="checkbox" checked onchange="fabricationVisible(this.checked)">
            Fab layer
          </label><!-- This comment eats space! All of it!
          --><label class="menu-label" style="width: calc(50% - 17px); border-left: 0;">
            <input id="silkscreenCheckbox" type="checkbox" checked onchange="silkscreenVisible(this.checked)">
            Silkscreen
          </label>
          <label class="menu-label" style="width: calc(50% - 18px)">
            <input id="referencesCheckbox" type="checkbox" checked onchange="referencesVisible(this.checked)">
            References
          </label><!-- This comment eats space! All of it!
          --><label class="menu-label" style="width: calc(50% - 17px); border-left: 0;">
            <input id="valuesCheckbox" type="checkbox" checked onchange="valuesVisible(this.checked)">
            Values
          </label>
          <div id="tracksAndZonesCheckboxes">
            <label class="menu-label" style="width: calc(50% - 18px)">
              <input id="tracksCheckbox" type="checkbox" checked onchange="tracksVisible(this.checked)">
              Tracks
            </label><!-- This comment eats space! All of it!
            --><label class="menu-label" style="width: calc(50% - 17px); border-left: 0;">
              <input id="zonesCheckbox" type="checkbox" checked onchange="zonesVisible(this.checked)">
              Zones
            </label>
          </div>
          <label class="menu-label" style="width: calc(50% - 18px)">
            <input id="padsCheckbox" type="checkbox" checked onchange="padsVisible(this.checked)">
            Pads
          </label><!-- This comment eats space! All of it!
          --><label class="menu-label" style="width: calc(50% - 17px); border-left: 0;">
            <input id="dnpOutlineCheckbox" type="checkbox" checked onchange="dnpOutline(this.checked)">
            DNP outlined
          </label>
          <label class="menu-label">
            <input id="highlightRowOnClickCheckbox" type="checkbox" checked onchange="setHighlightRowOnClick(this.checked)">
            Highlight row on click
          </label>
          <label class="menu-label">
            <input id="dragCheckbox" type="checkbox" checked onchange="setRedrawOnDrag(this.checked)">
            Continuous redraw on drag
          </label>
          <label class="menu-label">
            Highlight first pin
            <form id="highlightpin1">
              <div class="flexbox">
                <label>
                  <input type="radio" name="highlightpin1" value="none" onchange="setHighlightPin1('none')">
                  None
                </label>
                <label>
                  <input type="radio" name="highlightpin1" value="all" onchange="setHighlightPin1('all')">
                  All
                </label>
                <label>
                  <input type="radio" name="highlightpin1" value="selected" onchange="setHighlightPin1('selected')">
                  Selected
                </label>
              </div>
            </form>
          </label>
          <label class="menu-label">
            <span>Board rotation</span>
            <span style="float: right"><span id="rotationDegree">0</span>&#176;</span>
            <input id="boardRotation" type="range" min="-36" max="36" value="0" class="slider" oninput="setBoardRotation(this.value)">
          </label>
          <label class="menu-label">
            <input id="offsetBackRotationCheckbox" type="checkbox" onchange="setOffsetBackRotation(this.checked)">
            Offset back rotation
          </label>
          <label class="menu-label">
            <div style="margin-left: 5px">Bom checkboxes</div>
            <input id="bomCheckboxes" class="menu-textbox" type=text
                   oninput="setBomCheckboxes(this.value)">
          </label>
          <label class="menu-label">
            <div style="margin-left: 5px">Mark when checked</div>
            <div id="markWhenCheckedContainer"></div>
          </label>
          <label class="menu-label">
            <span class="shameless-plug">
              <span>Created using</span>
              <a id="github-link" target="blank" href="https://github.com/openscopeproject/InteractiveHtmlBom">InteractiveHtmlBom</a>
              <a target="blank" title="Mouse and keyboard help" href="https://github.com/openscopeproject/InteractiveHtmlBom/wiki/Usage#bom-page-mouse-actions" style="text-decoration: none;"><label class="help-link">?</label></a>
            </span>
          </label>
        </div>
      </div>
      <div class="button-container hideonprint">
        <button id="fl-btn" class="left-most-button" onclick="changeCanvasLayout('F')"
                title="Front only">F
        </button>
        <button id="fb-btn" class="middle-button" onclick="changeCanvasLayout('FB')"
                title="Front and Back">FB
        </button>
        <button id="bl-btn" class="right-most-button" onclick="changeCanvasLayout('B')"
                title="Back only">B
        </button>
      </div>
      <div class="button-container hideonprint">
        <button id="bom-btn" class="left-most-button" onclick="changeBomLayout('bom-only')"
                title="BOM only"></button>
        <button id="lr-btn" class="middle-button" onclick="changeBomLayout('left-right')"
                title="BOM left, drawings right"></button>
        <button id="tb-btn" class="right-most-button" onclick="changeBomLayout('top-bottom')"
                title="BOM top, drawings bot"></button>
      </div>
      <div class="button-container hideonprint">
        <button id="bom-grouped-btn" class="left-most-button" onclick="changeBomMode('grouped')"
                title="Grouped BOM"></button>
        <button id="bom-ungrouped-btn" class="middle-button" onclick="changeBomMode('ungrouped')"
                title="Ungrouped BOM"></button>
        <button id="bom-netlist-btn" class="right-most-button" onclick="changeBomMode('netlist')"
                title="Netlist"></button>
      </div>
      <div class="hideonprint menu">
        <button class="statsbtn"></button>
        <div class="menu-content">
          <table class="stats">
            <tbody>
              <tr>
                <td width="40%">Board stats</td>
                <td>Front</td>
                <td>Back</td>
                <td>Total</td>
              </tr>
              <tr>
                <td>Components</td>
                <td id="stats-components-front">~</td>
                <td id="stats-components-back">~</td>
                <td id="stats-components-total">~</td>
              </tr>
              <tr>
                <td>Groups</td>
                <td id="stats-groups-front">~</td>
                <td id="stats-groups-back">~</td>
                <td id="stats-groups-total">~</td>
              </tr>
              <tr>
                <td>SMD pads</td>
                <td id="stats-smd-pads-front">~</td>
                <td id="stats-smd-pads-back">~</td>
                <td id="stats-smd-pads-total">~</td>
              </tr>
              <tr>
                <td>TH pads</td>
                <td colspan=3 id="stats-th-pads">~</td>
              </tr>
            </tbody>
          </table>
          <table class="stats">
            <col width="40%"/><col />
            <tbody id="checkbox-stats">
              <tr>
                <td colspan=2 style="border-top: 0">Checkboxes</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
      <div class="hideonprint menu">
        <button class="iobtn"></button>
        <div class="menu-content">
          <div class="menu-label menu-label-top">
            <div style="margin-left: 5px;">Save board image</div>
            <div class="flexbox">
              <input id="render-save-width" class="menu-textbox" type="text" value="1000" placeholder="Width"
                  style="flex-grow: 1; width: 50px;" oninput="validateSaveImgDimension(this)">
              <span>X</span>
              <input id="render-save-height" class="menu-textbox" type="text" value="1000" placeholder="Height"
                  style="flex-grow: 1; width: 50px;" oninput="validateSaveImgDimension(this)">
            </div>
            <label>
              <input id="render-save-transparent" type="checkbox">
              Transparent background
            </label>
            <div class="flexbox">
              <button class="savebtn" onclick="saveImage('F')">Front</button>
              <button class="savebtn" onclick="saveImage('B')">Back</button>
            </div>
          </div>
          <div class="menu-label">
            <span style="margin-left: 5px;">Config and checkbox state</span>
            <div class="flexbox">
              <button class="savebtn" onclick="saveSettings()">Export</button>
              <button class="savebtn" onclick="loadSettings()">Import</button>
              <button class="savebtn" onclick="resetSettings()">Reset</button>
            </div>
          </div>
          <div class="menu-label">
            <span style="margin-left: 5px;">Save bom table as</span>
            <div class="flexbox">
              <button class="savebtn" onclick="saveBomTable('csv')">csv</button>
              <button class="savebtn" onclick="saveBomTable('txt')">txt</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div id="topdivider">
    <div class="hideonprint">
      <div id="toptoggle" onclick="topToggle()">︽</div>
    </div>
  </div>
  <div id="bot" class="split" style="flex: 1 1">
    <div id="bomdiv" class="split split-horizontal">
      <div style="width: 100%">
        <input id="reflookup" class="textbox searchbox reflookup hideonprint" type="text" placeholder="Ref lookup"
               oninput="updateRefLookup(this.value)">
        <input id="filter" class="textbox searchbox filter hideonprint" type="text" placeholder="Filter"
               oninput="updateFilter(this.value)">
        <div class="button-container hideonprint" style="float: left; margin: 0;">
          <button id="copy" title="Copy bom table to clipboard"
               onclick="saveBomTable('clipboard')"></button>
        </div>
      </div>
      <div id="dbg"></div>
      <table class="bom" id="bomtable">
        <thead id="bomhead">
        </thead>
        <tbody id="bombody">
        </tbody>
      </table>
    </div>
    <div id="canvasdiv" class="split split-horizontal">
      <div id="frontcanvas" class="split" touch-action="none" style="overflow: hidden">
        <div style="position: relative; width: 100%; height: 100%;">
          <canvas id="F_bg" style="position: absolute; left: 0; top: 0; z-index: 0;"></canvas>
          <canvas id="F_fab" style="position: absolute; left: 0; top: 0; z-index: 1;"></canvas>
          <canvas id="F_slk" style="position: absolute; left: 0; top: 0; z-index: 2;"></canvas>
          <canvas id="F_hl" style="position: absolute; left: 0; top: 0; z-index: 3;"></canvas>
        </div>
      </div>
      <div id="backcanvas" class="split" touch-action="none" style="overflow: hidden">
        <div style="position: relative; width: 100%; height: 100%;">
          <canvas id="B_bg" style="position: absolute; left: 0; top: 0; z-index: 0;"></canvas>
          <canvas id="B_fab" style="position: absolute; left: 0; top: 0; z-index: 1;"></canvas>
          <canvas id="B_slk" style="position: absolute; left: 0; top: 0; z-index: 2;"></canvas>
          <canvas id="B_hl" style="position: absolute; left: 0; top: 0; z-index: 3;"></canvas>
        </div>
      </div>
    </div>
  </div>
</div>

</body>

</html>





<img width="1897" height="631" alt="image" src="https://github.com/user-attachments/assets/02c7996f-5387-4431-9811-42a02d390e3d" />
PCBWay specializes in providing high-quality, one-stop PCB manufacturing and PCBA assembly services, covering a variety of types, 
including multilayer boards, flexible boards, and high-frequency boards, and supports rapid prototyping and mass production.
They also offer supporting services such as component procurement, SMT, CNC machining, and 3D printing. 
With advanced equipment and strict quality control,PCBWAY provide customers with efficient and reliable electronics manufacturing solutions.
Thanks to PCBWAY!

<img width="449" height="509" alt="image" src="https://github.com/user-attachments/assets/d7f354b1-bca7-4688-b912-c92503ab5190" />


<img width="957" height="743" alt="image" src="https://github.com/user-attachments/assets/e9a65579-a771-434e-bd49-3b56b3f076d9" />

