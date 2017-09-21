# Introduction
Smitapurva Fiori (SP Fiori) is a bootstrap based theme which looks like SAP Fiori. Main objective of this repository are css files inside CSS folder.

## Installation
- Clone this git repository.
- Install these node modules:
* Bootstrap 3.3 `npm i bootstrap@3 --save`.
* Startbootstrap Simple Sidebar `npm i startbootstrap-simple-sidebar --save`.

# UI Components
## Box
Box is used in Fiori Dashboard. It could be used inside `row` and `col-[size]-[col]` within Bootstrap's grid system. Example:
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
* Header, contains: navigation button (shell_nav) and title (shell_title).
* Body, contains: any `<html>` components. It usually contain table, or forms.
* Footer, contains: action buttons such as "Approve", "Reject", or iconic button.
![shell](https://user-images.githubusercontent.com/31851739/30687066-61a67bba-9ee4-11e7-9374-a9c167a9db80.png "Shell Component")
Example of usage:
```html
<div class="shell-container">
    <div class="shell__header">
        <a class="shell__nav">
            <span class="glyphicon glyphicon-chevron-left"></span>
        </a>
        <h1 class="shell__title">Inputs</h1>
    </div>
    <div class="shell__body">
        Content Here
    </div>
    <div class="shell__footer text-right">
        <button class="btn btn-default"><span class="glyphicon glyphicon-cog"></span></button>
        <button class="btn btn-success">Approve</button>
        <button class="btn btn-danger">Reject</button>
    </div>
</div>
```
Options:
* Add class `no-padding` after `shell__body` to remove padding.