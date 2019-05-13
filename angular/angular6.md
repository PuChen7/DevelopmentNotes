# Angular 6

## Content
* [Component](#component)

### Component
#### Resources:
  - [Official Docs](https://angular.io/guide/architecture-components)

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
