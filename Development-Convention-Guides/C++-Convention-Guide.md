[[_TOC_]]

## Conditional Statements
- Use ternary operators when code can be concise without compromising readability.

  >```c++
  >const char* meridiem = hour < 12 ? "PM" : "AM";
  >```

- Do not use nested tenaries.

  >**BAD**👎
  >
  ><strike>
  >
  >```c++
  >bool operator<(const Point3D& rhs) const { return x < rhs.x ? true : (x == rhs.x ? (y < rhs.y ? true : (y == rhs.y ? z < rhs.z : false)) : false); }
  >```
  >
  ></strike>
  >
  >**BETTER**👍
  >
  >```c++
  >bool operator<(const Point3D& rhs) const {
  >    if (x < rhs.x) return true;
  >    if (x > rhs.x) return false;
  >    if (y < rhs.y) return true;
  >    if (y > rhs.y) return false;
  >    if (z < rhs.z) return true;
  >    return false;
  >}
  >```

- Do not omit braces unless in case of a one-line statement.

  >**BAD**👎
  >
  ><strike>
  >
  >```c++
  >for (int i = 1; i <= num; i++)
  >    if (i % 2)
  >        sum_odd += value;
  >    else
  >        sum_even += value;
  >```
  >
  ></strike>
  >
  >**BETTER**👍
  >
  >```c++
  >for (int i = 1; i <= num; i++) {
  >    if (i % 2) sum_odd += value;
  >    else sum_even += value;
  >}
  >```
  >
  >**BEST**👏
  >
  >```c++
  >for (int i = 1; i <= num; i++) {
  >    if (i % 2) {
  >        sum_odd += value;
  >    } else {
  >        sum_even += value;
  >    }
  >}
  >```