ngIf
=======
-[hidden]='false' : simply hides the element

-*ngIf='false' : removes the element completely from the DOM

-using the Logical NOT (!)


ngIf Syntax -->
============
<p *ngIf="condition">

    content to render, when the condition is true 
    
</p>
=====================================================
<p *ngIf="!condition">

    content to render, when the condition is false
    
</p>


ngIf else syntax-->
====================
<div *ngIf="condition; else elseBlock">

    content to render, when the condition is true 
    
</div>
 
<ng-template #elseBlock>

    content to render, when the condition is false 
    
</ng-template>
=====================================================

ngIf then else Syntax
=======================
<div *ngIf="condition; then thenBlock else elseBlock"> 

    This content is not shown
    
</div>
 
<ng-template #thenBlock>

    content to render when the condition is true.
    
</ng-template>
 
<ng-template #elseBlock>

    content to render when condition is false.
    
</ng-template>

===========================================================
 
 
In app.module.ts
======================
import { FormsModule } from '@angular/forms';


@NgModule({


imports: [


     FormsModule    
     
]



# NgifTest

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 9.0.4.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
