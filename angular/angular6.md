# Angular 6

## Content
* [Component](#component)

### Component
#### Resources:
[Official Docs](https://angular.io/guide/architecture-components)

- A component controls a patch of screen called a `view`
- You define a component's application logic—what it does to support the view—inside a class. The class interacts with the view through an API of properties and methods.

#### Component Metadata
- The metadata for a component tells Angular where to get the major building blocks that it needs to create and present the component and its view
-  It associates a `template` with the component, either directly with inline code, or by reference. The `component` and its `template` describe a `view`.
- The `@Component` decorator identifies the class immediately below it as a component class, and specifies its `metadata`.
- Example:
```javascript
    @Component({
      selector:    'app-hero-list',
      templateUrl: './hero-list.component.html',
      providers:  [ HeroService ]
    })
    export class HeroListComponent implements OnInit {
    /* . . . */
    }
```
#### Template and views
- You define a component's view with its companion template. A template is a form of HTML that tells Angular how to render the component.
- The template immediately associated with a component defines that component's `host view`. 
- Example: template.html
```html
<h2>Hero List</h2>

<p><i>Pick a hero from the list</i></p>
<ul>
  <li *ngFor="let hero of heroes" (click)="selectHero(hero)">
    {{hero.name}}
  </li>
</ul>

<app-hero-detail *ngIf="selectedHero" [hero]="selectedHero"></app-hero-detail>
```

#### Data binding
- a mechanism for coordinating the parts of a `template` with the parts of a `component`, tell Angular how to connect both sides
- The following diagram shows the four forms of data binding markup.
- ![Data Binding](https://angular.io/generated/images/guide/architecture/databinding.png)
- In two-way binding, a data property value flows to the input box from the component as with property binding. The user's changes also flow back to the component, resetting the property to the latest value, as with event binding.
- ![Bingding](https://angular.io/generated/images/guide/architecture/component-databinding.png)

#### Difference between `component` and `service`
- Component
  - a class with a decorator @Component which tells angular that the class is a component. 
  - They are always associated with an HTML template and some CSS.
  - When a part of html gets repeated with a similar functionality it is always best to put it into a component. This component can be called where ever the same functionality is required.
- Service
  - They are cenral units for some common functions across the application.
  - They are simple classes with functions and members.
