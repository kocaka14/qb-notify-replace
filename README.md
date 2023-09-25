# qb-notify-replace
replaces default qbcore notify with okokNotify

## Join discord for more [Discord](https://discord.com/invite/eWBEM4eRD2)

[![Discord Presence](https://lanyard.cnrad.dev/api/703985319774650489)](https://discord.com/users/703985319774650489)

- **1 Go To qb-core/client/functions.lua**

- **2 Find The Following Code: This Is Located Around Line 88**

- **3 Delete From Around Line 88 To Around 111 Where The End Of That Function Is**

- **4 Paste The Following Code!**


 ```
QBCore.Functions.Notify = function(Message, Type, Time, Title)
    local Title = Title ~= nil and Title or "Notification"
    local Message = Message ~= nil and Message or "Message"
    local Time = Time ~= nil and Time or 2000
    local Type = Type ~= nil and Type or "info"
    if ttype == 'primary' then ttype = 'info' end
    exports['okokNotify']:Alert(Title, Message, Time, Type)
end
```

I also give you an css edited Okok-Notify

![image](https://github.com/kocaka14/qb-notify-replace/assets/101359455/f890b16b-0435-4a5d-8b16-944227ac6fd7)
