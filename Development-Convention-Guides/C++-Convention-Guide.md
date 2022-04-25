[[_TOC_]]

## General
- Use `#pragma once`, other than `#ifndef` include guards.

## C++ Standard
- Use `std::numbers::pi` instead of `M_PI`.
- Use `std::chrono::steady_clock` or `std::chrono::system_clock` instead of `std::chrono::high_resolution_clock`.

## Conditional Statements
- Use ternary operators when code can be concise without compromising readability.

  >```c++
  >const char* meridiem = hour < 12 ? "PM" : "AM";
  >```

- Do not use nested tenaries.

  >**Bad**👎
  >```c++
  >bool operator<(const Point3D& rhs) const { return x < rhs.x ? true : (x == rhs.x ? (y < rhs.y ? true : (y == rhs.y ? z < rhs.z : false)) : false); }
  >```

  >**Good**👍
  >```c++
  >bool operator<(const Point3D& rhs) const {
  >    if (x < rhs.x) { return true; }
  >    if (x > rhs.x) { return false; }
  >    if (y < rhs.y) { return true; }
  >    if (y > rhs.y) { return false; }
  >    if (z < rhs.z) { return true; }
  >    return false;
  >}
  >```

- Do not omit braces.

  >**Bad**👎
  >```c++
  >for (int i = 1; i <= num; i++)
  >    if (i % 2)
  >        sum_odd += i;
  >    else
  >        sum_even += i;
  >```

  >**Good**👏
  >```c++
  >for (int i = 1; i <= num; i++) {
  >    if (i % 2) {
  >        sum_odd += i;
  >    } else {
  >        sum_even += i;
  >    }
  >}
  >```