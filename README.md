# What is todo.sslet?
This is a spreadsheet version of todo.txt that can be managed in a spreadsheet.
Columns can be added (links, work hours, etc.) and extended according to the user's preferences.

## Differences from todo.txt
1. spreadsheet functions for sorting, filtering, and autofilling
1. a link column is provided to allow access to external resources. We envision links to issue trackers, calendar applications, reference sites, etc.
1. context is set as a tag
1. branch numbers are allowed in the priority order. Also, it is assumed that parentheses are not necessary. Example: `C-1`.
1. Allow additional columns.

## Installation
Copy the code below to the clipboard and paste it into cell A1 of your Excel or Google spreadsheet.  
Line breaks at the end of the line are required.

```tsv:todo_en.sslet
Done	Priority	Completion date	Creation date	Tags	Projects	Links

```

## Usage
Enter one task per line.
Each line contains the following items

### Completed
Indicates that the task has been completed. Uncompleted tasks are blank, and completed tasks are indicated by an "x".

### Priority
Indicates the priority of the task. It is represented by a single alphabetic character and can be duplicated in other lines.
A branch number of any depth can be attached. The branch number is represented by "-{number}".

### Creation date (optional)
Describes the date the task was created. May be left blank.

### Completion date (optional)
Describe the date when the Task was completed. May be left blank.

### Tasks (optional)
Briefly describe the Task.

### Projects (optional)
Describe which project the Task is for. May be left blank.
Project is described as "+{project name}". Multiple entries are allowed.

### Tags (optional)
Enter keywords for search and filtering, separated by spaces. May be left blank.
Tags are described as "#{tag name}". Multiple tags can be entered.

### Notes (optional)
This is a free text field. You may leave it blank. The `keyword:content` format is recommended, but not mandatory.

### Link (optional)
Link to an external web page or any cell. May be left blank.

### Example of Task Entry
Completed | Priority | Creation date | Completion date | Tasks | Projects | Tags | Notes | Link
---|---|---|---|---|---|---|---|---
| x | C | 2022/04/20 | 2022/05/08 | send a carnation |  | #phone #family | due:2022/05/08
|  | A | 2022/06/12 |  | Make a schedule for the week. | +ProjectA +ProjectX | 
|  | C-1 |  |  | Make a sign | +garagesale |  |  | https://www.example.com//en-us/materials/
|  |  |  |  |  |  | #shopping | cat food

## Convenient Usage
### Use the filter function
You can use the spreadsheet function to filter and refine by project, tag, priority, creation date, or completion date to see the tasks that need to be done today or the progress of tasks in a certain project.  
Of course, sorting also allows you to sort tasks by date or by priority.

### Using the Table function
The spreadsheet's table function allows you to add a new row to the task list when you press enter on the last row.  
You can also use filters and sorting.

### Using the Search Function
You can also use the spreadsheet's text search function to search across tasks, project names, and tag names.

### Example of adding columns
Completed | Priority | Creation date | Completion date | Tasks | Projects | Tags | Notes | Link | starting time | End time | the time required
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | ---
|  |  |  |  |  |  |  |  |  |  |  | =K2-J2

In this example we have added columns for start time, end time, and required time. The cell under Duration Time contains a formula, which is copied and used with auto-fill after the second case.

Translated with www.DeepL.com/Translator (free version)
