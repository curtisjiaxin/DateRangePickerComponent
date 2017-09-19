# DateRangePickerComponent

Quote bootstarp and rewrite so that change the data that we want.

### grammar:
+ [Angular](https://angular.io),
+ [Type Script](http://www.typescriptlang.org/),
+ [SCSS](http://sass-lang.com/)
+ [Bootstrap](http://getbootstrap.com/2.3.2/)

## Component

Create ``data-range-picker.component``

Import the essential dependence.
```
import { Component, ElementRef, OnInit, Input, Output, EventEmitter } from '@angular/core';
import { DateRangePicker } from 'daterangepicker';
import { KscDateRangePickerModel } from './ksc-date-range-picker.model';
import * as _ from 'lodash';
import * as moment from 'moment';

@Component({
  selector: 'ksc-data-range-picker',
  template: `<div class="ksc-date-range-picker-container">
                <span class="input-group-btn">
                <button class="btn default date-range-toggle" type="button" (selected)='selectDtRange($event)'>
                    <i class="fa fa-calendar"></i>
                </button>
                  </span>
              </div>`,
  styleUrls: ['./ksc-date-range-picker.component.scss']
})
```
Write the HTML in ``template`` , and create scss file and write the route in`` styleUrls:[`  `]``
