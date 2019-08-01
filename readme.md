
# File drop Component

It's an angular component for generic usage.

## Installation

Download the component and add it into your module.

## Usage

```TypeScript
import { FileDropComponent } from './file-drop/app-elastic.component';
import { DragNdropDirective } from './file-drop/drag-ndrop.directive';

@NgModule({
  declarations: [
    AppComponent,
    ....,
    FileDropComponent,
    DragNdropDirective
  ],
  imports: [
    BrowserModule,
    FormsModule,
    HttpClientModule,
    FileDropModule
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }

//** in your html file"
   <app-file-drop [multiple]="true" (filesDropEvent)="yourFileReciverFunction($event)">
   </app-file-drop>
```

## Parameters
Name  | Description | Example | 
------------- | ------------- | -------------
(filesDropEvent)  | on file drop event or add event | (filesDropEvent)="yourFIleReciverFunction($event)"|
multiple | enable multiple to allow selection of multiple files | [multiple]="true"

## Other requirements
None.


## Contributing
Pull requests are welcomed. For major changes, please open an issue first to discuss what you would like to change.
Please make sure to update tests as appropriate.


## License
