# Stack

Author: Jishith M P

A simple LIFO (Last In, First Out) Stack collection for Zen with type-specific operations for:

- `int`
- `bool`
- `double`
- `long`
- `byte`
- `string`

## Installation

    zen install stack

## Usage

    import (Stack) from "stack"

    Stack s

    s.pushInt(10)
    s.pushInt(20)
    s.pushInt(30)

    screen(s.peekInt())     // 30
    screen(s.popInt())      // 30
    screen(s.popInt())      // 20

## API

### Integer

    s.pushInt(value)
    s.popInt()
    s.peekInt()
    s.sizeInt()
    s.isEmptyInt()

### Boolean

    s.pushBool(value)
    s.popBool()
    s.peekBool()
    s.sizeBool()
    s.isEmptyBool()

### Double

    s.pushDouble(value)
    s.popDouble()
    s.peekDouble()
    s.sizeDouble()
    s.isEmptyDouble()

### Long

    s.pushLong(value)
    s.popLong()
    s.peekLong()
    s.sizeLong()
    s.isEmptyLong()

### Byte

    s.pushByte(value)
    s.popByte()
    s.peekByte()
    s.sizeByte()
    s.isEmptyByte()

### String

    s.pushString(value)
    s.popString()
    s.peekString()
    s.sizeString()
    s.isEmptyString()

## Behavior

Stack follows LIFO ordering:

    s.pushInt(10)
    s.pushInt(20)
    s.pushInt(30)

    s.popInt() // 30
    s.popInt() // 20
    s.popInt() // 10

`push*()` adds a value to the top of the stack.

`pop*()` returns and removes the value from the top.

`peek*()` returns the top value without removing it.

`size*()` returns the number of values currently stored for that type.

`isEmpty*()` returns `true` when the corresponding stack is empty.

## Supported Types

| Type | Push | Pop | Peek | Size | Is Empty |
|------|------|-----|------|------|----------|
| `int` | `pushInt()` | `popInt()` | `peekInt()` | `sizeInt()` | `isEmptyInt()` |
| `bool` | `pushBool()` | `popBool()` | `peekBool()` | `sizeBool()` | `isEmptyBool()` |
| `double` | `pushDouble()` | `popDouble()` | `peekDouble()` | `sizeDouble()` | `isEmptyDouble()` |
| `long` | `pushLong()` | `popLong()` | `peekLong()` | `sizeLong()` | `isEmptyLong()` |
| `byte` | `pushByte()` | `popByte()` | `peekByte()` | `sizeByte()` | `isEmptyByte()` |
| `string` | `pushString()` | `popString()` | `peekString()` | `sizeString()` | `isEmptyString()` |

## License

MIT
