
         ANGULAR -Front End
--------------------------------------
    BASIC COMMANDS
    ---------------
    1. project creaton - ng new app-name
    2. project run - ng s -o
    3. component creation - ng g c component-name
    4. Service creation - ng g s service-folder/service-name
    5. router enable user module
    6. create pipe 

    BASIC CONCEPTS
    ---------------
    1. Module : root module - appModule, used to hold components
    2. Components : parts of UI, combination of ts file,html file,css file, Root copmonent
    -AppComponent
    3. set up path for component - use routing-module.ts file
        - use Routes array, specif path of each component as an object in the array
        - use router-outlet selector in root component - used to switch component template according to the user requested path
    4. Data Binding : Data sharing within a component
        - One Way binding 
            - String Interpolation : use {{class-property}}
            - Property binding : use  [class-property] = "expression"
            - event binding : (event-name) = "function-call"
            - event binding using $event : (event-name) = "function-call($event)"
            - event binding using template referance variable : #variable-name
        - Two way binding : using ngModel Directive
            - import FormsModule file, then use [(ngModel)]="class-property"
    5. Angular Directive : are class that add additional behaviour to html elements
        - prebuilt Directive
            - Component Directive : component selector used to display component template
            - ngModel Driective : used to manage form controls
            - Structural Directive : used to add / remove elements from angular app
                - *ngIf="condition"
                - *ngFor="let array-items of array-name"
            - Attribute Directive : used to provide class of style
                - ngClass : used to provide class to html element
    6. Dependency Injection : when two class are dependent then one class can access others property and function, it should  provide in constructor
        - syntax : access-specifier variable-name : dependent-class-name
    7. Angular Services : To share common logic with all component
        - Template driven Forms
        - Model driven Forms
    8. Handiling Asynchronus function : RxJS Library
        - Observable :
            - subscribe(callback/observer object) : resolve state 
        - API Call : use http method in httpClient class
            - Import  HttpClientModule to your Module file
    9. 
    