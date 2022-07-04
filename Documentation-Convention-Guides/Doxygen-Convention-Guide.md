[[_TOC_]]

## Comment Format
- There are several different ways to document codes in doxygen format, but Javadoc style, which consists of a C-style comment is recommended to use.

  >```
  >/**
	> * @brief <write here>
	> * @param <write here>
	> * @...
	> * @...
	> * @return <write here>
	>*/
	>void func();
  >```

## Description

- First letter of each statement must be `capitalized`.

  >**Bad**👍
  >```diff
	> * @brief adds up the given numbers.
	>int sum(const std::vector<int>& numbers);
  >```

  >**Good**👍
  >```diff
	> * @brief Adds up the given numbers.
	>int sum(const std::vector<int>& numbers);
  >```

- Statements must be ended with `.`

  >**Bad**👍
  >```diff
	> * @brief Adds up the given numbers
	>int sum(const std::vector<int>& numbers);
  >```

  >**Good**👍
  >```diff
	> * @brief Adds up the given numbers.
	>int sum(const std::vector<int>& numbers);
  >```
