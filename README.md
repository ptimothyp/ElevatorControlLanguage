# Elevator Control Language
Simple parser using [Superpower](https://github.com/datalust/superpower), the parser combinator library by [Nicholas Blumhardt](https://twitter.com/nblumhardt)

Hey! Would you like to create a parser? Then take a look to learn how to create a one for a simple language! :)

I have invented a very basic grammar just to learn. I have thought of an elevator that follows a list of instructions to go up, down and wait.

**Example**:

```
(UP 100),
(DOWN 200),
(DOWN 100),
(DOWN @1),
(UP @3),
(WAIT),
(UP 300)
```

As you see, it consists of a list of comma-separated verbs to move, for example, an elevator.

- The verbs are **UP**, **DOWN** or **WAIT**.
- Every verb is enclosed by parentheses: **( )**
- **UP** and **DOWN** require either an absolute number or a relative number, that indicates the floor to which the elevator should move. 
- Relative floor numbers come with a **@** before the number.
- **WAIT** doesn't accept any number, because it stops the elevator for a while.

### This project was inspired by [this thread](https://stackoverflow.com/questions/47740985/parsing-a-simple-text-grammar-with-superpower/47743790#47743790) in StackOverflow.
