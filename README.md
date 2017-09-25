# Introduction
Smitapurva Fiori (SP Fiori) is a bootstrap based theme which looks like SAP Fiori. Main objective of this repository are css files inside CSS folder.

## Installation
- Clone this git repository.
- Install these node modules:
* Bootstrap 3.3 `npm i bootstrap@3 --save`.
* Gulp 3.9.1 `npm i gulp --save`.
* Gulp Concat `npm i gulp-concat --save`.

## Running the apps locally
Try using `npm start` or `gulp start` to start apps in `localhost: 8283` (default).

# UI Components

## Box
Box is used in Fiori Dashboard. It could be used inside `row` and `col-[size]-[col]` within Bootstrap's grid system.
![box](https://user-images.githubusercontent.com/31851739/30687565-d5e8cd42-9ee5-11e7-84c0-ef5d80794215.png)

Example of usage:
```html
<div class="col-md-2 col-sm-4 col-xs-6">
    <div class="box">
        <h3 class="box__header">My Time Events</h3>
        <h4 class="box__subheader">Manage my time events</h4>
        <h2 class="box__icon"><span class="glyphicon glyphicon-glass"></span></h2>
        <h2 class="box__number">12</h2>
        <h4 class="box__footer">Pending Events</h4>
    </div>
</div>
```

## Shell
Shell is a common container or page that is used in Fiori app. Each shell consists of following part.
* Sidebar Header, contains: header title (text).
* Sidebar Body, contains: free space to add any HTML tag. It usually contains sidebar menu navigation (separate topic).
* Sidebar Footer, contains: free space to any action buttons (if needed).
* Header, contains: navigation button (shell_nav) and title (shell_title).
* Body, contains: any HTML components. It usually contain table, or forms.
* Footer, contains: action buttons such as "Approve", "Reject", or icon button.

![shell](https://user-images.githubusercontent.com/31851739/30733116-c62e4214-9f9f-11e7-93ae-f43472b022a6.png)


Example of usage:
```html
<div class="shell-container">
    <aside class="shell__sidebar">
        <div class="shell__sidebar-header">
            Header here...
        </div>
        <div class="shell__sidebar-body">
            Sidebar menu here...
        </div>
        <div class="shell__sidebar-footer">
            Footer here...
        </div>
    </aside>
    <section class="shell__main">
        <div class="shell__header">
            <a class="shell__nav" href="#menu-toggle" id="menu-toggle">
                <span class="glyphicon glyphicon-chevron-left"></span>
            </a>
            <h1 class="shell__title">Main header here...</h1>
        </div>
        <div class="shell__body">
            Main content here...
        </div>
        <div class="shell__footer text-right">
            <button class="btn btn-default"><span class="glyphicon glyphicon-cog"></span></button>
            <button class="btn btn-success">Approve</button>
            <button class="btn btn-danger">Reject</button>
        </div>
    </section>
</div>
```

Options:
* Add class `no-padding` after `shell__body` to remove padding.

## Paper
Paper is a background. It is commonly used inside `shell__body` component.

![paper](https://user-images.githubusercontent.com/31851739/30688344-13ff2ea8-9ee8-11e7-9883-55093acc0f88.png)

Example of usage:
```html
<div class="paper paper--shadow">
    <h4>Put your title here</h4>
    <p>This is basic paper usage.</p>
</div>
```

Options:
* Add class `paper--shadow` after `paper` to add shadow.