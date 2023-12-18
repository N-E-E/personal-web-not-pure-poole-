---
layout: post
title: 2023 HUAWEI Developer Course Summary ———— Modern C++ and design pattern
date: 2023-12-09
last_modified_at: 2020-10-01 01:08:25 +0800
tags: [Engineer, Modern C++, design pattern]
toc:  true
---

# Lesson 1: CMake templates(With gtest), git commit rules

### CMake templates with gtest
It's a good template to use in cmake projects!

[template](https://github.com/N-E-E/1_developer_test)

### git commit rules
- If enabled, commit files according to the update contents. Remember: **Never use `git add .` in root folder**
- seperate the commit of source code and test code.
- commit after every update unit. Don't update everything until the end.
- commit messages should be as detailed as possible

# Lesson 2: design pattern in OOP
### basics
Encapsulation, Inheritance and Polymorphism

### table-driven and strategy pattern
In the problem, every price calculation method is a strategy, we can put them in a map.

### how to decouple the inheritance relation
Single Responsibility Principle: Each class should be responsible for only one functionality.

When dealing with multiple strategies, functional programming can be used to simplify classes. Utilize the `std::function` library to pass strategy functions.

# Lesson 3: More STL && modern C++ knowledge
## STL

### Iterator Validity

Beware of iterator invalidation.

### std::begin

```cpp
std::sort(std::begin(x), std::end(x));  // recommended
```
### std::string Utilizes Small String Optimization
It reallocates to the heap after exceeding 15 characters.

### Fixed-Width Types
Examples include int8_t, uint8_t.

printf cannot be used; instead, use cout.

### std::byte
8 bits, represents binary bit content, and can only perform bitwise operations.

Static_cast to byte may result in truncation.

## Modern C++
### auto
auto x = {1, 2, 3} will deduce an initializer_list.

auto cannot deduce traditional arrays. It is recommended to use array.

Auto deducing function return values requires the function definition to be visible in the current file, implying that the function definition should be in the header file (inline or template).

### {} Uniform Initialization
1. {} does not allow implicit narrowing conversions. E.g., int = {double + double} --> error.

### initializer_list
```cpp
auto x = {1, 2, 3, 4}   // Automatically converts to initializer_list. Assumes all elements have consistent types.
```

### constexpr
Evaluated at compile-time and implies const.
```cpp
const int a = 1;  // Can ensure value is determined at compile time.
const int a = val;  // Cannot ensure.

constexpr int x = 1;
int* p = &x;  // error
const int* cp = &x;  // OK
```
- Define as constexpr whenever possible.
- constexpr cannot include dynamic allocation behavior or containers; it can only include constexpr functions.

### static_assert

### std::array
- Replaces native arrays, same type, fixed size.
- Function returning arrays are often written as templates.
- Elements are initialized as if the type has no default constructor.

### Lvalues, Rvalues, Move Semantics
Move semantics and destructors are generally defined as noexcept.



