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