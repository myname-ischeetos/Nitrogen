## Script
```lua
local owner = "myname-ischeetos"
local branch = "Main"

local function webImport(file)
    local s = ("https://raw.githubusercontent.com/%s/Nitrogen/main/%s/%s.lua"):format(owner, branch, file)
    return loadstring(game:HttpGetAsync(s))()
end

webImport("init")
webImport("ui/main")
```

# Nitrogen
<i>General purpose pen-testing tool for games on the Roblox engine</i>


<p align="center">
    <img src="https://cdn.discordapp.com/attachments/633472429917995038/722143730500501534/Hydroxide_Logo.png"/>
    </br>
    <img src="https://cdn.discordapp.com/attachments/694726636138004593/742408546334933002/unknown.png" width="677px"/>
</p>

## Features
* Upvalue Scanner
    * View/Modify Upvalues
    * View first-level values in table upvalues
    * View information of closure
* Constant Scanner
    * View/Modify Constants
    * View information of closure
* Script Scanner
    * View general information of scripts (source, protos, constants, etc.)
    * Retrieve all protos found in GC
* Module Scanner
    * View general information of modules (return value, source, protos, constants, etc.)
    * Retrieve all protos found in GC
* RemoteSpy
    * Log calls of remote objects (RemoteEvent, RemoteFunction, BindableEvent, BindableFunction)
    * Ignore/Block calls based on parameters passed
    * Traceback calling function/closure
* ClosureSpy
    * Log calls of closures
    * View general information of closures (location, protos, constants, etc.)

More to come, soon.

## Images/Videos
<p align="center">
    <img src="https://i.gyazo.com/63afdd764cdca533af5ebca843217a7e.gif" /> (not Nitrogen)
</p>

