OF Daily Standup Generator v0.5

This is forked from my Flexible Daily Report generator, [which you can find here.](https://github.com/ccmills/OF-FlexibleReporting). You can install and configure in the same way.

It adds functionality of pulling your tasks from a "Today" perspective if you have it, and adds user prompt section for "Hangups" to add notes. It's most useful for teams running daily standups of the Agile variety. 

## Known issues
* Perspective titles are not easily configurable, so if you don't have a "Today" and "TodayProj" perspective (where the latter is grouped by project) it will currently break. I'll expand functionality....eventually
* The tasks grabbed from the perspective currently ignore the __ignoreList__ settings, so if you have personal and work actions comingling, they'll show up under your Today heading together, even if one or the other belongs to a folder in __ignoreList__. This can be sovled by having your perspectives inherit focus and focusing on work or personal projects beforehand, but the script doesn't currently do anything about that.
* Today tasks are sorted by project. In the future, the could be sorted by due date, flag status, context or other grouping exposed via OF dictionary.