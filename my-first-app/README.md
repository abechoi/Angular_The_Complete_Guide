<h1 align=center>
  My First App
</h1>
<p align=center>
Angular - The Complete Guide 2021 Edition
</p>
<p align=center>
Created by Maximillian Schwarzmuller
</p>

## Setup

```
npm i -g @angular/cli@latest

// make sure npm, angular, and node are up-to-date
ng version

// create project
ng new my-first-app --no-strict
```

## Input

app.component.html

```
<input type="text" [(ngModel)]="name">
<p>{{ name }}</p>
```

app.component.ts

```
export class AppComponent {
  name = 'Abe';
}
```

app.module.ts

```
// add FormsModule to use ngModel
import {FormsModule} from '@angular/forms';

@NgModule({
  imports: [
    FormsModule
  ]
})
```
