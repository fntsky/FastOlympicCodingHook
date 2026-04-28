# FastOlympicCodingHook
Problem test-case parser for sublime text from various online judges. Depends on [Competitive Companion](https://github.com/jmerle/competitive-companion) and [FastOlympicCoding](https://github.com/Jatana/FastOlympicCoding).

<u><b>Fork 版功能变化</b></u>

- 增加样例保存成功提示。
- 增加获取样例成功/失败提示。
- 增加开始监听选中文件的成功提示。

<u><b>Setup</b></u>

- Make sure you have `python3`, [FastOlympicCoding](https://github.com/Jatana/FastOlympicCoding) and [Competitive Companion](https://github.com/jmerle/competitive-companion) installed.
- Add `12345` in the list of ports of competitive-companion browser extension.
- Clone the [repository](https://github.com/DrSchwad/FastOlympicCodingHook) inside your Sublime Text Packages folder and rename the cloned folder to `FastOlympicCodingHook`. You can do a quick google search to find your packages folder. For example, on MacOS it is `~/Library/Application Support/Sublime Text/Packages/`.
- Configure the relative directory and file suffix for test cases files in the FastOlympicCoding settings (`FastOlympicCoding.sublime-settings`). <b>After making changes to this file, remember to restart Sublime Text.</b>

<u><b>Usage</b></u>

1. Navigate to the file that you'll solve the problem in. Then right click anywhere in the file. You should find an option named `Listen to Competitive Companion`. Click on it.
2. In the browser, navigate to the problem page and click on the competitive-companion extension's `green plus icon`.

The problem's test cases and correct answers will now be parsed and stored in `tests_relative_dir` within the parent directory of your code file, using the filename `tests_file_suffix` appended to your code file's name. For example if you are solving `abc.py`, the test case file will be `abc.tests`. If you don't have any `tests_relative_dir` defined, the tests will be stored in the same directory as your code file.

To see a walkthrough of the setup process, you can watch this video:

[![Setup walkthrough](https://img.youtube.com/vi/68dm0bLwcsY/hqdefault.jpg)](https://youtu.be/68dm0bLwcsY)
