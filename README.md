# persian-material6-date-picker
Jalali date by displaying the correct calendar material 6 date picker

Retrieved from https://www.dotnettips.info/post/2890/%D8%B4%D9%85%D8%B3%DB%8C-%D8%B3%D8%A7%D8%B2%DB%8C-date-picker-%D8%AA%D9%88%DA%A9%D8%A7%D8%B1-angular-material-6x

requirements
npm install jalali-moment --save

Material 6+

Usage :



  <pre>
    <code>
       
       import { NgModule } from "@angular/core";
import {  DateAdapter,  MAT_DATE_FORMATS,  MAT_DATE_LOCALE } from "@angular/material";

import { MaterialPersianDateAdapter, PERSIAN_DATE_FORMATS } from "./material.persian-date.adapter";

@NgModule({
  providers: [
    { provide: DateAdapter, useClass: MaterialPersianDateAdapter, deps: [MAT_DATE_LOCALE] },
    { provide: MAT_DATE_FORMATS, useValue: PERSIAN_DATE_FORMATS }
  ]
})
export class MaterialModule {
}

  

       
    </code>
</pre>


Component :

<code>
  
  ```html
<mat-form-field>
    <input matInput [matDatepicker]="picker6" placeholder="json gregorian input" [(ngModel)]="dateControl">
    <mat-datepicker-toggle matSuffix [for]="picker6"></mat-datepicker-toggle>
    <mat-datepicker #picker6></mat-datepicker>
</mat-form-field>
```
 </code>
 

Continuation : https://www.dotnettips.info/post/2890/%D8%B4%D9%85%D8%B3%DB%8C-%D8%B3%D8%A7%D8%B2%DB%8C-date-picker-%D8%AA%D9%88%DA%A9%D8%A7%D8%B1-angular-material-6x
