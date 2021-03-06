# Fire-Ant
Fire-Ant 是Ant-Design框架的Angular(4.*)实现的，可用作PC Web应用开发的UI框架。

Fire-Ant 是在参考Ant-Design的源码基础上，采用了更加简洁的实现，此外，在css格式上采用Sass代替了Less。封装后的组件更加灵活方便，使开发人员可以更加专注于业务的实现，可以极大减少前端开发时间。

FireAnt的中文名为“火蚁”，火蚁是蚂蚁团体的巧手匠，它们以在水中筑筏而著称，在影片《蚁人》中蚁人利用一个蚁筏通过了下水道。希望FireAnt能为前端开发人员和创业者们逢山开路、遇水搭桥，勇往直前。

- [Ant-Design](https://ant.design/index-cn) 由阿里巴巴的蚂蚁金服体验技术部出品，提供了丰富、灵活、实用的基础组件，基于React技术实现，对于喜欢Angular的童鞋来说，Fire-Ant无疑是一个值得选择的开发框架。

- [Angular](https://github.com/angular/angular) is a development platform for building mobile and desktop web applications using Typescript/JavaScript (JS) and other languages.


## Components

* Genernel
<table>
    <thead>
        <tr>
            <th>组件</th>
            <th>标签</th>
            <th>进度</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Button 按钮</td>
            <td>&lt;ant-button&gt;</td>
            <td>已完成(Done)</td>
        </tr>
        <tr>
            <td>Icon 图标</td>
            <td>&lt;ant-icon&gt;</td>
            <td>已完成(Done)</td>
        </tr>
    </tbody>
</table>

> Button 按钮：
```html
<ant-button type="primary">Primary</ant-button>
```
> Icon 图标：
```html
<ant-icon type="down"></ant-icon>
```

* Layout
<table>
    <thead>
        <tr>
            <th>组件</th>
            <th>标签</th>
            <th>进度</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Grid 栅格 - Row</td>
            <td>&lt;ant-row&gt;</td>
            <td>已完成(Done)</td>
        </tr>
        <tr>
            <td>Grid 栅格 - Col</td>
            <td>&lt;ant-col&gt;</td>
            <td>已完成(Done)</td>
        </tr>
        <tr>
            <td>Layout 布局</td>
            <td>
                &lt;ant-layout&gt;
            </td>
            <td>已完成(Done)</td>
        </tr>
        <tr>
            <td>Layout 布局 - Header</td>
            <td>
                &lt;ant-layout-header&gt;
            </td>
            <td>已完成(Done)</td>
        </tr>
        <tr>
            <td>Layout 布局 - Content</td>
            <td>
                &lt;ant-layout-content&gt;
            </td>
            <td>已完成(Done)</td>
        </tr>
        <tr>
            <td>Layout 布局 - Footer</td>
            <td>
                &lt;ant-layout-footer&gt;
            </td>
            <td>已完成(Done)</td>
        </tr>
        <tr>
            <td>Layout 布局 - Sider</td>
            <td>
                &lt;ant-layout-sider&gt;
            </td>
            <td>已完成(Done)</td>
        </tr>
    </tbody>
</table>

> Grid 栅格：
```html
<ant-row>
    <ant-col [span]="12">col-12</ant-col>
    <ant-col [span]="12">col-12</ant-col>
</ant-row>
```
> Layout 布局：
```html
<ant-layout>
    <ant-layout-sider>Sider</ant-layout-sider>
    <ant-layout>
        <ant-layout-header>Header</ant-layout-header>
        <ant-layout-content>Content</ant-layout-content>
        <ant-layout-footer>Footer</ant-layout-footer>
    </ant-layout>
</ant-layout>
```

* Navigation
<table>
    <thead>
        <tr>
            <th>组件</th>
            <th>标签</th>
            <th>进度</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Affix 固钉</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>Breadcrumb 面包屑</td>
            <td>&lt;ant-breadcrumb&gt;</td>
            <td>已完成(Done)</td>
        </tr>
        <tr>
            <td>BackTop 回到顶部</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>Dropdown 下拉菜单</td>
            <td>&lt;ant-dropdown-button&gt;</td>
            <td>已完成(Done)</td>
        </tr>
        <tr>
            <td>Menu 导航菜单</td>
            <td>&lt;ant-menu&gt;</td>
            <td>已完成(Done)</td>
        </tr>
        <tr>
            <td>Pagination 分页</td>
            <td>&lt;ant-pagination&gt;</td>
            <td>已完成(Done)</td>
        </tr>
        <tr>
            <td>Steps 步骤条</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
    </tbody>
</table>

> Breadcrumb 面包屑：
```html
<ant-breadcrumb>
      <ant-breadcrumb-item>Home</ant-breadcrumb-item>
      <ant-breadcrumb-item><a href="">Application Center</a></ant-breadcrumb-item>
      <ant-breadcrumb-item><a href="">Application List</a></ant-breadcrumb-item>
      <ant-breadcrumb-item>An Application</ant-breadcrumb-item>
</ant-breadcrumb>
```

> Dropdown 下拉菜单：
```html
<ant-dropdown-button>
    <ant-button (click)="onButtonClick($event)">Dropdown</ant-button>
    <ant-menu (menuClick)="onMenuClick($event)">
        <ant-menu-item key="1">1st menu item</ant-menu-item>
        <ant-menu-item key="2">2nd memu item</ant-menu-item>
        <ant-menu-item key="3">3d menu item</ant-menu-item>
    </ant-menu>
</ant-dropdown-button>

<a class="dropdown-link" href="javascript:;" dropdown>
    Hover me <ant-icon type="down"></ant-icon>
    <ant-menu>
        <ant-menu-item>
            <a target="_blank" rel="noopener noreferrer" href="http://www.alipay.com/">1st menu item</a>
        </ant-menu-item>
        <ant-menu-item>
            <a target="_blank" rel="noopener noreferrer" href="http://www.taobao.com/">2nd menu item</a>
        </ant-menu-item>
        <ant-menu-item>
            <a target="_blank" rel="noopener noreferrer" href="http://www.tmall.com/">3d menu item</a>
        </ant-menu-item>
    </ant-menu>
</a>
```

> Menu 导航菜单：
```html
<ant-submenu key="sub1">
    <div ant-submenu-title>
        <ant-icon type="mail"></ant-icon> Menu One
    </div>
    <ant-menu-item key="1">Option 1</ant-menu-item>
    <ant-menu-item key="2">Option 2</ant-menu-item>
    <ant-menu-item key="3">Option 3</ant-menu-item>
    <ant-menu-item key="4">Option 4</ant-menu-item>
    </ant-submenu>
    <ant-submenu key="sub2">
    <div ant-submenu-title>
        <ant-icon type="appstore"></ant-icon> Menu Two
    </div>
    <ant-menu-item key="5">Option 5</ant-menu-item>
    <ant-menu-item key="6">Option 6</ant-menu-item>
    <ant-submenu key="sub3">
        <div ant-submenu-title>Submenu</div>
        <ant-menu-item key="7">Option 7</ant-menu-item>
        <ant-menu-item key="8">Option 8</ant-menu-item>
    </ant-submenu>
    </ant-submenu>
    <ant-submenu key="sub4">
    <div ant-submenu-title>
        <ant-icon type="setting"></ant-icon> Menu Three
    </div>
    <ant-menu-item key="9">Option 9</ant-menu-item>
    <ant-menu-item key="10">Option 10</ant-menu-item>
    <ant-menu-item key="11">Option 11</ant-menu-item>
    <ant-menu-item key="12">Option 12</ant-menu-item>
    </ant-submenu>
</ant-menu>
```

> Pagination 分页：
```html
<ant-pagination [current]="1" [total]="50" (pageChange)="onPageChange($event)"></ant-pagination>
```

* Data Entry
<table>
    <thead>
        <tr>
            <th>组件</th>
            <th>标签</th>
            <th>进度</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>AutoComplete 自动完成</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>Checkbox 多选框</td>
            <td>&lt;ant-checkbox&gt;</td>
            <td>已完成(Done)</td>
        </tr>
        <tr>
            <td>Cascader 级联选择</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>DatePicker 日期选择框</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>Form 表单</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>InputNumber 数字输入框</td>
            <td>&lt;ant-number&gt;</td>
            <td>已完成(Done)</td>
        </tr>
        <tr>
            <td>Input 输入框</td>
            <td>&lt;ant-input&gt;</td>
            <td>已完成(Done)</td>
        </tr>
        <tr>
            <td>Mention 提及</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>Rate 评分</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>Radio 单选框</td>
            <td>&lt;ant-radio&gt;</td>
            <td>已完成(Done)</td>
        </tr>
        <tr>
            <td>Switch 开关</td>
            <td>&lt;ant-switch&gt;</td>
            <td>已完成(Done)</td>
        </tr>
        <tr>
            <td>Slider 滑动输入条</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>Select 选择器</td>
            <td>&lt;ant-select&gt;</td>
            <td>已完成(Done)</td>
        </tr>
        <tr>
            <td>TreeSelect 树选择</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>Transfer 穿梭框</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>TimePicker 时间选择框</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>Upload 上传</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
    </tbody>
</table>

> Checkbox 多选框：
```html
<ant-checkbox-group [(ngModel)]="example4.group1" (change)="onChange($event)">
    <ant-checkbox value="Apple">Apple</ant-checkbox>
    <ant-checkbox value="Pear">Pear</ant-checkbox>
    <ant-checkbox value="Orange">Orange</ant-checkbox>
</ant-checkbox-group>
```

> InputNumber 数字输入框：
```html
<ant-number [min]="1" [max]="10" (change)="onChange($event)"
    [(ngModel)]="example1.value1"></ant-number>
```

> Input 输入框：
```html
<ant-input placeholder="Basic usage" [(ngModel)]="example1.value"></ant-input>

<ant-addon style="margin-bottom: 16px">
    <addon-before>http://</addon-before>
    <addon-after>.com</addon-after>
    <ant-input [(ngModel)]="example2.value1"></ant-input>
</ant-addon>

<ant-input placeholder="Enter your userName" [(ngModel)]="example5.username">
    <input-prefix>
        <ant-icon type="user"></ant-icon>
    </input-prefix>
    <input-suffix>
        <ant-icon type="close-circle"></ant-icon>
    </input-suffix>
</ant-input>

<ant-input type="textarea" [(ngModel)]="example4.value1" placeholder="Autosize height based on content lines" [autosize]="true"></ant-input>
```

> Radio 单选框：
```html
<ant-radio-group [(ngModel)]="example3.group1" (change)="onGroupChange($event)">
    <ant-radio value="1">A</ant-radio>
    <ant-radio value="2">B</ant-radio>
    <ant-radio value="3">C</ant-radio>
    <ant-radio value="4">D</ant-radio>
</ant-radio-group>

<ant-radio-group mode="button" [(ngModel)]="example5.group1" (change)="onGroupChange($event)">
    <ant-radio value="a">Hangzhou</ant-radio>
    <ant-radio value="b">Shanghai</ant-radio>
    <ant-radio value="c">Beijing</ant-radio>
    <ant-radio value="d">Chengdu</ant-radio>
</ant-radio-group>
```

> Switch 开关：
```html
<ant-switch (change)="onChange($event)"></ant-switch>

<ant-switch (change)="onChange($event)" checkedText="开" uncheckedText="关"></ant-switch>
```

> Select 选择器：
```html
单选模式 (default)：
<ant-select [(ngModel)]="example6.value1"
    [size]="example6.size" style="width: 200px;">
    <ant-option *ngFor="let i of getNumRange()" [value]="i">
        选项{{i}}
    </ant-option>
</ant-select>

combobox模式：
<ant-select [(ngModel)]="example6.value2"
    [size]="example6.size" mode="combobox" style="width: 200px;">
    <ant-option *ngFor="let i of getNumRange()" [value]="i">
        选项{{i}}
    </ant-option>
</ant-select>

multiple模式：
<ant-select [(ngModel)]="example6.value3"
    placeholder="Please select"
    [size]="example6.size" mode="multiple" style="width: 100%;">
    <ant-option *ngFor="let i of getNumRange()" [value]="i">
        选项{{i}}
    </ant-option>
</ant-select>

tags模式：
<ant-select [(ngModel)]="example6.value4"
    placeholder="Please select"
    [size]="example6.size" mode="tags" style="width: 100%;">
    <ant-option *ngFor="let i of getNumRange()" [value]="i">
        选项{{i}}
    </ant-option>
</ant-select>
```

* Data Display
<table>
    <thead>
        <tr>
            <th>组件</th>
            <th>标签</th>
            <th>进度</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Avatar 头像</td>
            <td>&lt;ant-avatar&gt;</td>
            <td>已完成(Done)</td>
        </tr>
        <tr>
            <td>Badge 徽标数</td>
            <td>&lt;ant-badge&gt;</td>
            <td>已完成(Done)</td>
        </tr>
        <tr>
            <td>Collapse 折叠面板</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>Carousel 走马灯</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>Card 卡片</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>Calendar 日历</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>Popover气泡卡片</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>Tree 树形控件</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>Tooltip 文字提示器</td>
            <td>&lt;ant-tooltip&gt;</td>
            <td>已完成(Done)</td>
        </tr>
        <tr>
            <td>Timeline 时间轴</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>Tag 标签</td>
            <td>&lt;ant-tag&gt;</td>
            <td>已完成(Done)</td>
        </tr>
        <tr>
            <td>Tabs 标签页</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>Table 表格</td>
            <td>&lt;ant-table&gt;</td>
            <td>已完成(Done)</td>
        </tr>
    </tbody>
</table>

> Avatar 头像：
```html
<ant-avatar icon="user"></ant-avatar>
<ant-avatar><ant-avatar-text>U</ant-avatar-text></ant-avatar>
<ant-avatar src="https://zos.alipayobjects.com/rmsportal/ODTLcjxAfvqbxHnVXCYX.png"></ant-avatar>
```

> Badge 徽标数：
```html
<ant-badge [count]="5" [showZero]="true">
    <a href="#" class="head-example"></a>
</ant-badge>

<ant-badge [dot]="true">
    <ant-icon type="notification"></ant-icon>
</ant-badge>

<ant-badge status="success"></ant-badge>
<ant-badge status="error"></ant-badge>
<ant-badge status="default"></ant-badge>
<ant-badge status="processing"></ant-badge>
<ant-badge status="warning"></ant-badge>
```

> Tooltip 文字提示器：
```html
<span antTooltip title="prompt text">Tooltip will show when mouse enter.</span>
```

> Tag 标签：
```html
<ant-tag [closable]="true" (beforeClose)="beforeClose($event)" (close)="afterClose($event)">Tag 1</ant-tag>
```

> Table 表格：
```html
<ant-table>
    <table-header>这是表格标题</table-header>
    <table-content>
        <thead>
            <tr>
                <th>姓名</th>
                <th>年龄</th>
                <th>地址</th>
                <th>操作</th>
            </tr>
        </thead>
        <tbody>
            <tr *ngFor="let item of getExample1Data()">
                <td>{{item.name}}</td>
                <td>{{item.age}}</td>
                <td>{{item.address}}</td>
                <td>
                    <a href="#">编辑</a>
                    <span class="ant-divider"></span>
                    <a href="#">删除</a>
                    <span class="ant-divider"></span>
                    <a href="#" class="ant-dropdown-link">
                        更多 <ant-icon type="down"></ant-icon>
                    </a>
                </td>
            </tr>
        </tbody>
    </table-content>
    <table-footer>这是表格注脚</table-footer>
</ant-table>
```

* Feedback
<table>
    <thead>
        <tr>
            <th>组件</th>
            <th>标签</th>
            <th>进度</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Alert 警告提示</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>Modal 对话框</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>Message 全局提示</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>Notification 通知提醒框</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>Progress 进度条</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>Popconfirm 气泡确认框</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
        <tr>
            <td>Spin 加载中</td>
            <td> </td>
            <td>待开发 (Pending)</td>
        </tr>
    </tbody>
</table>





## Install

```bash
npm install fire-ant --save
```

如果下载速度较慢，可以尝试加入[淘宝 NPM 镜像](http://npm.taobao.org)，以加快模块下载速度。

```bash
npm install -g cnpm --registry=https://registry.npm.taobao.org
```

然后通过cnpm命令来安装：
```bash
cnpm install fire-ant --save
```

## Quickstart

直接下载本工程，并启动运行查看Demo：
```bash
git clone https://github.com/fbchen/fire-ant-example.git
cd fire-ant-example
cnpm install
```

下载后，通过开发工具[VSCode](http://code.visualstudio.com/Download)打开安装目录，点击调试“启动程序”，然后在浏览器中输入 http://localhost:4200/ 直接预览效果。

## Usage

```ts
import { NgModule } from '@angular/core';
import { FormsModule } from '@angular/forms';
import { BrowserModule } from '@angular/platform-browser';

import { AntModule } from 'fire-ant';

import { AppComponent }   from './app.component';

@NgModule({
    imports: [
        FormsModule,
        BrowserModule,
        AntModule
    ],
    declarations: [

    ],
    providers: [],
    bootstrap: [ AppComponent ]
})
export class AppModule { }
```

# Live Example
Open Chrome, and visits:
[https://fbchen.github.io/fire-ant](https://fbchen.github.io/fire-ant/index.html)

Demo Project:
[https://github.com/fbchen/fire-ant-example](https://github.com/fbchen/fire-ant-example)


