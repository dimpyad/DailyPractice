### Problem #1
- Topic: String
- Difficulty Level: Easy
- [Link to the problem](https://leetcode.com/problems/excel-sheet-column-title/)
- [Similar problem](https://leetcode.com/problems/excel-sheet-column-number/)			

### Problem #2
- Identify the problem statement from the below code
- Add comments to make the code more readable
- Add test scenarios.
```
public boolean isValidInput(String input)
	{
		String zeroTo255
			= "(\\d{1,2}|(0|1)\\"
			+ "d{2}|2[0-4]\\d|25[0-5])";

		String regex
			= zeroTo255 + "\\."
			+ zeroTo255 + "\\."
			+ zeroTo255 + "\\."
			+ zeroTo255;

		Pattern p = Pattern.compile(regex);
		if (input == null) {
			return false;
		}
		Matcher m = p.matcher(input);
		return m.matches();
	}
```
