[[_TOC_]]

## Naming
- Use `snake_case` for source code filenames (C++ headers/sources, python scripts, shell scripts, ...) : a combination of small letters `[a-z]` and underscores `_` with one full stop `.` as a seperator for the file extension.

  >**Bad**👎
  >```diff
  >CSVReader.h
  >csvReader.hpp
  >csv+reader.cpp
  >csv-reader.py
  >csv reader.sh
  >```

  >**Good**👍
  >```diff
  >csv_reader.h
  >csv_reader.hpp
  >csv_reader.cpp
  >csv_reader.py
  >csv_reader.sh
  >```

- Use `.yaml` as an extension for YAML files.