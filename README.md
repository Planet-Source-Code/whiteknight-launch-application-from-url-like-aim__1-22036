<div align="center">

## Launch Application From URL Like AIM


</div>

### Description

This tells how to launch a program from a web browser by typping in a url like AIM (e.g. myapp:// would launch c:\program files\myapp\myapp.exe)
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[whiteknight](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/whiteknight.md)
**Level**          |Intermediate
**User Rating**    |4.2 (25 globes from 6 users)
**Compatibility**  |VB 5\.0, VB 6\.0
**Category**       |[Registry](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/registry__1-36.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/whiteknight-launch-application-from-url-like-aim__1-22036/archive/master.zip)





### Source Code

In the Regestry <a id="key" style="cursor:default;color:blue;">HKEY_CLASSES_ROOT</a> Create a Key named what you want the 'protocol' to be (e.g. myapp).<br> The '<a id="key" style="cursor:default;color:blue;">(Default)</a>' value for that key is a description of the protocol.<br> A Subvalue needs to be created named '<a id="key" style="cursor:default;color:blue;">URLProtocol</a>' the value of this is "".<br> Then create a New SubKey to the protocol Key name it '<a id="key" style="cursor:default;color:blue;">shell</a>', no values need to be set here.<br> Now create a SubKey to '<a id="key" style="cursor:default;color:blue;">shell</a>', name this '<a id="key" style="cursor:default;color:blue;">open</a>', no values to set. Next create asubkey to '<a id="key" style="cursor:default;color:blue;">open</a>', name this '<a id="key" style="cursor:default;color:blue;">command</a>'.<br> The '<a id="key" style="cursor:default;color:blue;">(Default)</a>' value for this key is the path to the application(e.g. c:\program files\myapp\myapp.exe %1).<br> The '<a id="key" style="cursor:default;color:blue;">%1</a> will return any command line params to your application, i.e. any thing after the '<a id="key" style="cursor:default;color:blue;">myapp://</a>' will be returned. <br><br>
Thats it now you can open up your browser and type in the protocol (e.g. myapp://) and your application will launch. <BR><BR>
I have tested that so It does work. <BR><BR>If you like this please post comments and vote.
if anyone knows how to see if commands are passed please either post how in the comments or email me @ witenite87@excite.com.<BR><BR><BR>
Download a working use of this in a Win32 Whois Client. It Looks like other windows utilities like ping, ipconfig ect. It does NOT use the winsock ocx it uses winsock API. Its FREE so Get it now. <a href="http://camalot.virtualave.net" target="_whois">Download the WhoIs Client Here</a>

