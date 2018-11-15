# IntelliJ IDEA Shortcuts

## Editing and Working With Code

#### Moving Line and Statement
**Ctrl** + **Shift** + **Up**       to move line/statement up

**Ctrl** + **Shift** + **Down**     to move line/statement down

#### Duplicating and Deleting line
**Ctrl** + **D**        to duplicate current line

**Ctrl** + **Y**        to delete current line

#### View Parameter Information
**Ctrl** + **P**        to view suggested parameters for a method/constructor

#### Commenting and Block Commenting Code
**Ctrl** + **/**                to comment or uncomment current selection

**Ctrl** + **Shift** + **/**        to block comment or uncomment current selection

#### Folding and Expanding Code
**Ctrl** + **+**        to expand current code block

**Ctrl** + **-**        to fold current code block

## Code Navigation

#### Navigating to Class by Partial Match, Camel Humps and Wildcard Search
**Ctrl** + **N**                    to navigate to class

- partial match
- camel humps (TPE -> **T**hread**P**ool**E**xecutor)
- wildcard search (Thread*execut -> ThreadPoolExecutor)

**Ctrl** + **Alt** + **Left**       to navigate back

#### Navigating to Symbols
**Ctrl** + **Alt** + **Shift** + **N** to navigate to symbol

- filter method by class name (TPE.getTask -> **T**hread**P**ool**E**xecutor.getTask())

#### Navigating to File
**Ctrl** + **Shift** + **N**        to navigate to file

- type folder with slash to look up folder

#### Navigating to Action
**Ctrl** + **Shift** + **A**        to navigate to desired action

- type java compiler to see the option in settings

#### Search Everywhere
**Double Shift**        to search everywhere (classes, files, symbols, actions)

- **tab** to move between sections in search everywhere window

#### Tabs, the No. 1 Productivity Killer
Switch tabs off by:
- pressing **Ctrl** + **Shift** + **A**
- type tab place and choose **Tab placement: None**

**Ctrl** + **E**                    to navigate to recent files
**Ctrl** + **Shift** + **E**        to navigate to recent edited files

## Code Selection

#### Selecting Characters, Words and Lines
**Ctrl** + **Shift** + **Right** or **Left**

Action: Move Caret to Next/Previous Word with Selection

**Shift** + **Home** or **End**

Action: Move Caret to Text Start/End with Selection

#### Extending and Shrinking Selection
**Ctrl** + **W**                    to extend selection
**Ctrl** + **Shift** + **W**        to shrink selection

## Code Completion
#### Smart Code Completion I
**Ctrl** + **Shift** + **Space**        to invoke smart code completion

- after the new keyword in an object declaration
- in the list of parameters of a method call
- in return statements

#### Smart Code Completion II
**Ctrl** + **Shift** + **Space Twice**      to invokde smart code completion for:

- static expressions
- collections, lists and arrays

#### Static Method Completion
**Ctrl** + **Space Twice**       to display static method suggestion list

#### Postfix Completion
**Ctrl** + **J**    to display postfix completion suggestion list

- nn/null (check expression to be null)
- notnull (checks expression to be not-null)
- synchronized (produces synchronization statement)

**Null example**
```
String s = "Hello";
        s.null
```
after pressing enter, intelliJ will produce
```
String s = "Hello";
if (s == null) {

        }
```

**Synchronized example**
```
String s = "Hello";
        s.synchronized
```
after pressing enter, intelliJ will produce
```
String s = "Hello";
synchronized (s) {

}
```

## Code Generation
#### Generating Constructor, getter, setter, equals and hashCode Methods
**Alt** + **Insert**        to display generate menu in class file

## Version Control
#### VCS Operations Popup, Searching for Branches, Annotation
Default keymap

**Alt** + **Back Quote**        to bring up VCS operations popup

My shortcut for fedora

**Alt** + **V**                 to bring up VCS operations popup

## Language injection
Lets say we want to create a json string:

```
String json = "";
```

Press **Alt** + **Enter** to display the intention actions and select

<i>Inject language or reference</i>

select **JSON** and press enter.

**JSON** has been injected into the string.

Press **Alt** + **Enter** again and select

<i>Edit JSON fragment</i>

IntelliJ opens new fragment editor for you.

When you insert JSON code into the fragment editor, the code gets
automatically injected into the original string.

When you are done, press **Ctrl** + **F4** to end the current fragment editor.

Output of the language injection into the original string:
```
//language=JSON
String json = "{\"jsonObject\": {\n" +
                       "  \"fieldA\": 5,\n" +
                       "  \"fieldB\": \"String\"\n" +
           "}}";
```