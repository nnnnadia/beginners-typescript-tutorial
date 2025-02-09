# Parameter X implicitly has an 'any' type

```typescript
const addTwoNumbers = (a, b) => {
   return a + b
}
```

> Parameter 'a' implicitly has an 'any' type.
>
> Parameter 'b' implicitly has an 'any' type.

## What is going on?

Missing type annotation to a parameter in a function.

It is turned on by strict mode.

```json
// tsconfig.json
{
  "compilerOptions": {
    "strict": true
  }
}
```

## Why is this important?

This is the essence of Typescript, without it the code is loosely typed and errors are prone to happen.
