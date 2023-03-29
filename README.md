# Typescript

- We can declare variables in typescript as follows

```
let name: string
or
let name: string = "amit"
```

- if we are going to initialize the variable with some value then typescript can infer the type based on that value.

```

let name = "amit" //so here the type of name is infered as string

```

## The "Any" type

##### Remember: Be very careful when using this type

- The "Any" type bypasses typechecking
- This means that any variable declared using any type will not undergo typechecking.

```

let email: any;

```

- In fact in the type.config file we can turn on the **noImplicitAny** flag so that whenever a variable is declared as any, it will give error
- This flag can be helpful because sometimes typescript is not able to infer the type for us and thus uses "Any" type. 
