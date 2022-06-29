[[_TOC_]]

## Comment Format
- There are several different ways to document codes in doxygen format, but it is recommended to follow the comment style shown below.

  >```
  >/**
	> * @brief <write here>
	> * @param <write here>
	> * @return <write here>
	>*/
  >```

Examples,

  >**Bad**👎
  > ```
	>/****************************************************
	> * @brief Scans connected sensors.
	> * @param token Stop token.
	> * @param option Options for sensor scanning.
	> * @param listener Invoked when the sensor is found.
	> ****************************************************/
	>static void scan(std::stop_token token, const ScanOption& option, const std::function<void(std::shared_ptr<Sensor>)>& listener);
  > ```

  >**Good**👍
  > ```
	>/**
	> * @brief Scans connected sensors.
	> * @param token Stop token.
	> * @param option Options for sensor scanning.
	> * @param listener Invoked when the sensor is found.
	> */
	>static void scan(std::stop_token token, const ScanOption& option, const std::function<void(std::shared_ptr<Sensor>)>& listener);
  > ```
