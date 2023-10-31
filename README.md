# Github Docs Example

## Step 1 - Using Codeblocks.

Codeblocks in markdown make it *very easy* for tech people to **copy, paste, share** code.
A good __Cloud Engineer__ uses Codeblocks whenever possible.

Because it allows others to copy and paste their code to replicate or research issue.
- In order to create a codeblocks in markdown, you need to use three backticks: __```__
- Do not be confused with quotation **'**
- When you can you should attempt to apply syntax highlighting

```Python
import os
from pyats import aetest
from pyats.datastructures.logic import And, Not, Or
from genie.harness.main import gRun


def main():
    test_path = os.path.dirname(os.path.abspath(__file__))
    gRun(
        trigger_datafile=test_path+'/get_switch_model.yaml',
        trigger_uids=['get_model'],
        subsection_datafile=test_path+'/subsection_datafile.yaml',
        testbed=test_path+'/apac_cisco_switch_tb.yaml',
    )
```

You should use codeblocks for both code and errors. 
```bash
NameError: name 'non_existent_variable' is not defined
```
> Here is an example of python error.

## Step 2 - How to take screenshot
Do not upload a part of your code as it is difficult to understand the full context.

## Step 3 - Use Git hub Flavored Markdown task lists

Github extends markdown to have a list where you can check off items. [<sup>[1]</sup>](#references)
- [x] Finish step 1
- [ ] Finish step 2
- [ ] Finish step 3

## Step 4 - Use Emojis (optional)

Github Flavoured Markdown (GFM) supports emoji shortcodes. [<sup>[3]</sup>](#references)
- Here are some examples:
  
| Name | Shortcode | Emoji |
| --- | --- | --- |
| Yummy | `:yum:` | 😋 |
| Cloud | `:cloud:` | ☁️ |
| Rainbow | `:rainbow:` | 🌈 |

## Step 5 - How to creat a table
Github extends the functionality of markdown table to provide more alignment and table cell formatting options. [<sup>[4]</sup>](#references)
```markdown
| Name | Shortcode | Emoji |
| --- | --- | --- |
| Yummy | `:yum:` | 😋 |
| Cloud | `:cloud:` | ☁️ |
| Rainbow | `:rainbow:` | 🌈 |
```

## Step 6 - Link to another file
Github supports to link to documents in other places.
[Ironman](/misc/ironman.md)

## References
- [Github Flavored Markdown Spec](https://github.github.com/gfm/) <sup>[1]</sup>
- [Basic writing and formatting syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) <sup>[2]</sup>
- [GFM - Emojis Cheatsheet](https://github.com/ikatyang/emoji-cheat-sheet) <sup>[3]</sup>
- [GFM - Table](https://github.github.com/gfm/#tables-extension-) <sup>[4]</sup>

