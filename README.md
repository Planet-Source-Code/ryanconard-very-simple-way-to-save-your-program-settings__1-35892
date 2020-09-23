<div align="center">

## Very simple way to save your program settings\!


</div>

### Description

This is very, very simple.. This is the easiest way to save a save a setting, besides using Print to text file.. it can be useful to save from and load to text boxes, dropdowns, listboxes, what have you.. because of its simplicity i dont expect votes.. its just a small piece of code.. but vote if you want to... thanks, enjoy!
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[RyanConard](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/ryanconard.md)
**Level**          |Beginner
**User Rating**    |3.7 (22 globes from 6 users)
**Compatibility**  |VB 5\.0, VB 6\.0
**Category**       |[Coding Standards](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/coding-standards__1-43.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/ryanconard-very-simple-way-to-save-your-program-settings__1-35892/archive/master.zip)





### Source Code

```
'This code is very, very simple..
'I dont care if you vote on it or not..
'just enjoy it..
Private Sub cmdGet_Click()
'This calls upon everything in cmdSave
'Then puts the text in txtSave
txtSave.Text = GetSetting(App.ProductName, "Settings", "txtSave", txtSave.Text)
End Sub
Private Sub cmdSave_Click()
'This saves the following:
'1. Product Name [Located under Project > ..Properties > Make]
'2. It writes a category called "Settings"
'3. It writes a sub category called "txtSave"
'4. Under sub category "txtSave" it writes whatever text is in txtSave
SaveSetting App.ProductName, "Settings", "txtSave", txtSave.Text
End Sub
Private Sub txtSave_Change()
'No code goes here
'Just make a txtSave
End Sub
```

