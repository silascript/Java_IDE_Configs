# Eclipse 内置UI的部分CSS


---


## 基础CSS


### e4_classic

```shell

$ cat /opt/JavaIDE/eclipse-ee/plugins/org.eclipse.ui.themes_1.2.2700.v20250122-1423/css/e4_classic.css 
/*******************************************************************************
 * Copyright (c) 2010, 2014 IBM Corporation and others.
 *
 * This program and the accompanying materials
 * are made available under the terms of the Eclipse Public License 2.0
 * which accompanies this distribution, and is available at
 * https://www.eclipse.org/legal/epl-2.0/
 *
 * SPDX-License-Identifier: EPL-2.0
 *
 * Contributors:
 *     IBM Corporation - initial API and implementation
 *     Lars Vogel <Lars.Vogel@gmail.com> - Bug 420836
 *******************************************************************************/

.MPart.busy {
	font-style: italic;
}

.MPart.highlighted {
	font-weight: bold;
}

.MPartStack, .MPart {
	font-family: '#org-eclipse-ui-workbench-TAB_TEXT_FONT';
}

CTabItem:selected {
	color: '#org-eclipse-ui-workbench-ACTIVE_TAB_TEXT_COLOR';
}

.MTrimmedWindow {
	margin-top: 0px;
	margin-bottom: 0px;
	margin-left: 2px;
	margin-right: 2px;
}

.MPartStack {
	swt-tab-renderer: null;
	swt-selected-tabs-background: '#org-eclipse-ui-workbench-INACTIVE_TAB_BG_START' '#org-eclipse-ui-workbench-INACTIVE_TAB_BG_END' 100%;
	swt-simple: false;
	color: '#org-eclipse-ui-workbench-INACTIVE_TAB_TEXT_COLOR';
}

.MPartStack.active {
	swt-selected-tabs-background: '#org-eclipse-ui-workbench-ACTIVE_TAB_BG_START' '#org-eclipse-ui-workbench-ACTIVE_TAB_BG_END' 100%;
}

.MPartStack.active.noFocus {
	swt-selected-tabs-background: '#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_BG_START' '#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_BG_END' 100%;
}

.MPartStack.active.noFocus > CTabItem:selected {
	color: '#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_TEXT_COLOR';
}

.DragFeedback {
	background-color: COLOR-WIDGET-NORMAL-SHADOW;
}

.ModifiedDragFeedback {
	background-color: #A0A000;
}

#org-eclipse-ui-editorss {
	swt-tab-height: 8px;
}


```


### e4_basestyle

```shell

$ cat /opt/JavaIDE/eclipse-ee/plugins/org.eclipse.ui.themes_1.2.2700.v20250122-1423/css/e4_basestyle.css
/*******************************************************************************
 * Copyright (c) 2010, 2014 IBM Corporation and others.
 *
 * This program and the accompanying materials
 * are made available under the terms of the Eclipse Public License 2.0
 * which accompanies this distribution, and is available at
 * https://www.eclipse.org/legal/epl-2.0/
 *
 * SPDX-License-Identifier: EPL-2.0
 *
 * Contributors:
 *     IBM Corporation - initial API and implementation
 *     Lars Vogel <Lars.Vogel@gmail.com> - Bug 420836
 *******************************************************************************/

@import url("platform:/plugin/org.eclipse.ui.themes/css/common/e4_globalstyle.css");
@import url("platform:/plugin/org.eclipse.ui.themes/css/light/e4-light_globalstyle.css");
@import url("platform:/plugin/org.eclipse.ui.themes/css/light/e4-light_ide_colorextensions.css");
@import url("platform:/plugin/org.eclipse.ui.themes/css/light/e4-light_partstyle.css");
@import url("platform:/plugin/org.eclipse.ui.themes/css/light/e4-light_tabstyle.css");
@import url("platform:/plugin/org.eclipse.ui.themes/css/light/e4-light-drag-styling.css");

```


### e4_default_gtk


```shell

$ cat /opt/JavaIDE/eclipse-ee/plugins/org.eclipse.ui.themes_1.2.2700.v20250122-1423/css/e4_default_gtk.css 
/*******************************************************************************
 * Copyright (c) 2010, 2014 IBM Corporation and others.
 *
 * This program and the accompanying materials
 * are made available under the terms of the Eclipse Public License 2.0
 * which accompanies this distribution, and is available at
 * https://www.eclipse.org/legal/epl-2.0/
 *
 * SPDX-License-Identifier: EPL-2.0
 *
 * Contributors:
 *     IBM Corporation - initial API and implementation
 *     Lars Vogel <Lars.Vogel@gmail.com> - Bug 420836
 *     Mickael Istria <mistria@redhat.com> - 325937
 *     Patrik Suzzi <psuzzi@gmail.com> - Bug 501250
 *     SAP SE - light theme improvements
 *******************************************************************************/

@import url("platform:/plugin/org.eclipse.ui.themes/css/e4_basestyle.css");

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_UNSELECTED_TABS_COLOR_START {
	color: #f8f8f8; /* same as '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND' cannot use it directly*/
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_UNSELECTED_TABS_COLOR_END {
	color: #F8F8F8; /* same as '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND' cannot use it directly*/
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_TAB_OUTER_KEYLINE_COLOR {
	color: #e5e5e5;
}
ColorDefinition#org-eclipse-ui-workbench-ACTIVE_TAB_INNER_KEYLINE_COLOR {
	color: #f8f8f8; /* same as '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND' cannot use it directly*/
}
ColorDefinition#org-eclipse-ui-workbench-ACTIVE_TAB_OUTLINE_COLOR {
	color: #e5e5e5;
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_UNSELECTED_TABS_COLOR_START {
	color: #f8f8f8; /* same as '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND' cannot use it directly*/
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_UNSELECTED_TABS_COLOR_END {
	color: #f8f8f8; /* same as '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND' cannot use it directly*/
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_TAB_OUTER_KEYLINE_COLOR {
	color: #e5e5e5;
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_TAB_INNER_KEYLINE_COLOR {
	color: #f8f8f8; /* same as '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND' cannot use it directly*/
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_TAB_OUTLINE_COLOR {
	color: #e5e5e5;
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_TAB_BG_START {
	color: #f8f8f8; /* same as '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND' cannot use it directly*/
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_TAB_BG_END {
	color: #f8f8f8; /* same as '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND' cannot use it directly*/
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_TAB_BG_START{
	color: #f8f8f8; /* same as '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND' cannot use it directly*/
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_TAB_BG_END {
	color: #f8f8f8;  /* same as '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND' cannot use it directly*/
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_NOFOCUS_TAB_BG_START {
	color: #f8f8f8; /* same as '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND' cannot use it directly*/
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_NOFOCUS_TAB_BG_END {
	color: #f8f8f8; /* same as '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND' cannot use it directly*/
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_BG_START {
	color: #f8f8f8; /* same as '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND' cannot use it directly*/
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_BG_END {
	color: #f8f8f8; /* same as '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND' cannot use it directly*/
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_TEXT_COLOR {
	color: #000000;
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_TAB_TEXT_COLOR {
	color: #000000;
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_TAB_TEXT_COLOR {
	color: #000000;
}

.MTrimmedWindow {
	background-color: #f6f5f4;
}

.MTrimBar {
	background-color: #f6f5f4;
}

.MTrimBar#org-eclipse-ui-main-toolbar  {
	background-color: COLOR-WIDGET-BACKGROUND #f6f5f4 100%;
}

.MPartStack {
	swt-simple: false;
}

CTabFolder.MArea {
	background-color: '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND';
	swt-selected-tab-fill: '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND';
	swt-unselected-tabs-color: '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND';
	swt-outer-keyline-color: '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND';
	swt-inner-keyline-color: '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND';
	swt-tab-outline: #ffffff;
}

CTabFolder Canvas {
	background-color: '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND';
}

.MTrimBar#org-eclipse-ui-main-toolbar {
	background-color: '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND';
}

.MTrimBar#org-eclipse-ui-trim-status {
	background-color: '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND';
}

.View Composite,
.View Composite Tree,
.View Composite Label,
.View ToolBar,
.View Group,
.View Group Label,
.View Section,
.View BusyIndicator,
.View Text[style~='SWT.READ_ONLY'],
.View SashForm,
.View OleFrame,
.View Browser,
.View WebSite,
.View StyledText[style~='SWT.READ_ONLY'],
.View Link,
.View FormText,
.View Hyperlink,
.View Canvas,
.View FigureCanvas
{
	background-color: '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND';
}

.View TitleRegion{
	background-color: '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND';
}

.MPartStack.active .View TitleRegion{
	background-color: '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND';
}

.View Button[style~='SWT.CHECK']{
	background-color: inherit;
}

.View Toolbar ToolItem{
	background-color: #eaeaea;
}

.View TabbedPropertyList{
	swt-tabBackground-color: #ffffff;
}

.View Composite PrependingAsteriskFilteredTree,
.View PrependingAsteriskFilteredTree Text,
.View Group Text,
.View Group Combo,
.View Composite Text,
.View Button[style~='SWT.PUSH']{
	background-color: #ffffff;
}

.MPartStack{
	swt-selected-tab-highlight: #8a8a8a;
	swt-selected-highlight-top: false;
}

.MPartStack.active {
	swt-selected-tab-highlight: #2160bb;
	swt-selected-highlight-top: false;
}

/* text color and background color of unselected tabs in editor*/
#org-eclipse-ui-editorss CTabItem{
	color: #000000;
	background-color: #f8f8f8;
}

/*text color and background color of selected tab in editor */
#org-eclipse-ui-editorss CTabItem:selected{
	color: #000000;
	background-color: #ffffff;
}

#org-eclipse-ui-editorss CTabFolder{
	swt-selected-tab-fill : #ffffff;
	swt-selected-tab-highlight: #8a8a8a;
	swt-selected-highlight-top: true;	
	swt-tab-outline:#e5e5e5; 
	swt-tab-outer-keyline: #e5e5e5;
	swt-draw-custom-tab-content-background: true;
	swt-unselected-hot-tab-color-background:#ffffff;
}

#org-eclipse-ui-editorss CTabFolder.active {
	swt-selected-tab-highlight: #2160bb;
	swt-selected-highlight-top: true;
}

#org-eclipse-e4-ui-compatibility-editor Composite{
	background-color: #ffffff;
}

Composite.MPartSashContainer{
	background-color: '#org-eclipse-ui-workbench-SECONDARY_BACKGROUND';
}

Composite.MArea{
	background-color: #ffffff;
}

.MPart CTabFolder{
	swt-outer-keyline-color: #ffffff;
}


```



### common e4_globalstyle

```shell

$ cat /opt/JavaIDE/eclipse-ee/plugins/org.eclipse.ui.themes_1.2.2700.v20250122-1423/css/common/e4_globalstyle.css 
/*******************************************************************************
 * Copyright (c) 2020 IBM Corporation and others.
 *
 * This program and the accompanying materials
 * are made available under the terms of the Eclipse Public License 2.0
 * which accompanies this distribution, and is available at
 * https://www.eclipse.org/legal/epl-2.0/
 *
 * SPDX-License-Identifier: EPL-2.0
 *
 * Contributors:
 *     IBM Corporation - initial API and implementation
 *******************************************************************************/
 
.MTrimmedWindow.topLevel {
	margin-top: 0px;
	margin-bottom: 0px;
	margin-left: 0px;
	margin-right: 0px;
}

.MPartStack Tree, .MPartStack Table {
	font-family: '#org-eclipse-ui-workbench-TREE_TABLE_FONT';
}

```



---


## Light Style


### e4-light_globalstyle

```shell

cat /opt/JavaIDE/eclipse-ee/plugins/org.eclipse.ui.themes_1.2.2700.v20250122-1423/css/light/e4-light_globalstyle.css 
/*******************************************************************************
 * Copyright (c) 2010, 2020 IBM Corporation and others.
 *
 * This program and the accompanying materials
 * are made available under the terms of the Eclipse Public License 2.0
 * which accompanies this distribution, and is available at
 * https://www.eclipse.org/legal/epl-2.0/
 *
 * SPDX-License-Identifier: EPL-2.0
 *
 * Contributors:
 *     IBM Corporation - initial API and implementation
 *     Lars Vogel <Lars.Vogel@gmail.com> - Bug 420836
 *******************************************************************************/


Form, FormHeading {
	background-color: #ffffff;
	background: #ffffff;
	color: #505050;
}

Form {
	/* Bug 465148: Additional styling for the Form */
	text-background-color: #ffffff;

	tb-toggle-hover-color: #505050;
	tb-toggle-color: #505050;
	h-hover-full-color: #505050;
	h-hover-light-color: #505050;
	h-bottom-keyline-2-color: #eaeaea;
	h-bottom-keyline-1-color: #eaeaea;
}


Section {
	background-color: #ffffff;
	color: #505050;
	background-color-titlebar: #eaeaea;
	background-color-gradient-titlebar: #eaeaea;
	border-color-titlebar: #ffffff;
}

TabbedPropertyTitle > CLabel{
	color: #505050;
}

TabbedPropertyTitle {
	swt-backgroundGradientStart-color:  #eaeaea;
	swt-backgroundGradientEnd-color:    #eaeaea;
	swt-backgroundBottomKeyline1-color: #eaeaea;
	swt-backgroundBottomKeyline2-color: #eaeaea;
}

TabbedPropertyList {
	swt-tabNormalShadow-color   : '#org-eclipse-ui-workbench-INACTIVE_TAB_OUTLINE_COLOR';             /* color of shadow lines around the tabs */
	swt-tabDarkShadow-color     : '#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_SELECTED_TEXT_COLOR'; /* line color of the tiny scroll triangle (at top / at bottom) */
	swt-tabAreaBackground-color : #ffffff;
	swt-tabBackground-color     : '#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_BG_START';
	color                       : #505050; /* text color in the tab / tab area */
}

```




### e4-light_partstyle

```shell

$ cat /opt/JavaIDE/eclipse-ee/plugins/org.eclipse.ui.themes_1.2.2700.v20250122-1423/css/light/e4-light_partstyle.css 
/*******************************************************************************
 * Copyright (c) 2010, 2020 IBM Corporation and others.
 *
 * This program and the accompanying materials
 * are made available under the terms of the Eclipse Public License 2.0
 * which accompanies this distribution, and is available at
 * https://www.eclipse.org/legal/epl-2.0/
 *
 * SPDX-License-Identifier: EPL-2.0
 *
 * Contributors:
 *     IBM Corporation - initial API and implementation
 *     Lars Vogel <Lars.Vogel@gmail.com> - Bug 420836
 *******************************************************************************/


/* ################################ CSS for .MParts ########################## */

.MPart.busy {
	font-style: italic;
}

.MPart.highlighted {
	font-weight: bold;
}

.MPartStack, .MPart {
	font-family: '#org-eclipse-ui-workbench-TAB_TEXT_FONT';
}



```

### e4-light_ide_colorextensions

```shell

$ cat /opt/JavaIDE/eclipse-ee/plugins/org.eclipse.ui.themes_1.2.2700.v20250122-1423/css/light/e4-light_ide_colorextensions.css
/*******************************************************************************
 * Copyright (c) 2010, 2020 IBM Corporation and others.
 *
 * This program and the accompanying materials
 * are made available under the terms of the Eclipse Public License 2.0
 * which accompanies this distribution, and is available at
 * https://www.eclipse.org/legal/epl-2.0/
 *
 * SPDX-License-Identifier: EPL-2.0
 *
 * Contributors:
 *     IBM Corporation - initial API and implementation
 *     Lars Vogel <Lars.Vogel@gmail.com> - Bug 420836
 *******************************************************************************/

/* ColorDefinitions for the light theme for the Eclipse IDE
*
* ThemeExtensions and ColorDefinition are  mapped to the Colors and Fonts preference
* dialog in the IDE
*/

/* New ColorDefinitions for the E4 default theme */ 
ThemesExtension { color-definition: 
	'#org-eclipse-ui-workbench-INACTIVE_UNSELECTED_TABS_COLOR_START', 
	'#org-eclipse-ui-workbench-INACTIVE_UNSELECTED_TABS_COLOR_END',
	'#org-eclipse-ui-workbench-INACTIVE_TAB_OUTER_KEYLINE_COLOR',
	'#org-eclipse-ui-workbench-INACTIVE_TAB_INNER_KEYLINE_COLOR',
	'#org-eclipse-ui-workbench-INACTIVE_TAB_OUTLINE_COLOR',
	'#org-eclipse-ui-workbench-ACTIVE_UNSELECTED_TABS_COLOR_START',
	'#org-eclipse-ui-workbench-ACTIVE_UNSELECTED_TABS_COLOR_END',
	'#org-eclipse-ui-workbench-ACTIVE_TAB_OUTER_KEYLINE_COLOR',
	'#org-eclipse-ui-workbench-ACTIVE_TAB_INNER_KEYLINE_COLOR',
	'#org-eclipse-ui-workbench-ACTIVE_TAB_OUTLINE_COLOR',
	'#org-eclipse-ui-workbench-ACTIVE_TAB_TEXT_COLOR',
	'#org-eclipse-ui-workbench-INACTIVE_TAB_TEXT_COLOR',
	'#org-eclipse-ui-workbench-SECONDARY_BACKGROUND';
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_UNSELECTED_TABS_COLOR_START {
	color: #ffffff;
	category: '#org-eclipse-ui-presentation-default';
	label: url('platform:/plugin/org.eclipse.ui.themes?message=INACTIVE_UNSELECTED_TABS_COLOR_START')
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_UNSELECTED_TABS_COLOR_END {
	color: #ffffff;
	category: '#org-eclipse-ui-presentation-default';
	label: url('platform:/plugin/org.eclipse.ui.themes?message=INACTIVE_UNSELECTED_TABS_COLOR_END');
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_TAB_OUTER_KEYLINE_COLOR {
	color: #ffffff;
	category: '#org-eclipse-ui-presentation-default';
	label: url('platform:/plugin/org.eclipse.ui.themes?message=INACTIVE_TAB_OUTER_KEYLINE_COLOR');
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_TAB_INNER_KEYLINE_COLOR {
	color: #ffffff;
	category: '#org-eclipse-ui-presentation-default';
	label: url('platform:/plugin/org.eclipse.ui.themes?message=INACTIVE_TAB_INNER_KEYLINE_COLOR');
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_TAB_OUTLINE_COLOR {
	color: #b6bccc;
	category: '#org-eclipse-ui-presentation-default';
	label: url('platform:/plugin/org.eclipse.ui.themes?message=INACTIVE_TAB_OUTLINE_COLOR');
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_UNSELECTED_TABS_COLOR_START {
	color: #ffffff;
	category: '#org-eclipse-ui-presentation-default';
	label: url('platform:/plugin/org.eclipse.ui.themes?message=ACTIVE_UNSELECTED_TABS_COLOR_START');
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_UNSELECTED_TABS_COLOR_END {
	color: #ffffff;
	category: '#org-eclipse-ui-presentation-default';
	label: url('platform:/plugin/org.eclipse.ui.themes?message=ACTIVE_UNSELECTED_TABS_COLOR_END');
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_TAB_OUTER_KEYLINE_COLOR {
	color: #cccccc;
	category: '#org-eclipse-ui-presentation-default';
	label: url('platform:/plugin/org.eclipse.ui.themes?message=ACTIVE_TAB_OUTER_KEYLINE_COLOR');
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_TAB_INNER_KEYLINE_COLOR {
	color: #ffffff;
	category: '#org-eclipse-ui-presentation-default';
	label: url('platform:/plugin/org.eclipse.ui.themes?message=ACTIVE_TAB_INNER_KEYLINE_COLOR');
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_TAB_OUTLINE_COLOR {
	color: #b6bccc;
	category: '#org-eclipse-ui-presentation-default';
	label: url('platform:/plugin/org.eclipse.ui.themes?message=ACTIVE_TAB_OUTLINE_COLOR');
}

ColorDefinition#org-eclipse-ui-workbench-SECONDARY_BACKGROUND {
	color: #f8f8f8;
	category: '#org-eclipse-ui-presentation-default';
	label: url('platform:/plugin/org.eclipse.ui.themes?message=SECONDARY_BACKGROUND');
	editable: false;
}

/* Already existing ColorDefinitions overridden for the E4 default theme */
ColorDefinition#org-eclipse-ui-workbench-INACTIVE_TAB_BG_START {
	color: #dddfe5;
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_TAB_BG_END {
	color: #ffffff;
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_TAB_BG_START{
	color: #ffffff;
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_TAB_BG_END {
	color: #ffffff;
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_BG_START {
	color: #FFFFFF;
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_BG_END {
	color: #FFFFFF;
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_TEXT_COLOR {
	/* Never use black */
	color: #101010;
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_TAB_TEXT_COLOR {
	color: '#COLOR_WIDGET_FOREGROUND';
	category: '#org-eclipse-ui-presentation-default';
	label: url('platform:/plugin/org.eclipse.ui.themes?message=ACTIVE_TAB_TEXT_COLOR');
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_TAB_TEXT_COLOR {
	color: '#COLOR_WIDGET_FOREGROUND';
	category: '#org-eclipse-ui-presentation-default';
	label: url('platform:/plugin/org.eclipse.ui.themes?message=INACTIVE_TAB_TEXT_COLOR');
}


```





### e4-light_tabstyle


```shell

$ cat /opt/JavaIDE/eclipse-ee/plugins/org.eclipse.ui.themes_1.2.2700.v20250122-1423/css/light/e4-light_tabstyle.css 
/*******************************************************************************
 * Copyright (c) 2010, 2020 IBM Corporation and others.
 *
 * This program and the accompanying materials
 * are made available under the terms of the Eclipse Public License 2.0
 * which accompanies this distribution, and is available at
 * https://www.eclipse.org/legal/epl-2.0/
 *
 * SPDX-License-Identifier: EPL-2.0
 *
 * Contributors:
 *     IBM Corporation - initial API and implementation
 *     Lars Vogel <Lars.Vogel@gmail.com> - Bug 420836
 *     SAP SE - light theme improvements
 *******************************************************************************/


/* ################################ CSS for Tabs ########################## */

#org-eclipse-ui-editorss {
	swt-tab-height: 8px;
}

.MPartStack {
	swt-tab-renderer: url('bundleclass://org.eclipse.e4.ui.workbench.renderers.swt/org.eclipse.e4.ui.workbench.renderers.swt.CTabRendering');
	swt-selected-tab-fill: '#org-eclipse-ui-workbench-INACTIVE_TAB_BG_START' '#org-eclipse-ui-workbench-INACTIVE_TAB_BG_END' 100% 100%;
	swt-unselected-tabs-color: '#org-eclipse-ui-workbench-INACTIVE_UNSELECTED_TABS_COLOR_START' '#org-eclipse-ui-workbench-INACTIVE_UNSELECTED_TABS_COLOR_END' 100% 100%;
	swt-outer-keyline-color: '#org-eclipse-ui-workbench-INACTIVE_TAB_OUTER_KEYLINE_COLOR';
	swt-inner-keyline-color: '#org-eclipse-ui-workbench-INACTIVE_TAB_INNER_KEYLINE_COLOR';
	swt-tab-outline: '#org-eclipse-ui-workbench-INACTIVE_TAB_OUTLINE_COLOR';
	padding: 0px;
	color: '#org-eclipse-ui-workbench-INACTIVE_TAB_TEXT_COLOR';
	swt-draw-custom-tab-content-background: true;
	swt-unselected-hot-tab-color-background:#EAEAEA;
}

.MPartStack.active {
	swt-selected-tab-fill: '#org-eclipse-ui-workbench-ACTIVE_TAB_BG_START' '#org-eclipse-ui-workbench-ACTIVE_TAB_BG_END' 100% 100%;
	swt-unselected-tabs-color: '#org-eclipse-ui-workbench-ACTIVE_UNSELECTED_TABS_COLOR_START' '#org-eclipse-ui-workbench-ACTIVE_UNSELECTED_TABS_COLOR_END' 100% 100%;
	swt-outer-keyline-color: '#org-eclipse-ui-workbench-ACTIVE_TAB_OUTER_KEYLINE_COLOR';
	swt-inner-keyline-color: '#org-eclipse-ui-workbench-ACTIVE_TAB_INNER_KEYLINE_COLOR';
	swt-tab-outline: '#org-eclipse-ui-workbench-ACTIVE_TAB_OUTLINE_COLOR';
	swt-draw-custom-tab-content-background: true;
}

.MPartStack.active.noFocus {
	swt-selected-tab-fill: '#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_BG_START' '#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_BG_END' 100% 100%;
}

CTabItem:selected {
	color: '#org-eclipse-ui-workbench-ACTIVE_TAB_TEXT_COLOR';
}

CTabFolder.MArea {
	swt-tab-renderer: url('bundleclass://org.eclipse.e4.ui.workbench.renderers.swt/org.eclipse.e4.ui.workbench.renderers.swt.CTabRendering');
	padding: 0px;
}

CTabFolder {
	swt-selected-tab-highlight: none;
}

CTabFolder.active {
	swt-selected-tab-highlight: rgb(103,145,230);
	swt-selected-highlight-top: false;
}

.MPartStack.active.noFocus > CTabItem:selected {
	color: '#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_TEXT_COLOR';
}

.MPartStack > Composite {
	background-color: '#org-eclipse-ui-workbench-INACTIVE_TAB_BG_END';
}

.MPartStack.active > Composite {
	background-color: '#org-eclipse-ui-workbench-ACTIVE_TAB_BG_END';
}

.MPartStack.active.noFocus > Composite {
	background-color: '#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_BG_END';
}


```

### e4-light-drag-styling


```shell

$ cat /opt/JavaIDE/eclipse-ee/plugins/org.eclipse.ui.themes_1.2.2700.v20250122-1423/css/light/e4-light-drag-styling.css 
/*******************************************************************************
 * Copyright (c) 2010, 2020 IBM Corporation and others.
 *
 * This program and the accompanying materials
 * are made available under the terms of the Eclipse Public License 2.0
 * which accompanies this distribution, and is available at
 * https://www.eclipse.org/legal/epl-2.0/
 *
 * SPDX-License-Identifier: EPL-2.0
 *
 * Contributors:
 *     IBM Corporation - initial API and implementation
 *     Lars Vogel <Lars.Vogel@gmail.com> - Bug 420836
 *******************************************************************************/


/* ################################ CSS related to drag and drop ########################## */

.DragFeedback {
	background-color: COLOR-WIDGET-NORMAL-SHADOW;
}

.ModifiedDragFeedback {
	background-color: #A0A000;
}


```



---

## Dark Style



### e4-dark_globalstyle


```shell

$ cat /opt/JavaIDE/eclipse-ee/plugins/org.eclipse.ui.themes_1.2.2700.v20250122-1423/css/dark/e4-dark_globalstyle.css 
/*******************************************************************************
 * Copyright (c) 2010, 2015 Andrea Guarinoni and others.
 *
 * This program and the accompanying materials
 * are made available under the terms of the Eclipse Public License 2.0
 * which accompanies this distribution, and is available at
 * https://www.eclipse.org/legal/epl-2.0/
 *
 * SPDX-License-Identifier: EPL-2.0
 *
 * Contributors:
 *     Andrea Guarinoni <andrea.guarinoni.dev@outlook.com> - initial API and implementation
 *     Stefan Winkler <stefan@winklerweb.net> - Bug 434189, 430848
 *     Simon Scholz <simon.scholz@vogella.com> - Bug 431635
 *     Fabio Zadrozny <fabiofz@gmail.com> - Bug 465148, 465711
 *     Lars Vogel <Lars.Vogel@vogella.com> Bug 463652,466275
 *******************************************************************************/

/*******************************************************************************
 * The following bugs are referred to in this style sheet
 * 2.) Bug 419377 - Setting a property to 'inherit' is not supported
 * 3.) Bug 430051 - Regression for CTabRendering when drawing bottom tabs
 *******************************************************************************/


/* ############################## Global Styles ############################## */

Shell,
Composite, ScrolledComposite, ExpandableComposite, Canvas, TabFolder, CLabel, Label,
CoolBar, Sash, Group, RefactoringLocationControl, ChangeParametersControl, Link, FilteredTree,
ProxyEntriesComposite, NonProxyHostsComposite, DelayedFilterCheckboxTree,
Splitter, ScrolledPageContent, ViewForm, LaunchConfigurationFilteredTree,
ContainerSelectionGroup, BrowseCatalogItem, EncodingSettings,
ProgressMonitorPart, DocCommentOwnerComposite, NewServerComposite,
NewManualServerComposite, ServerTypeComposite, FigureCanvas,
DependenciesComposite, ListEditorComposite, WrappedPageBook,
CompareStructureViewerSwitchingPane, CompareContentViewerSwitchingPane,
QualifiedNameComponent, RefactoringStatusViewer,
MessageLine,
Button /* SWT-BUG: checkbox inner label font color is not accessible */,
Composite > *,
Composite > * > *,
Group > StyledText {
    background-color:'#org-eclipse-ui-workbench-DARK_BACKGROUND'; 
    color:'#org-eclipse-ui-workbench-DARK_FOREGROUND'; 
}

/* ############################## Toolbar ############################## */
/* Ensure that the labels in the tabfolder gets updated
   See Bug 552780
*/
TabFolder > *,
CTabFolder > *,
TabFolder > Composite > *, /* Composite > CommitSearchPage$... */
CTabFolder > Composite > *, /* Composite > CommitSearchPage$... */
TabFolder > Composite > * > * { /* [style~='SWT.NO_BACKGROUND'] <- generate E4 non-sense bugs in apparently not related other rules Composite > ContentMergeViewer$... > TextMergeViewer$... */ 
	color:'#org-eclipse-ui-workbench-DARK_FOREGROUND'; 
}

/* Toolbar should inherit the colors of its container to avoid drawing artifacts*/
ToolBar {
	background-color:inherit;	
}

Combo,
List,
Text,
Spinner,
CCombo {
    background-color:'#org-eclipse-ui-workbench-DARK_BACKGROUND'; 
    color:'#org-eclipse-ui-workbench-DARK_FOREGROUND'; 
}
Composite > StyledText,
Shell [style~='SWT.DROP_DOWN'] > StyledText, /* for eg. folded code popup (but it's ignored) */
SashForm > StyledText {
	/*	Fix StyledText inside a SashForm */
    background-color:'#org-eclipse-ui-workbench-DARK_BACKGROUND'; 
    color:'#org-eclipse-ui-workbench-DARK_FOREGROUND'; 
}

Text[style~='SWT.SEARCH'],
Text[style~='SWT.SEARCH'] + Label /* SWT-BUG: adjacent sibling selector is ignored (CSS2.1) */ {
    /* search boxes */
    background-color: #333;
    color: #F4F7F7;
}

Text[style~='SWT.READ_ONLY'] {
    background-color: '#org-eclipse-ui-workbench-DARK_BACKGROUND'; 
    color: #bbbbbb;
}

Shell Tree, Shell Table, Shell List {
	background-color: #2F2F2F;
}

DatePicker,
DatePicker > Text,
ScheduleDatePicker,
ScheduleDatePicker > Text {
    background-color:'#org-eclipse-ui-workbench-DARK_BACKGROUND'; 
    color:'#org-eclipse-ui-workbench-DARK_FOREGROUND'; 
}


ScrolledFormText,
FormText {
    background-color:'#org-eclipse-ui-workbench-DARK_BACKGROUND'; 
    color:'#org-eclipse-ui-workbench-DARK_FOREGROUND'; 
}

Table,
Tree,
RegistryFilteredTree {
    background-color:inherit;
    color:'#org-eclipse-ui-workbench-DARK_FOREGROUND'; 
}

Hyperlink,
ImageHyperlink {
	background-color: inherit;
    color: #6fc5ee;
}


ViewerPane,
DrillDownComposite {
    background-color: #232323;
    color: #CCC;
}

ProgressInfoItem,
ProgressInfoItem > *,
CompareViewerPane,
CompareViewerPane > * {
    background-color: inherit;
    color: '#org-eclipse-ui-workbench-DARK_FOREGROUND'; 
}

ProgressIndicator {
    background-color: #777;
    color: '#org-eclipse-ui-workbench-DARK_FOREGROUND'; 
}

DiscoveryItem,
DiscoveryItem Label,
DiscoveryItem Composite {
    background-color: #383C3E;
    color: #dddddd;
}
DiscoveryItem StyledText {
    background-color: #383C3E;
    color: #aaaaaa;
}
DiscoveryItem Link {
    background-color: #383C3E;
    color: #8B9498;
}

CatalogSwitcher,
CatalogSwitcher > ScrolledComposite > Composite > Composite /* ignored because hard-coded */,
CategoryItem {
    background-color: '#org-eclipse-ui-workbench-DARK_BACKGROUND'; 
    color: #dddddd;
}
GradientCanvas,
GradientCanvas > Label {
    background-color: #3f4447;
    color: #9ac9d8;
}
GradientCanvas {
    /* SWT-BUG workaround: GradientCanvas background-color is ignored */
    background: #3f4447;
}
CategoryItem > GradientCanvas,
CategoryItem > GradientCanvas > Label {
    /* SWT-BUG workaround: a style for background is not applied on GradientCanvas (CSS engine repaint issue) */
    background-color: #fafafa;
    color: #333;
}
CategoryItem > GradientCanvas {
    /* SWT-BUG workaround: a style for background is not applied on GradientCanvas (CSS engine repaint issue) */
    background: #fafafa;
    background-image: #333;
}

WebSite {
    background-color: #41464A;
    color: #dddddd;
}

Form,
FormHeading {
    background-color: #505F70;
    color: #9AC9D8;
}

Form {
	/* Bug 465148: Additional styling for the Form */
    text-background-color: #505F70;

	tb-toggle-hover-color: #313538;
	tb-toggle-color: #313538;
	h-hover-full-color: #313538;
	h-hover-light-color: #313538;
	h-bottom-keyline-2-color: #313538;
	h-bottom-keyline-1-color: #313538;

	/* We also have to force the background mode (the
	 * Label/ToolBar in the heading should inherit it).
	 */
    swt-background-mode: 'force';
}

Section {
    background-color: #4F5355;
    color: #AEBED0;
    background-color-titlebar: #4F5355;
    background-color-gradient-titlebar: #4F5355;
    border-color-titlebar: #4F5355;
    swt-titlebar-color: #cccccc;
	tb-toggle-hover-color: #F4F7F7;
	tb-toggle-color: #F4F7F7;
}

Table,
Tree {
	swt-header-color: #CCC;
	swt-header-background-color: #383D3F;
}

Twistie {
    color: #E8E4DF;
}

.MPartSashContainer {
    background-color: '#org-eclipse-ui-workbench-DARK_BACKGROUND'; 
    color: #EEEEEE;
}

HeapStatus {
	background-color: #4F5355;
	color: #EEEEEE;
}

PageSiteComposite, PageSiteComposite > CImageLabel {
    color: #EEEEEE;
}
PageSiteComposite > PropertyTable {
    background-color: #333;
    color: #EEEEEE;
}
PageSiteComposite > PropertyTable:disabled {
/* SWT-BUG: event is triggered but styles for PropertyTable are hard-coded */
    background-color: #444;
    color: #EEEEEE;
}

/* See Bug 430848: We need to override the theme of the Eclipse splash screen, because
 * otherwise the splash screen would be partly switched to the dark theme during startup,
 * which does not look very nice.
 */
Label#org-eclipse-ui-splash-progressText {
	background-color: inherit; /* transparent */
	color: #9c9696; /* see property startupForegroundColor in the product */
}

Label#org-eclipse-ui-buildid-text {
	background-color: inherit; /* transparent */
}

ProgressIndicator#org-eclipse-ui-splash-progressIndicator {
	background-color: #e1e1e1;
}

Link {
	swt-link-foreground-color: '#org-eclipse-ui-workbench-LINK_COLOR'
}

ExpandableComposite {
    swt-titlebar-color: #cccccc;
	tb-toggle-hover-color: #F4F7F7;
	tb-toggle-color: #F4F7F7;
}

TabbedPropertyTitle > CLabel{
	color: #9AC9D8;
}

TabbedPropertyTitle {
	swt-backgroundGradientStart-color:  #505F70;
	swt-backgroundGradientEnd-color:    #505F70;
	swt-backgroundBottomKeyline1-color: #505F70;
	swt-backgroundBottomKeyline2-color: #505F70;
}

TabbedPropertyList {
	swt-tabNormalShadow-color   : '#org-eclipse-ui-workbench-INACTIVE_TAB_OUTLINE_COLOR';             /* color of shadow lines around the tabs */
	swt-tabDarkShadow-color     : '#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_SELECTED_TEXT_COLOR'; /* line color of the tiny scroll triangle (at top / at bottom) */
	swt-tabAreaBackground-color : '#org-eclipse-ui-workbench-DARK_BACKGROUND';    /*same as canvas*/
	swt-tabBackground-color     : '#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_BG_START';
	color                       : '#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_SELECTED_TEXT_COLOR'; /* text color in the tab / tab area */
}



```

---

### e4-dark_partstyle

```shell

$ cat /opt/JavaIDE/eclipse-ee/plugins/org.eclipse.ui.themes_1.2.2700.v20250122-1423/css/dark/e4-dark_partstyle.css 
/*******************************************************************************
 * Copyright (c) 2010, 2014 Andrea Guarinoni and others.
 *
 * This program and the accompanying materials
 * are made available under the terms of the Eclipse Public License 2.0
 * which accompanies this distribution, and is available at
 * https://www.eclipse.org/legal/epl-2.0/
 *
 * SPDX-License-Identifier: EPL-2.0
 *
 * Contributors:
 *     Andrea Guarinoni <andrea.guarinoni.dev@outlook.com> - initial API and implementation
 *     Lars Vogel - initial API and implementation
 *******************************************************************************/


/* ################################ CSS for .MParts ########################## */

.MPart {
    font-family: '#org-eclipse-ui-workbench-TAB_TEXT_FONT';
    background-color: #292929;
    color: #DDDDDD;
}

.MPart.busy {
    font-style: italic;
}

.MPart.highlighted {
    font-weight: bold;
}

.MPart Composite,
.MPart Composite > *,
.MPart Composite > * > *,
.MPart Label,
.MPart ScrolledForm,
.MPart Form,
.MPart Section,
.MPart FormText,
.MPart Link,
.MPart Sash,
.MPart Button,
.MPart Group,
.MPart SashForm,
.MPart Tree,
.MPart FilteredTree,
.MPart RegistryFilteredTree,
.MPart PageSiteComposite,
.MPart DependenciesComposite,
.MPart Text[style~='SWT.READ_ONLY'],
.MPart FigureCanvas,
.MPart ListEditorComposite,
.MPart ScrolledComposite,
.Mpart ScrolledComposite ProgressInfoItem,
.MPart Form ScrolledPageBook,
.MPart DependenciesComposite > SashForm > Section > * { /* Section > DependenciesComposite$... */
    background-color: #2F2F2F;
    color: #AAAAAA;
}


.MPart Section > Label {
    background-color: #2F2F2F;
    color: #ABCEDA;
}

.MPart Table,
.MPart Browser,
.Mpart OleFrame,
.MPart ViewForm,
.MPart ViewForm > CLabel,
.MPart PageBook > Label,
.MPart PageBook > SashForm {
    background-color: #313538;
    color: #CCC;
}

.MPart Section Tree {
    background-color: #383A3B;
    color: #DDDDDD;
}

.MPart DatePicker,
.MPart DatePicker > Text,
.MPart ScheduleDatePicker,
.MPart ScheduleDatePicker > Text,
.MPart CCombo,
.MPart Spinner,
.MPart Composite > StyledText,
.MPart PageBook > SashForm Label,
.MPart SashForm > Text[style~='SWT.BORDER'] {
    background-color: #3f4447;
    color: #BBBBBB;
}

.MPart FormHeading,
.MPart FormHeading > TitleRegion,
.MPart FormHeading > TitleRegion > Label,
.MPart FormHeading > TitleRegion > StyledText {
    background-color: #505f70;
    color: #9ac9d8;
}

.MPart FormHeading,
.MPart FormHeading > TitleRegion {
    swt-background-mode: none;
}
.MPart FormHeading > CLabel {
    background-color: #505f70;
}

.MPartFormHeaderCLabelError {
	color:'#org-eclipse-ui-workbench-FORM_HEADING_ERROR_COLOR';
}
.MPartFormHeaderCLabelWarning {
	color:'#org-eclipse-ui-workbench-FORM_HEADING_WARNING_COLOR';
}
.MPartFormHeaderCLabelInfo {
	color:'#org-eclipse-ui-workbench-FORM_HEADING_INFO_COLOR';
}

/* ------------------------------------------------------------- */

#org-eclipse-jdt-ui-SourceView StyledText,
#org-eclipse-wst-jsdt-ui-SourceView StyledText {
    background-color: #252525;
}

/* ------------------------------------------------------------- */

#org-eclipse-ui-console-ConsoleView .MPart > Composite,
#org-eclipse-ui-console-ConsoleView .MPart StyledText,
#org-eclipse-ui-console-ConsoleView .MPart PageBook Label {
    background-color: #2F2F2F;
    color: #CCCCCC;
}

/* ------------------------------------------------------------- */

#org-eclipse-e4-ui-compatibility-editor Canvas {
	background-color: inherit;
}

#org-eclipse-e4-ui-compatibility-editor LayoutCanvas {
    background-color: #252525;
    color: #CCCCCC;
}



```


### e4-dark_preferencestyle

```shell

$ cat /opt/JavaIDE/eclipse-ee/plugins/org.eclipse.ui.themes_1.2.2700.v20250122-1423/css/dark/e4-dark_preferencestyle.css 
/*******************************************************************************
 * Copyright (c) 2014, 2015 Lars Vogel and others.
 *
 * This program and the accompanying materials
 * are made available under the terms of the Eclipse Public License 2.0
 * which accompanies this distribution, and is available at
 * https://www.eclipse.org/legal/epl-2.0/
 *
 * SPDX-License-Identifier: EPL-2.0
 *
 * Contributors:
 *     Lars Vogel <Lars.Vogel@gmail.com> - initial API and implementation
 *     Andrea Guarinoni - intial color schema definition
 *     Lars Vogel <Lars.Vogel@vogella.com> - Ongoing maintenance
 *******************************************************************************/

/* ############################## Eclipse UI properties ############################## */


IEclipsePreferences#org-eclipse-ui-editors:org-eclipse-ui-themes { /* pseudo attribute added to allow contributions without replacing this node, see Bug 466075 */
	preferences:
		'AbstractTextEditor.Color.Background.SystemDefault=false'
		'AbstractTextEditor.Color.SelectionForeground.SystemDefault=false'
		'AbstractTextEditor.Color.SelectionBackground.SystemDefault=false'
		'AbstractTextEditor.Color.Background=30,31,34'
		'AbstractTextEditor.Color.Foreground.SystemDefault=false'
		'AbstractTextEditor.Color.SelectionBackground=33,66,131'
		'AbstractTextEditor.Color.SelectionForeground=147,161,161'
		'AbstractTextEditor.Color.Foreground=204,204,204'
		'AbstractTextEditor.Color.FindScope=30,120,155'
		'asOccurencesIndicationColor=72,72,72'
		'breakpointIndicationColor=51,119,193'
		'currentIPColor=90,90,90'
		'currentLineColor=55,55,55'
		'deletionIndicationColor=224,226,228'
		'filteredSearchResultIndicationColor=27,98,145'
		'hyperlinkColor=102,175,249'
		'hyperlinkColor.SystemDefault=false'
		'infoIndicationColor=86,194,170'
		'lineNumberColor=119,145,154'
		'linked.slave.color=66,156,255'
		'matchingTagIndicationColor=72,72,72'
		'occurrenceIndicationColor=27,98,145'
		'overrideIndicatorColor=78,120,117'
		'printMarginColor=81,86,88'
		'searchResultHighlighting=false'
		'searchResultIndication=true'
		'searchResultIndicationColor=94,94,94'
		'searchResultTextStyle=BOX'
		'secondaryIPColor=90,90,90'
		'spellingIndicationColor=253,170,211'
		'writeOccurrenceIndicationColor=27,98,145'
		'org.eclipse.ui.editors.stickyLinesSeparatorColor=81,86,88'
}

IEclipsePreferences#org-eclipse-ui-workbench:org-eclipse-ui-themes { /* pseudo attribute added to allow contributions without replacing this node, see Bug 466075 */
	preferences:
		'ACTIVE_HYPERLINK_COLOR=138,201,242'
		'CONFLICTING_COLOR=240,15,66'
		'CONTENT_ASSIST_BACKGROUND_COLOR=52,57,61'
		'CONTENT_ASSIST_FOREGROUND_COLOR=238,238,238'
		'org.eclipse.ui.workbench.INFORMATION_BACKGROUND=81,86,88'
		'org.eclipse.ui.workbench.INFORMATION_FOREGROUND=238,238,238'
		'org.eclipse.ui.workbench.HOVER_BACKGROUND=52,57,61'
		'org.eclipse.ui.workbench.HOVER_FOREGROUND=238,238,238'
		'org.eclipse.ui.workbench.FORM_HEADING_ERROR_COLOR=255,110,110'
		'org.eclipse.ui.workbench.FORM_HEADING_WARNING_COLOR=255,200,0'
		'org.eclipse.ui.workbench.FORM_HEADING_INFO_COLOR=170,170,170'
		'ERROR_COLOR=247,68,117'
		'HYPERLINK_COLOR=111,197,238'
		'INCOMING_COLOR=31,179,235'
		'OUTGOING_COLOR=238,238,238'
		'RESOLVED_COLOR=108,210,17'
		'EDITION_COLOR=238,238,238'
		'org.eclipse.search.ui.match.highlight=206,92,0'
		'org.eclipse.ui.editors.rangeIndicatorColor=27,118,153'
		'org.eclipse.jface.REVISION_NEWEST_COLOR=75,44,3'
		'org.eclipse.jface.REVISION_OLDEST_COLOR=154,113,61'
}


```


### e4-dark_ide_colorextensions


```shell

$ cat /opt/JavaIDE/eclipse-ee/plugins/org.eclipse.ui.themes_1.2.2700.v20250122-1423/css/dark/e4-dark_ide_colorextensions.css 
/*******************************************************************************
 * Copyright (c) 2010, 2014 Andrea Guarinoni and others.
 *
 * This program and the accompanying materials
 * are made available under the terms of the Eclipse Public License 2.0
 * which accompanies this distribution, and is available at
 * https://www.eclipse.org/legal/epl-2.0/
 *
 * SPDX-License-Identifier: EPL-2.0
 *
 * Contributors:
 *     IBM Corporation - initial API and implementation
 *     Andrea Guarinoni - initial API and implementation
 *******************************************************************************/

/* ColorDefinitions for the dark theme for the Eclipse IDE
*
* ThemeExtensions and ColorDefinition are  mapped to the Colors and Fonts preference
* dialog in the IDE
*/

ThemesExtension { color-definition:
    '#org-eclipse-ui-workbench-DARK_BACKGROUND',
    '#org-eclipse-ui-workbench-DARK_FOREGROUND',
	'#org-eclipse-ui-workbench-INACTIVE_UNSELECTED_TABS_COLOR_START',
	'#org-eclipse-ui-workbench-INACTIVE_UNSELECTED_TABS_COLOR_END',
    '#org-eclipse-ui-workbench-INACTIVE_TAB_BG_START',
    '#org-eclipse-ui-workbench-INACTIVE_TAB_BG_END',
	'#org-eclipse-ui-workbench-INACTIVE_TAB_OUTER_KEYLINE_COLOR',
	'#org-eclipse-ui-workbench-INACTIVE_TAB_INNER_KEYLINE_COLOR',
	'#org-eclipse-ui-workbench-INACTIVE_TAB_OUTLINE_COLOR',
	'#org-eclipse-ui-workbench-INACTIVE_TAB_TEXT_COLOR',
    '#org-eclipse-ui-workbench-INACTIVE_TAB_UNSELECTED_TEXT_COLOR',
    '#org-eclipse-ui-workbench-INACTIVE_TAB_SELECTED_TEXT_COLOR',
    '#org-eclipse-ui-workbench-ACTIVE_UNSELECTED_TABS_COLOR_START',
	'#org-eclipse-ui-workbench-ACTIVE_UNSELECTED_TABS_COLOR_END',
    '#org-eclipse-ui-workbench-ACTIVE_TAB_BG_START',
    '#org-eclipse-ui-workbench-ACTIVE_TAB_BG_END',
	'#org-eclipse-ui-workbench-ACTIVE_TAB_OUTER_KEYLINE_COLOR',
	'#org-eclipse-ui-workbench-ACTIVE_TAB_INNER_KEYLINE_COLOR',
	'#org-eclipse-ui-workbench-ACTIVE_TAB_OUTLINE_COLOR',
	'#org-eclipse-ui-workbench-ACTIVE_TAB_TEXT_COLOR',
    '#org-eclipse-ui-workbench-ACTIVE_TAB_UNSELECTED_TEXT_COLOR',
    '#org-eclipse-ui-workbench-ACTIVE_TAB_SELECTED_TEXT_COLOR',
    '#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_BG_START',
    '#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_BG_END',
    '#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_TEXT_COLOR',
    '#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_SELECTED_TEXT_COLOR',
    '#org-eclipse-ui-workbench-LINK_COLOR';
}

ColorDefinition#org-eclipse-ui-workbench-DARK_BACKGROUND {
	/* color: #515658; */
	color: #48484c;
	category: '#org-eclipse-ui-presentation-default';
	label: url('platform:/plugin/org.eclipse.ui.themes?message=DARK_BACKGROUND');
}

ColorDefinition#org-eclipse-ui-workbench-DARK_FOREGROUND {
	color: #eeeeee;
	category: '#org-eclipse-ui-presentation-default';
	label: url('platform:/plugin/org.eclipse.ui.themes?message=DARK_FOREGROUND');
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_UNSELECTED_TABS_COLOR_START {
	color: #515658;
	category: '#org-eclipse-ui-presentation-default';
	label: url('platform:/plugin/org.eclipse.ui.themes?message=INACTIVE_UNSELECTED_TABS_COLOR_START');
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_UNSELECTED_TABS_COLOR_END {
	color: #464649;
	category: '#org-eclipse-ui-presentation-default';
	label: url('platform:/plugin/org.eclipse.ui.themes?message=INACTIVE_UNSELECTED_TABS_COLOR_END');
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_TAB_BG_START {
    color: #3B4042;
    category: '#org-eclipse-ui-presentation-default';
    label: url('platform:/plugin/org.eclipse.ui.themes?message=INACTIVE_TAB_BG_START');
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_TAB_BG_END {
    color: #313538;
    category: '#org-eclipse-ui-presentation-default';
    label: url('platform:/plugin/org.eclipse.ui.themes?message=INACTIVE_TAB_BG_END');
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_TAB_OUTER_KEYLINE_COLOR {
	color: #515658;
	category: '#org-eclipse-ui-presentation-default';
	label: url('platform:/plugin/org.eclipse.ui.themes?message=INACTIVE_TAB_OUTER_KEYLINE_COLOR');
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_TAB_INNER_KEYLINE_COLOR {
	color: #515658;
	category: '#org-eclipse-ui-presentation-default';
	label: url('platform:/plugin/org.eclipse.ui.themes?message=INACTIVE_TAB_INNER_KEYLINE_COLOR');
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_TAB_OUTLINE_COLOR {
	color: #3B4042;
	category: '#org-eclipse-ui-presentation-default';
	label: url('platform:/plugin/org.eclipse.ui.themes?message=INACTIVE_TAB_OUTLINE_COLOR');
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_TAB_TEXT_COLOR {
    color: #BBBBBB;
    category: '#org-eclipse-ui-presentation-default';
    label: url('platform:/plugin/org.eclipse.ui.themes?message=INACTIVE_TAB_TEXT_COLOR');
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_TAB_UNSELECTED_TEXT_COLOR {
    color: #BBBBBB;
    category: '#org-eclipse-ui-presentation-default';
    label: url('platform:/plugin/org.eclipse.ui.themes?message=INACTIVE_TAB_UNSELECTED_TEXT_COLOR');
}

ColorDefinition#org-eclipse-ui-workbench-INACTIVE_TAB_SELECTED_TEXT_COLOR {
    color: #FFFFFF;
    category: '#org-eclipse-ui-presentation-default';
    label: url('platform:/plugin/org.eclipse.ui.themes?message=INACTIVE_TAB_SELECTED_TEXT_COLOR');
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_UNSELECTED_TABS_COLOR_START {
	color: #49484C;
	category: '#org-eclipse-ui-presentation-default';
	label: url('platform:/plugin/org.eclipse.ui.themes?message=ACTIVE_UNSELECTED_TABS_COLOR_START');
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_UNSELECTED_TABS_COLOR_END {
	color: #48484C;
	category: '#org-eclipse-ui-presentation-default';
	label: url('platform:/plugin/org.eclipse.ui.themes?message=ACTIVE_UNSELECTED_TABS_COLOR_END');
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_TAB_BG_START {
    color: #48484C;
    category: '#org-eclipse-ui-presentation-default';
    label: url('platform:/plugin/org.eclipse.ui.themes?message=ACTIVE_TAB_BG_START');
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_TAB_BG_END {
    color: #48484C;
    category: '#org-eclipse-ui-presentation-default';
    label: url('platform:/plugin/org.eclipse.ui.themes?message=ACTIVE_TAB_BG_END');
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_TAB_OUTER_KEYLINE_COLOR {
	color: #646464;
	category: '#org-eclipse-ui-presentation-default';
	label: url('platform:/plugin/org.eclipse.ui.themes?message=ACTIVE_TAB_OUTER_KEYLINE_COLOR');
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_TAB_INNER_KEYLINE_COLOR {
	color: #4B4C4F;
	category: '#org-eclipse-ui-presentation-default';
	label: url('platform:/plugin/org.eclipse.ui.themes?message=ACTIVE_TAB_INNER_KEYLINE_COLOR');
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_TAB_OUTLINE_COLOR {
	color:#646464;
	category: '#org-eclipse-ui-presentation-default';
	label: url('platform:/plugin/org.eclipse.ui.themes?message=ACTIVE_TAB_OUTLINE_COLOR');
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_TAB_TEXT_COLOR {
    color: #BBBBBB;
    category: '#org-eclipse-ui-presentation-default';
    label: url('platform:/plugin/org.eclipse.ui.themes?message=ACTIVE_TAB_TEXT_COLOR');
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_TAB_UNSELECTED_TEXT_COLOR {
    color: #BBBBBB;
    category: '#org-eclipse-ui-presentation-default';
    label: url('platform:/plugin/org.eclipse.ui.themes?message=ACTIVE_TAB_UNSELECTED_TEXT_COLOR');
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_TAB_SELECTED_TEXT_COLOR {
    color: #FFFFFF;
    category: '#org-eclipse-ui-presentation-default';
    label: url('platform:/plugin/org.eclipse.ui.themes?message=ACTIVE_TAB_SELECTED_TEXT_COLOR');
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_BG_START {
    color: #2B2C2D;
    category: '#org-eclipse-ui-presentation-default';
    label: url('platform:/plugin/org.eclipse.ui.themes?message=ACTIVE_NOFOCUS_TAB_BG_START');
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_BG_END {
    color: #292929;
    category: '#org-eclipse-ui-presentation-default';
    label: url('platform:/plugin/org.eclipse.ui.themes?message=ACTIVE_NOFOCUS_TAB_BG_END');
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_TEXT_COLOR {
    color: #FFFFFF;
    category: '#org-eclipse-ui-presentation-default';
    label: url('platform:/plugin/org.eclipse.ui.themes?message=ACTIVE_NOFOCUS_TAB_TEXT_COLOR');
}

ColorDefinition#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_SELECTED_TEXT_COLOR {
    color: #FFFFFF;
    category: '#org-eclipse-ui-presentation-default';
    label: url('platform:/plugin/org.eclipse.ui.themes?message=ACTIVE_NOFOCUS_TAB_SELECTED_TEXT_COLOR');
}

ColorDefinition#org-eclipse-ui-workbench-LINK_COLOR {
    color: #6FC5EE;
    category: '#org-eclipse-ui-presentation-default';
    label: url('platform:/plugin/org.eclipse.ui.themes?message=LINK_COLOR');
}


```

### e4-dark_tabstyle


```shell

$ cat /opt/JavaIDE/eclipse-ee/plugins/org.eclipse.ui.themes_1.2.2700.v20250122-1423/css/dark/e4-dark_tabstyle.css 
/*******************************************************************************
 * Copyright (c) 2018 Andrea Guarinoni and others.
 *
 * This program and the accompanying materials
 * are made available under the terms of the Eclipse Public License 2.0
 * which accompanies this distribution, and is available at
 * https://www.eclipse.org/legal/epl-2.0/
 *
 * SPDX-License-Identifier: EPL-2.0
 *
 * Contributors:
 *     Andrea Guarinoni <andrea.guarinoni.dev@outlook.com> - initial API and implementation
 *     Lars Vogel - initial API and implementation
 *******************************************************************************/


/* ################################ CSS for Tabs ########################## */

#org-eclipse-ui-editorss {
	swt-tab-height: 8px;
}

.MPartStack {
    font-family: '#org-eclipse-ui-workbench-TAB_TEXT_FONT';
    swt-tab-renderer: url('bundleclass://org.eclipse.e4.ui.workbench.renderers.swt/org.eclipse.e4.ui.workbench.renderers.swt.CTabRendering');
}

CTabFolder {
    /* Set the styles for the inner tabs: */
    color: '#org-eclipse-ui-workbench-INACTIVE_TAB_TEXT_COLOR';
    swt-tab-renderer: url('bundleclass://org.eclipse.e4.ui.workbench.renderers.swt/org.eclipse.e4.ui.workbench.renderers.swt.CTabRendering');
    swt-tab-outline: '#org-eclipse-ui-workbench-ACTIVE_TAB_OUTLINE_COLOR'; /* border color for selected tab */
    swt-outer-keyline-color: '#org-eclipse-ui-workbench-ACTIVE_TAB_OUTER_KEYLINE_COLOR'; /* border color for whole tabs container */
    swt-unselected-tabs-color: '#org-eclipse-ui-workbench-ACTIVE_UNSELECTED_TABS_COLOR_START' '#org-eclipse-ui-workbench-ACTIVE_UNSELECTED_TABS_COLOR_END' 100% 100%; /* title background for unselected tab */
    swt-selected-tab-fill: '#org-eclipse-ui-workbench-ACTIVE_TAB_BG_END'; /* title background for selected tab */
    swt-unselected-hot-tab-color-background: #161616; /* Bug 465711 */
    swt-selected-tab-highlight: none;
}

CTabFolder[style~='SWT.DOWN'][style~='SWT.BOTTOM'] {
    /* Set the styles for the bottom inner tabs (Bug 430051): */
    swt-tab-renderer: url('bundleclass://org.eclipse.e4.ui.workbench.renderers.swt/org.eclipse.e4.ui.workbench.renderers.swt.CTabRendering');
    swt-unselected-hot-tab-color-background: #161616;/*  Bug 465711 */
    swt-selected-tab-highlight: #316c9b;
    swt-selected-highlight-top: false;
}

CTabFolder.active {
    swt-selected-tab-highlight: #316c9b;
    swt-selected-highlight-top: false;
}

CTabItem,
CTabItem CLabel {
    background-color: '#org-eclipse-ui-workbench-ACTIVE_TAB_BG_END'; /* HACK for background of CTabFolder inner Toolbars */
    color: '#org-eclipse-ui-workbench-INACTIVE_TAB_UNSELECTED_TEXT_COLOR';
}

CTabItem:selected,
CTabItem:selected CLabel {
    color: '#org-eclipse-ui-workbench-INACTIVE_TAB_SELECTED_TEXT_COLOR';
}

.MPartStack.active > CTabItem,
.MPartStack.active > CTabItem CLabel {
    background-color: '#org-eclipse-ui-workbench-ACTIVE_TAB_BG_END'; /* HACK for background of CTabFolder inner Toolbars */
    color: '#org-eclipse-ui-workbench-ACTIVE_TAB_UNSELECTED_TEXT_COLOR';
}
.MPartStack.active > CTabItem:selected,
.MPartStack.active > CTabItem:selected CLabel {
    color: '#org-eclipse-ui-workbench-ACTIVE_TAB_SELECTED_TEXT_COLOR';
}

.MPartStack.active.noFocus > CTabItem:selected {
    color: '#org-eclipse-ui-workbench-ACTIVE_NOFOCUS_TAB_SELECTED_TEXT_COLOR';
}

CTabFolder > Composite#ToolbarComposite {
  background-color: '#org-eclipse-ui-workbench-ACTIVE_TAB_BG_END'; /* HACK for background of CTabFolder inner Toolbars */
}

CTabFolder.MArea CTabItem, 
CTabFolder.MArea CTabItem CLabel {
    background-color: '#org-eclipse-ui-workbench-DARK_BACKGROUND';  /* Disable HACK for background of CTabFolder inner Toolbars */
}

CTabItem.busy {
    color: #888888;
}


```






