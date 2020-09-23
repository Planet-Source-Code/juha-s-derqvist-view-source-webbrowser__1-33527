<div align="center">

## View Source \- Webbrowser


</div>

### Description

View source - using webbrowser control.

No need of those msinet.ocx which all people always tell to use to get source of HTML-page.

This is a simple and beatiful way to do it.

PS..another even smart way is to add a webbrowser2.visible = false and to change viewsource function to use the hidden one.. instead of the webbrowser1 (which you may use to navigate pages) ; )
 
### More Info
 
Source of webpage, opens notepad and if html-source is too big automaticly opens wordpad !!


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Juha sÃƒÂ¯Ã‚Â¿Ã‚Â½derqvist](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/juha-s-derqvist.md)
**Level**          |Intermediate
**User Rating**    |4.3 (26 globes from 6 users)
**Compatibility**  |VB 6\.0
**Category**       |[Internet/ HTML](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/internet-html__1-34.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/juha-s-derqvist-view-source-webbrowser__1-33527/archive/master.zip)





### Source Code

```
' a sub to be called from example webbrowser
' mnuviewsource
' webbrowser1 = webbrowser control
' combo1 = used as an addressbar
private sub viewsource
On Error Resume Next
If Combo1.Text <> "" Then
me.WebBrowser1.Navigate "view-source:" & Me.WebBrowser1.LocationURL 'view source
  else
'nothing here
  End If
end sub
```

