# SatelliteConstellationForInternet
An essay about Computer networks and satellite constellation for internet 

<html><head><meta http-equiv="Content-Type" content="text/html; charset=utf-8"/><title>ESSAY: Satellite connection networks</title><style>
/* cspell:disable-file */
/* webkit printing magic: print all background colors */
html {
	-webkit-print-color-adjust: exact;
}
* {
	box-sizing: border-box;
	-webkit-print-color-adjust: exact;
}

html,
body {
	margin: 0;
	padding: 0;
}
@media only screen {
	body {
		margin: 2em auto;
		max-width: 900px;
		color: rgb(55, 53, 47);
	}
}

body {
	line-height: 1.5;
	white-space: pre-wrap;
}

a,
a.visited {
	color: inherit;
	text-decoration: underline;
}

.pdf-relative-link-path {
	font-size: 80%;
	color: #444;
}

h1,
h2,
h3 {
	letter-spacing: -0.01em;
	line-height: 1.2;
	font-weight: 600;
	margin-bottom: 0;
}

.page-title {
	font-size: 2.5rem;
	font-weight: 700;
	margin-top: 0;
	margin-bottom: 0.75em;
}

h1 {
	font-size: 1.875rem;
	margin-top: 1.875rem;
}

h2 {
	font-size: 1.5rem;
	margin-top: 1.5rem;
}

h3 {
	font-size: 1.25rem;
	margin-top: 1.25rem;
}

.source {
	border: 1px solid #ddd;
	border-radius: 3px;
	padding: 1.5em;
	word-break: break-all;
}

.callout {
	border-radius: 3px;
	padding: 1rem;
}

figure {
	margin: 1.25em 0;
	page-break-inside: avoid;
}

figcaption {
	opacity: 0.5;
	font-size: 85%;
	margin-top: 0.5em;
}

mark {
	background-color: transparent;
}

.indented {
	padding-left: 1.5em;
}

hr {
	background: transparent;
	display: block;
	width: 100%;
	height: 1px;
	visibility: visible;
	border: none;
	border-bottom: 1px solid rgba(55, 53, 47, 0.09);
}

img {
	max-width: 100%;
}

@media only print {
	img {
		max-height: 100vh;
		object-fit: contain;
	}
}

@page {
	margin: 1in;
}

.collection-content {
	font-size: 0.875rem;
}

.column-list {
	display: flex;
	justify-content: space-between;
}

.column {
	padding: 0 1em;
}

.column:first-child {
	padding-left: 0;
}

.column:last-child {
	padding-right: 0;
}

.table_of_contents-item {
	display: block;
	font-size: 0.875rem;
	line-height: 1.3;
	padding: 0.125rem;
}

.table_of_contents-indent-1 {
	margin-left: 1.5rem;
}

.table_of_contents-indent-2 {
	margin-left: 3rem;
}

.table_of_contents-indent-3 {
	margin-left: 4.5rem;
}

.table_of_contents-link {
	text-decoration: none;
	opacity: 0.7;
	border-bottom: 1px solid rgba(55, 53, 47, 0.18);
}

table,
th,
td {
	border: 1px solid rgba(55, 53, 47, 0.09);
	border-collapse: collapse;
}

table {
	border-left: none;
	border-right: none;
}

th,
td {
	font-weight: normal;
	padding: 0.25em 0.5em;
	line-height: 1.5;
	min-height: 1.5em;
	text-align: left;
}

th {
	color: rgba(55, 53, 47, 0.6);
}

ol,
ul {
	margin: 0;
	margin-block-start: 0.6em;
	margin-block-end: 0.6em;
}

li > ol:first-child,
li > ul:first-child {
	margin-block-start: 0.6em;
}

ul > li {
	list-style: disc;
}

ul.to-do-list {
	padding-inline-start: 0;
}

ul.to-do-list > li {
	list-style: none;
}

.to-do-children-checked {
	text-decoration: line-through;
	opacity: 0.375;
}

ul.toggle > li {
	list-style: none;
}

ul {
	padding-inline-start: 1.7em;
}

ul > li {
	padding-left: 0.1em;
}

ol {
	padding-inline-start: 1.6em;
}

ol > li {
	padding-left: 0.2em;
}

.mono ol {
	padding-inline-start: 2em;
}

.mono ol > li {
	text-indent: -0.4em;
}

.toggle {
	padding-inline-start: 0em;
	list-style-type: none;
}

/* Indent toggle children */
.toggle > li > details {
	padding-left: 1.7em;
}

.toggle > li > details > summary {
	margin-left: -1.1em;
}

.selected-value {
	display: inline-block;
	padding: 0 0.5em;
	background: rgba(206, 205, 202, 0.5);
	border-radius: 3px;
	margin-right: 0.5em;
	margin-top: 0.3em;
	margin-bottom: 0.3em;
	white-space: nowrap;
}

.collection-title {
	display: inline-block;
	margin-right: 1em;
}

.page-description {
	margin-bottom: 2em;
}

.simple-table {
	margin-top: 1em;
	font-size: 0.875rem;
	empty-cells: show;
}
.simple-table td {
	height: 29px;
	min-width: 120px;
}

.simple-table th {
	height: 29px;
	min-width: 120px;
}

.simple-table-header-color {
	background: rgb(247, 246, 243);
	color: black;
}
.simple-table-header {
	font-weight: 500;
}

time {
	opacity: 0.5;
}

.icon {
	display: inline-block;
	max-width: 1.2em;
	max-height: 1.2em;
	text-decoration: none;
	vertical-align: text-bottom;
	margin-right: 0.5em;
}

img.icon {
	border-radius: 3px;
}

.user-icon {
	width: 1.5em;
	height: 1.5em;
	border-radius: 100%;
	margin-right: 0.5rem;
}

.user-icon-inner {
	font-size: 0.8em;
}

.text-icon {
	border: 1px solid #000;
	text-align: center;
}

.page-cover-image {
	display: block;
	object-fit: cover;
	width: 100%;
	max-height: 30vh;
}

.page-header-icon {
	font-size: 3rem;
	margin-bottom: 1rem;
}

.page-header-icon-with-cover {
	margin-top: -0.72em;
	margin-left: 0.07em;
}

.page-header-icon img {
	border-radius: 3px;
}

.link-to-page {
	margin: 1em 0;
	padding: 0;
	border: none;
	font-weight: 500;
}

p > .user {
	opacity: 0.5;
}

td > .user,
td > time {
	white-space: nowrap;
}

input[type="checkbox"] {
	transform: scale(1.5);
	margin-right: 0.6em;
	vertical-align: middle;
}

p {
	margin-top: 0.5em;
	margin-bottom: 0.5em;
}

.image {
	border: none;
	margin: 1.5em 0;
	padding: 0;
	border-radius: 0;
	text-align: center;
}

.code,
code {
	background: rgba(135, 131, 120, 0.15);
	border-radius: 3px;
	padding: 0.2em 0.4em;
	border-radius: 3px;
	font-size: 85%;
	tab-size: 2;
}

code {
	color: #eb5757;
}

.code {
	padding: 1.5em 1em;
}

.code-wrap {
	white-space: pre-wrap;
	word-break: break-all;
}

.code > code {
	background: none;
	padding: 0;
	font-size: 100%;
	color: inherit;
}

blockquote {
	font-size: 1.25em;
	margin: 1em 0;
	padding-left: 1em;
	border-left: 3px solid rgb(55, 53, 47);
}

.bookmark {
	text-decoration: none;
	max-height: 8em;
	padding: 0;
	display: flex;
	width: 100%;
	align-items: stretch;
}

.bookmark-title {
	font-size: 0.85em;
	overflow: hidden;
	text-overflow: ellipsis;
	height: 1.75em;
	white-space: nowrap;
}

.bookmark-text {
	display: flex;
	flex-direction: column;
}

.bookmark-info {
	flex: 4 1 180px;
	padding: 12px 14px 14px;
	display: flex;
	flex-direction: column;
	justify-content: space-between;
}

.bookmark-image {
	width: 33%;
	flex: 1 1 180px;
	display: block;
	position: relative;
	object-fit: cover;
	border-radius: 1px;
}

.bookmark-description {
	color: rgba(55, 53, 47, 0.6);
	font-size: 0.75em;
	overflow: hidden;
	max-height: 4.5em;
	word-break: break-word;
}

.bookmark-href {
	font-size: 0.75em;
	margin-top: 0.25em;
}

.sans { font-family: ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI Variable Display", "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol"; }
.code { font-family: "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace; }
.serif { font-family: Lyon-Text, Georgia, ui-serif, serif; }
.mono { font-family: iawriter-mono, Nitti, Menlo, Courier, monospace; }
.pdf .sans { font-family: Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI Variable Display", "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK JP'; }
.pdf:lang(zh-CN) .sans { font-family: Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI Variable Display", "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK SC'; }
.pdf:lang(zh-TW) .sans { font-family: Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI Variable Display", "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK TC'; }
.pdf:lang(ko-KR) .sans { font-family: Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI Variable Display", "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK KR'; }
.pdf .code { font-family: Source Code Pro, "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK JP'; }
.pdf:lang(zh-CN) .code { font-family: Source Code Pro, "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK SC'; }
.pdf:lang(zh-TW) .code { font-family: Source Code Pro, "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK TC'; }
.pdf:lang(ko-KR) .code { font-family: Source Code Pro, "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK KR'; }
.pdf .serif { font-family: PT Serif, Lyon-Text, Georgia, ui-serif, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Serif CJK JP'; }
.pdf:lang(zh-CN) .serif { font-family: PT Serif, Lyon-Text, Georgia, ui-serif, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Serif CJK SC'; }
.pdf:lang(zh-TW) .serif { font-family: PT Serif, Lyon-Text, Georgia, ui-serif, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Serif CJK TC'; }
.pdf:lang(ko-KR) .serif { font-family: PT Serif, Lyon-Text, Georgia, ui-serif, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Serif CJK KR'; }
.pdf .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK JP'; }
.pdf:lang(zh-CN) .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK SC'; }
.pdf:lang(zh-TW) .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK TC'; }
.pdf:lang(ko-KR) .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK KR'; }
.highlight-default {
	color: rgba(55, 53, 47, 1);
}
.highlight-gray {
	color: rgba(120, 119, 116, 1);
	fill: rgba(120, 119, 116, 1);
}
.highlight-brown {
	color: rgba(159, 107, 83, 1);
	fill: rgba(159, 107, 83, 1);
}
.highlight-orange {
	color: rgba(217, 115, 13, 1);
	fill: rgba(217, 115, 13, 1);
}
.highlight-yellow {
	color: rgba(203, 145, 47, 1);
	fill: rgba(203, 145, 47, 1);
}
.highlight-teal {
	color: rgba(68, 131, 97, 1);
	fill: rgba(68, 131, 97, 1);
}
.highlight-blue {
	color: rgba(51, 126, 169, 1);
	fill: rgba(51, 126, 169, 1);
}
.highlight-purple {
	color: rgba(144, 101, 176, 1);
	fill: rgba(144, 101, 176, 1);
}
.highlight-pink {
	color: rgba(193, 76, 138, 1);
	fill: rgba(193, 76, 138, 1);
}
.highlight-red {
	color: rgba(212, 76, 71, 1);
	fill: rgba(212, 76, 71, 1);
}
.highlight-default_background {
	color: rgba(55, 53, 47, 1);
}
.highlight-gray_background {
	background: rgba(241, 241, 239, 1);
}
.highlight-brown_background {
	background: rgba(244, 238, 238, 1);
}
.highlight-orange_background {
	background: rgba(251, 236, 221, 1);
}
.highlight-yellow_background {
	background: rgba(251, 243, 219, 1);
}
.highlight-teal_background {
	background: rgba(237, 243, 236, 1);
}
.highlight-blue_background {
	background: rgba(231, 243, 248, 1);
}
.highlight-purple_background {
	background: rgba(244, 240, 247, 0.8);
}
.highlight-pink_background {
	background: rgba(249, 238, 243, 0.8);
}
.highlight-red_background {
	background: rgba(253, 235, 236, 1);
}
.block-color-default {
	color: inherit;
	fill: inherit;
}
.block-color-gray {
	color: rgba(120, 119, 116, 1);
	fill: rgba(120, 119, 116, 1);
}
.block-color-brown {
	color: rgba(159, 107, 83, 1);
	fill: rgba(159, 107, 83, 1);
}
.block-color-orange {
	color: rgba(217, 115, 13, 1);
	fill: rgba(217, 115, 13, 1);
}
.block-color-yellow {
	color: rgba(203, 145, 47, 1);
	fill: rgba(203, 145, 47, 1);
}
.block-color-teal {
	color: rgba(68, 131, 97, 1);
	fill: rgba(68, 131, 97, 1);
}
.block-color-blue {
	color: rgba(51, 126, 169, 1);
	fill: rgba(51, 126, 169, 1);
}
.block-color-purple {
	color: rgba(144, 101, 176, 1);
	fill: rgba(144, 101, 176, 1);
}
.block-color-pink {
	color: rgba(193, 76, 138, 1);
	fill: rgba(193, 76, 138, 1);
}
.block-color-red {
	color: rgba(212, 76, 71, 1);
	fill: rgba(212, 76, 71, 1);
}
.block-color-default_background {
	color: inherit;
	fill: inherit;
}
.block-color-gray_background {
	background: rgba(241, 241, 239, 1);
}
.block-color-brown_background {
	background: rgba(244, 238, 238, 1);
}
.block-color-orange_background {
	background: rgba(251, 236, 221, 1);
}
.block-color-yellow_background {
	background: rgba(251, 243, 219, 1);
}
.block-color-teal_background {
	background: rgba(237, 243, 236, 1);
}
.block-color-blue_background {
	background: rgba(231, 243, 248, 1);
}
.block-color-purple_background {
	background: rgba(244, 240, 247, 0.8);
}
.block-color-pink_background {
	background: rgba(249, 238, 243, 0.8);
}
.block-color-red_background {
	background: rgba(253, 235, 236, 1);
}
.select-value-color-uiBlue { background-color: rgba(35, 131, 226, .07); }
.select-value-color-pink { background-color: rgba(245, 224, 233, 1); }
.select-value-color-purple { background-color: rgba(232, 222, 238, 1); }
.select-value-color-green { background-color: rgba(219, 237, 219, 1); }
.select-value-color-gray { background-color: rgba(227, 226, 224, 1); }
.select-value-color-transparentGray { background-color: rgba(227, 226, 224, 0); }
.select-value-color-translucentGray { background-color: rgba(0, 0, 0, 0.06); }
.select-value-color-orange { background-color: rgba(250, 222, 201, 1); }
.select-value-color-brown { background-color: rgba(238, 224, 218, 1); }
.select-value-color-red { background-color: rgba(255, 226, 221, 1); }
.select-value-color-yellow { background-color: rgba(253, 236, 200, 1); }
.select-value-color-blue { background-color: rgba(211, 229, 239, 1); }
.select-value-color-pageGlass { background-color: undefined; }
.select-value-color-washGlass { background-color: undefined; }

.checkbox {
	display: inline-flex;
	vertical-align: text-bottom;
	width: 16;
	height: 16;
	background-size: 16px;
	margin-left: 2px;
	margin-right: 5px;
}

.checkbox-on {
	background-image: url("data:image/svg+xml;charset=UTF-8,%3Csvg%20width%3D%2216%22%20height%3D%2216%22%20viewBox%3D%220%200%2016%2016%22%20fill%3D%22none%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%0A%3Crect%20width%3D%2216%22%20height%3D%2216%22%20fill%3D%22%2358A9D7%22%2F%3E%0A%3Cpath%20d%3D%22M6.71429%2012.2852L14%204.9995L12.7143%203.71436L6.71429%209.71378L3.28571%206.2831L2%207.57092L6.71429%2012.2852Z%22%20fill%3D%22white%22%2F%3E%0A%3C%2Fsvg%3E");
}

.checkbox-off {
	background-image: url("data:image/svg+xml;charset=UTF-8,%3Csvg%20width%3D%2216%22%20height%3D%2216%22%20viewBox%3D%220%200%2016%2016%22%20fill%3D%22none%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%0A%3Crect%20x%3D%220.75%22%20y%3D%220.75%22%20width%3D%2214.5%22%20height%3D%2214.5%22%20fill%3D%22white%22%20stroke%3D%22%2336352F%22%20stroke-width%3D%221.5%22%2F%3E%0A%3C%2Fsvg%3E");
}
	
</style></head><body><article id="17275be0-d2f2-8070-a910-e67e282fbc01" class="page sans"><header><h1 class="page-title">ESSAY: Satellite connection networks</h1><p class="page-description"></p></header><div class="page-body"><p id="17675be0-d2f2-8025-b966-e11f77c43139" class="">How do thousands of satellites, orbiting around the Earth, communicate between each other and with the planet? Which algorithms and protocols allow these networks to transmit terabytes of data every second? In this essay I’m going to explore the innovative software architecture that drives satellite constellations and their role in transforming global connectivity.</p><p id="17675be0-d2f2-80db-a1a5-d99970f7173b" class="">First of all I’m going to make a brief digression on the first satellites. The first artificial satellite, Sputnik 1, was launched on October 4, 1957. It was very simple: a small aluminum sphere with four antennas. The launch of this satellite marked the beginning of the space age and it allowed us to comprehend the huge scientific, military and civil capabilities offered by the use of artificial satellites. According to UNOOSA records, there were 8,261 satellites orbiting the Earth in January 2022, out of which only 4,852 satellites were active (as at the end of December 2021). This was confirmed by the Union of Concerned Scientists (UCS), who maintains the record of the operational satellites.</p><table id="17675be0-d2f2-8083-9845-ee7379bcb0ea" class="simple-table"><tbody><tr id="17675be0-d2f2-8030-82ec-cd8882b99f2e"><td id="|uLC" class=""><strong>Number of satellites</strong></td><td id="SINJ" class=""><strong>Purpose</strong></td></tr><tr id="17675be0-d2f2-8002-9ec5-d24f05f2e968"><td id="|uLC" class="">3135</td><td id="SINJ" class="">Communication</td></tr><tr id="17675be0-d2f2-809a-bf99-cb10f8a52bb2"><td id="|uLC" class="">1030</td><td id="SINJ" class="">Earth observation</td></tr><tr id="17675be0-d2f2-804e-ab94-d5bb7dd4d55b"><td id="|uLC" class="">385</td><td id="SINJ" class="">Technology development</td></tr><tr id="17675be0-d2f2-8051-98af-f75a7aafc18f"><td id="|uLC" class="">154</td><td id="SINJ" class="">Navigation</td></tr><tr id="17675be0-d2f2-8026-a34c-e5b840628d99"><td id="|uLC" class="">22</td><td id="SINJ" class="">Earth science</td></tr><tr id="17675be0-d2f2-80d3-aec8-c6da765fac6d"><td id="|uLC" class="">18</td><td id="SINJ" class="">Other purposes</td></tr></tbody></table><h1 id="17675be0-d2f2-8008-8cc6-c35e632f74f2" class="">Satellite constellations for internet</h1><p id="17675be0-d2f2-80bd-9fcf-c431684e63e1" class="">The adoption of satellite constellations for internet data transmission represent a major technological innovation that could help to overcome the limitations of terrestrial infrastructures. Thanks to their position in orbit, satellites can ensure global coverage, reaching geographical areas that otherwise would be inaccessible. This approach uses advanced software communication systems to improve network resilience and to manage data traffic on a planetary scale, making them a scientifically valid solution to ensure reliable and scalable connectivity.</p><p id="17675be0-d2f2-808e-b465-d7bc91cbd0a4" class="">However, despite this introduction, how do they work?</p><h2 id="17675be0-d2f2-804d-83f2-c408b87c8f38" class="">Architecture</h2><p id="17675be0-d2f2-8062-8cb5-ce2a14b78455" class="">The satellites of the constellations for low-latency global broadband satellite internet access are positioned in low earth orbit (LEO) which works in harmony with terrestrial transceivers.</p><p id="17675be0-d2f2-8033-991a-c7176c314ac1" class="">Furthermore, low Earth orbit, as suggested by the name, is relatively close to the Earth, usually at less than 1000 km of altitude but it could also be lower. LEO satellites don’t always have to follow a specific path around the Earth and their plane can be tilted, this means there are more viable routes for satellites.</p><p id="17675be0-d2f2-80a4-bf4d-eb603a148ee5" class="">However, individual LEO satellites are less useful for tasks like communication because they move too fast to be tracked from ground stations. For this reason the satellites in LEO work often as part of a large constellation in order to cover large areas of the Earth simultaneously by working together.</p><p id="17675be0-d2f2-809e-814f-ff49261741b2" class="">Starlink by Space X is the most known constellation for internet communication. Space X already launched almost 6770 satellites (in November 2024), it had the permission to launch 12000 satellites and currently it has 42000 planned in future.</p><p id="17675be0-d2f2-80df-aef4-f91981dcde13" class="">Moreover, the satellite positioning is crucial to ensure global coverage and maximize network efficiency:</p><ul id="17675be0-d2f2-80ce-8cdf-e2285086c023" class="bulleted-list"><li style="list-style-type:disc">Satellites are distributed in polar or inclined orbits to cover uniformly the entire Earth&#x27;s surface. For instance, the Starlink constellation uses a “shell” configuration, where satellites orbit at different altitudes and inclinations.</li></ul><ul id="17675be0-d2f2-8060-881b-c7c1f3105104" class="bulleted-list"><li style="list-style-type:disc">Each satellite has an overlapping coverage area with its neighbors to ensure signal continuity during handovers between satellites.</li></ul><ul id="17675be0-d2f2-8041-9b22-deef16c54037" class="bulleted-list"><li style="list-style-type:disc">Satellites communicate with each other using lasers or radio waves, forming an orbital mesh network that reduces the need of ground stations and increases network resilience.</li></ul><p id="17675be0-d2f2-806b-bb62-cdd923f9daef" class="">Therefore, satellite constellation architecture isn’t just a matter of placement, but a balance between physics, engineering, and software working to ensure reliable, low-propagation time, and scalable connectivity.</p><h2 id="17675be0-d2f2-8063-a6b2-c8fbd86e1b27" class="">Software</h2><p id="17675be0-d2f2-80ff-a875-db32b1b5decd" class="">Internet satellite constellations represent an extraordinary evolution of communication infrastructures, which were possible thanks to a perfect integration between advanced hardware and new softwares.</p><p id="17675be0-d2f2-8071-8a29-c0fcafde88b7" class="">The main component of these satellite constellations’ software is the network management through dynamic routing and direct connections, called Inter-Satellite Links (ISL); it reduces latency in communications with the implementation of error recovery algorithms. In addition a fundamental role is played by the communication protocols used and optimized for satellite networks. Overall, the management of continuous development and cyber security are also of great importance.</p><h3 id="17675be0-d2f2-80ff-837d-cd90370c39fc" class="">Dynamic Routing</h3><p id="17775be0-d2f2-80bc-8881-e94f01638768" class="">Routing is the main function of the network layer in a computer network. Satellite networks could be very complex because of the distance between nodes, their movement in orbit and the varying conditions of the communication links, such as delay, bandwidth and potential signal interference. Therefore it’s important to find the best path for data. Dynamic routing is a process where a router can forward data through a different route for a given destination, based on the current conditions of the communication circuits within a system.</p><p id="17675be0-d2f2-80c7-acd6-f9a86a9d6375" class=""><strong>Static vs. dynamic routing:</strong></p><ul id="17675be0-d2f2-8035-9eb9-c91d350cbaa4" class="bulleted-list"><li style="list-style-type:disc"><strong>Path Selection</strong>: Static routing uses a single preconfigured route to move data to its destinations, conversely dynamic routing provides multiple viable routes to the destination.</li></ul><ul id="17675be0-d2f2-8087-a532-ce8554baffa8" class="bulleted-list"><li style="list-style-type:disc"><strong>Routing tables</strong>: Static routing has a smaller routing table with one entry for each destination on the contrary dynamic routing needs to send out their entire routing tables to identify the best route.</li></ul><ul id="17675be0-d2f2-80d0-969d-e1af232342b1" class="bulleted-list"><li style="list-style-type:disc"><strong>Protocols and algorithms</strong>: Dynamic routing uses distance vector, and other kinds of protocols to adjust routes.</li></ul><ul id="17675be0-d2f2-80b3-a5b0-c543d8ce1b4b" class="bulleted-list"><li style="list-style-type:disc"><strong>Computation and bandwidth</strong>: Dynamic routing requires more computation and bandwidth to generate multiple route possibilities.</li></ul><p id="17675be0-d2f2-80b8-a169-d74959ebff6a" class="">Dynamic routing in satellite constellations is essential to ensure efficient and reliable communication in networks with highly dynamic topologies. Unlike terrestrial networks, where nodes are generally stationary, satellites in low orbit (LEO) move rapidly relative to the Earth&#x27;s surface, requiring advanced data path management. Modern constellations use inter-satellite links (ISLs) to create a mesh network in space. These links allow satellites to communicate directly with each other, reducing dependency on ground stations and improving network delay and resilience. Dynamic routing uses these ISLs to route data through optimal paths, adapting in real time to changes in network topology due to satellite movement.</p><p id="17675be0-d2f2-8099-b214-e3557a89eecc" class="">Besides, the routing algorithms of these networks need to consider various factors, including latency, available bandwidth and link stability. Some approaches include:</p><ul id="17675be0-d2f2-8075-8b14-d02a2ee907ce" class="bulleted-list"><li style="list-style-type:disc"><strong>Virtual topology-based routing</strong>: It transforms the dynamic network into a series of predictable static topologies, facilitating the application of traditional routing algorithms.</li></ul><ul id="17675be0-d2f2-800c-a870-ef0c51cd0823" class="bulleted-list"><li style="list-style-type:disc"><strong>Predictive routing</strong>: It uses mathematical models to predict the future position of satellites and to anticipate changes in network topology, thus optimizing data routing.</li></ul><ul id="17675be0-d2f2-8016-ac41-e6fd76933d0c" class="bulleted-list"><li style="list-style-type:disc"><strong>Adaptive routing</strong>: Dynamically adjusts routing decisions based on current network conditions, such as congestion or faults, to maintain optimal performance.</li></ul><p id="17675be0-d2f2-8019-967a-e46462133cbb" class="">Low Earth Orbit systems require specialized routing protocols to manage the dynamic and  quick changing of the network topology. Many satellite constellations have their own dynamic routing protocols but they are proprietary and there isn&#x27;t information about them.</p><p id="17675be0-d2f2-808b-be52-dfc703994e9b" class="">However, an example of Dynamic routing algorithm is ‘Distance Vector’: in this algorithm each router has a table, containing the outgoing line to reach the destination and an estimated distance. Periodically each router sends to each neighbor a list of its estimated delay. Based on the estimates of the neighbors the router can update its routing table.</p><h3 id="17675be0-d2f2-80f4-b728-ffc0460afd00" class="">Communication protocols</h3><p id="17675be0-d2f2-80ef-89f1-ebe646cc7842" class="">According to the transport layer the transport protocols play a significant role in the satellite constellations: the Transmission Control Protocol (TCP) is one of the most used protocols in the terrestrial networks, however in the satellite networks it comes across some difficulties.</p><p id="17675be0-d2f2-80d5-962a-cfe9c123b917" class="">Among the main critical points of the application of this system, in the satellite networks, can be point out:</p><p id="17675be0-d2f2-807a-b4ad-fa9a8f4b0ab5" class="">high propagation time in the LEO satellites, but mostly in the GEO, possible false congestion detection, links variability and reduced efficiency since the initial TCP handshake needs more roundtrip.</p><p id="17675be0-d2f2-804f-a1eb-e1efb13a5acb" class="">In order to solve these problems in the satellite networks, over time have been developed different versions of the traditional protocols, which have been studied for this specific type of connections.</p><p id="17675be0-d2f2-80db-bca5-c16b48266130" class=""><strong>TCP-Peach</strong></p><p id="17675be0-d2f2-80c4-b297-eacac5f22a83" class="">It is designed for high delay networks and it uses test packages called dummy packets to estimate the capacity of the network without penalising transmission speed.</p><p id="17675be0-d2f2-8080-85b3-cd07c3de2a9b" class=""><strong>Split-TCP</strong></p><p id="17675be0-d2f2-8019-a912-edf8851d00d3" class="">It divides the connection in two sections: the first one between the sender and an Earth station, the second one between the Earth station and the receiver through the satellites. In this way it reduces the perceived latency and it improves the transmission efficiency.</p><p id="17675be0-d2f2-8016-aae8-d6bd821adf0c" class=""><strong>Information-centric TCP for Satellite Network (INTCP)</strong></p><p id="17675be0-d2f2-803c-a7f8-effeb427dbf8" class="">Furthermore, the INTCP is a truly innovative proposal. It is a transport layer protocol specifically designed to address the unique challenges of satellite networks.</p><p id="17675be0-d2f2-8052-a1da-d1acdffac464" class="">INTCP introduces a novel hop-by-hop transport layer design that incorporates several key features:</p><ul id="17675be0-d2f2-8079-9c72-e33f57fec23b" class="bulleted-list"><li style="list-style-type:disc"><strong>Hop-by-Hop Packet Retransmission</strong>: INTCP reduces retransmission lag and enhances reliability, by handling packet loss at each hop</li></ul><ul id="17675be0-d2f2-80db-aabe-c0567abd68c5" class="bulleted-list"><li style="list-style-type:disc"><strong>Hop-by-Hop Congestion Control</strong>: Each node manages traffic and congestion independently, optimizing bandwidth utilization and improving end-to-end throughput.</li></ul><ul id="17675be0-d2f2-8002-9e2f-f824d5054d81" class="bulleted-list"><li style="list-style-type:disc"><strong>Caching and Request-Response Model</strong>: The use of caching enables asynchronous multicast at the transport layer, conserving valuable spectrum resources in the satellite network.</li></ul><p id="17675be0-d2f2-80d5-900d-ce33b5aa9b54" class="">Performance evaluations using a simulated Starlink constellation over distances exceeding 1,000 km have demonstrated that INTCP significantly outperforms traditional TCP. In unicast scenarios, INTCP reduced one-way delay by 42%, decreased delay jitter by 53%, and increased throughput by 60%. In multicast scenarios, INTCP achieved more than six times the throughput of TCP.</p><p id="17675be0-d2f2-80d4-86d2-c2e76b21a2e8" class="">Functioning:</p><ol type="1" id="17675be0-d2f2-80ad-abd2-c91008ccb1bc" class="numbered-list" start="1"><li><strong>Data Naming</strong>: Each data packet is assigned a unique name that facilitates efficient data retrieval and routing.</li></ol><ol type="1" id="17675be0-d2f2-802c-a0bb-f999927077df" class="numbered-list" start="2"><li><strong>Request-Response Model</strong>: When a device needs data, it sends an &quot;Interest&quot; message to the network. Intermediate nodes, such as routers, check their caches to see if they have the requested data. If they do, they respond with the data; if not, the request propagates toward the data source.</li></ol><ol type="1" id="17675be0-d2f2-8090-be8d-e9eab916caea" class="numbered-list" start="3"><li><strong>Caching</strong>: Intermediate nodes cache data they forward. This caching allows subsequent requests for the same data to be served directly from the cache, reducing lag and conserving bandwidth.</li></ol><ol type="1" id="17675be0-d2f2-8021-b79c-d10697246500" class="numbered-list" start="4"><li><strong>Hop-by-Hop Retransmission</strong>: Handles packet loss at each hop. If a packet is lost between two nodes, the receiving node requests a retransmission from the previous node, ensuring faster recovery.</li></ol><ol type="1" id="17675be0-d2f2-80e4-8eb0-d65a35ee2ed3" class="numbered-list" start="5"><li><strong>Hop-by-Hop Congestion Control</strong>: Each node independently manages congestion by adjusting its transmission rate based on local network conditions. This decentralized approach helps optimize bandwidth utilization and maintain consistent performance.</li></ol><ol type="1" id="17675be0-d2f2-80ef-90f7-e21df83c2784" class="numbered-list" start="6"><li><strong>Asynchronous Multicast</strong>: INTCP supports multicast communication by allowing data to be cached and forwarded to multiple requesters simultaneously. This method efficiently uses network resources, especially in scenarios where the same data is requested by multiple devices.</li></ol><h3 id="17675be0-d2f2-8089-95c3-faf65b74fc1e" class="">Communication between Earth and satellites</h3><p id="17675be0-d2f2-805c-918c-cfb00785b7dd" class="">The communication between the Earth and satellites is fundamental for the modern telecommunication networks, including the internet communication systems that are based on satellite constellations. This interaction involves different technological and operational aspects, such as the use of ground stations, radio or laser frequencies, the beam-forming and the traffic management between terrestrial and satellite users.</p><p id="17675be0-d2f2-8094-a63e-eac0762b7126" class="">Ground stations are essential infrastructures that establish and maintain satellite links. They are equipped with satellite dishes, receivers and transmitters, and are responsible for critical operations such as satellite tracking, communications management and data processing.</p><h2 id="17675be0-d2f2-80a6-9066-f194eb3c1e4f" class="">Final Considerations</h2><p id="17675be0-d2f2-80e3-b8d1-ff5863621e39" class="">The satellite constellations represent one of the most promising innovations in the perspectives of global communications. The constellation LEO expansion and the progressive evolution of technologies are opening new possibilities to provide high-speed internet connectivity in remote and developing areas, reducing the digital divide and improving network resilience.</p><p id="17675be0-d2f2-8025-b38b-ed8bbf6818a0" class="">With these advancements, the ability to ensure efficient, reliable, and scalable communication across vast distances becomes increasingly achievable.</p><p id="17675be0-d2f2-8034-8206-ead18f2e4ce6" class="">Looking at the future, the satellites constellations’ expansion could radically transform the perspectives of global communications. Space communications could become an essential part of the global infrastructures of the internet with increasing density of orbiting satellites, the introduction of new technologies, such as AI for the dynamic network management and the improvement of routing techniques.</p><p id="17675be0-d2f2-80eb-882d-e7b05e250f12" class="">Furthermore, the adoption of hybrid networks, combining satellites with other communication technologies such as 5G, could facilitate the transition to a truly global connectivity system, capable of supporting an increasing number of IoT devices and data-intensive applications.</p><p id="17675be0-d2f2-80a7-8cd0-e19330e340e2" class="">In this context, the progressive innovation and improvement of transport protocols and other technologies, together with the increasing processing capacity on satellites, will pave the way for a future where the Internet will be accessible and reliable everywhere, accelerating economic and social development on a global scale.</p><p id="17775be0-d2f2-80ed-b28d-d10464d82114" class="">Overall the satellite constellations represent one of the most promising innovations in the perspectives of global communications. The constellation LEO expansion and the progressive evolution of technologies are opening new possibilities to provide high-speed internet connectivity in remote and developing areas, reducing the digital divide and improving network resilience.</p><p id="17775be0-d2f2-80f9-9934-c39399e0c6f2" class="">In addition, the ability to ensure efficient, reliable, and scalable communication across vast distances becomes increasingly achievable thanks to these advancements.</p><p id="17775be0-d2f2-80ae-a6e1-f52d7d19086c" class="">In the future, the satellites constellations’ expansion could radically transform the perspectives of global communications. Space communications could become an essential part of the global infrastructures of the internet with increasing density of orbiting satellites, the introduction of new technologies, such as AI for the dynamic network management and the improvement of routing techniques.</p><p id="17775be0-d2f2-8001-afb9-fe2222f685e0" class="">Furthermore, the adoption of hybrid networks, combining satellites with other communication technologies such as 5G, could facilitate the transition to a truly global connectivity system, capable of supporting an increasing number of IoT devices and data-intensive applications.</p><p id="17775be0-d2f2-80d0-9d20-e0c0a84e1fb5" class="">In this context, the progressive innovation and improvement of transport protocols and other technologies, together with the increasing processing capacity on satellites, will pave the way for a future where the Internet will be accessible and reliable everywhere, accelerating economic and social development on a global scale<del>.</del></p><h3 id="17675be0-d2f2-805d-bd8b-c4e476ca75b5" class="">Bibliography:</h3><p id="17675be0-d2f2-8071-9d19-c7ac30d9b37e" class=""><a href="https://it.wikipedia.org/wiki/Telecomunicazioni_satellitari">https://it.wikipedia.org/wiki/Telecomunicazioni_satellitari</a></p><p id="17675be0-d2f2-80f7-9625-d85818c4ed49" class=""><a href="https://ieeexplore.ieee.org/document/9680870">https://ieeexplore.ieee.org/document/9680870</a></p><p id="17675be0-d2f2-809e-8318-cc8f85a89c5e" class=""><a href="https://arxiv.org/abs/2112.14916?utm_source=chatgpt.com">https://arxiv.org/abs/2112.14916?utm_source=chatgpt.com</a></p><p id="17675be0-d2f2-80c9-88d6-ee3e55c7c910" class="">(<a href="https://en.wikipedia.org/wiki/OSI_model">https://en.wikipedia.org/wiki/OSI_model</a>)</p><p id="17675be0-d2f2-80df-8116-fba77cceea27" class=""><a href="https://arxiv.org/pdf/2401.09455">https://arxiv.org/pdf/2401.09455</a></p><p id="17675be0-d2f2-804e-a809-f0c2538e7b3f" class=""><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC9231381/">https://pmc.ncbi.nlm.nih.gov/articles/PMC9231381/</a></p><p id="17675be0-d2f2-80bd-8543-d6dfa06258c4" class=""><a href="https://ieeexplore.ieee.org/document/929853">https://ieeexplore.ieee.org/document/929853</a></p><p id="17675be0-d2f2-80c2-a427-d2680b2fe8ce" class=""><a href="https://ianakyildiz.com/bwn/papers/2001/j8.pdf">https://ianakyildiz.com/bwn/papers/2001/j8.pdf</a></p><p id="17675be0-d2f2-8006-85ba-fa96c78b5bfc" class=""><a href="https://ieeexplore.ieee.org/document/1189171">https://ieeexplore.ieee.org/document/1189171</a></p><p id="17675be0-d2f2-805a-982f-ef9af63e8508" class=""><a href="https://ieeexplore.ieee.org/document/9258315">https://ieeexplore.ieee.org/document/9258315</a></p><p id="17675be0-d2f2-8001-8905-e5e9ebd3897a" class=""><a href="https://ieeexplore.ieee.org/document/1264081?utm_source=chatgpt.com">https://ieeexplore.ieee.org/document/1264081?utm_source=chatgpt.com</a></p><p id="17675be0-d2f2-8017-ae7d-efead47bdfdc" class=""><a href="https://www.techtarget.com/searchnetworking/answer/Static-and-dynamic-routing">https://www.techtarget.com/searchnetworking/answer/Static-and-dynamic-routing</a></p><p id="17675be0-d2f2-80ff-b8f0-d3f6ac31005f" class=""><a href="https://en.wikipedia.org/wiki/Dynamic_routing">https://en.wikipedia.org/wiki/Dynamic_routing</a></p><p id="17675be0-d2f2-80fc-bd6b-d4fb3f7995a3" class=""><a href="https://learningnetwork.cisco.com/s/article/meraki-starlink-deployment-guide">https://learningnetwork.cisco.com/s/article/meraki-starlink-deployment-guide</a></p><p id="17675be0-d2f2-8092-a39d-d0919a20d73f" class=""><a href="https://en.wikipedia.org/wiki/Computer_network">https://en.wikipedia.org/wiki/Computer_network</a></p><p id="17675be0-d2f2-80d0-a47a-d1b327646670" class=""><a href="https://dl.ebooksworld.ir/motoman/MK.Computer.Networks.Fifth.Edition.A.Systems.Approach.www.EBooksWorld.ir.pdf">https://dl.ebooksworld.ir/motoman/MK.Computer.Networks.Fifth.Edition.A.Systems.Approach.www.EBooksWorld.ir.pdf</a></p><p id="17675be0-d2f2-802b-b060-c6833c4317a1" class=""><a href="https://csc-knu.github.io/sys-prog/books/Andrew%20S.%20Tanenbaum%20-%20Computer%20Networks.pdf">https://csc-knu.github.io/sys-prog/books/Andrew%20S.%20Tanenbaum%20-%20Computer%20Networks.pdf</a></p><p id="17675be0-d2f2-8005-8383-ea309ed2d334" class=""><a href="https://csc-knu.github.io/sys-prog/books/Andrew%20S.%20Tanenbaum%20-%20Computer%20Networks.pdf">https://csc-knu.github.io/sys-prog/books/Andrew%20S.%20Tanenbaum%20-%20Computer%20Networks.pdf</a></p><p id="17675be0-d2f2-80a8-a045-d76470d298cf" class=""><a href="https://www.esa.int/ESA_Multimedia/Images/2020/03/Low_Earth_orbit">https://www.esa.int/ESA_Multimedia/Images/2020/03/Low_Earth_orbit</a></p><p id="17675be0-d2f2-80a7-97e2-cab87fe80b88" class=""><a href="https://it.wikipedia.org/wiki/Orbita_terrestre_bassa">https://it.wikipedia.org/wiki/Orbita_terrestre_bassa</a></p><p id="17675be0-d2f2-80d2-aaf1-ee0834c85d04" class=""><a href="https://en.wikipedia.org/wiki/Low_Earth_orbit">https://en.wikipedia.org/wiki/Low_Earth_orbit</a></p></div></article><span class="sans" style="font-size:14px;padding-top:2em"></span></body></html>
