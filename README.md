# qb-notify-replace
replaces default qbcore notify with okokNotify


- **1 Go To qb-core/client/functions.lua**

- **2 Find The Following Code: This Is Located Around Line 88**

- **3 Delete From Around Line 88 To Around 111 Where The End Of That Function Is**

- **4 Paste The Following Code In To Replace That Code!**


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

![image](https://github.com/kocaka14/qb-notify-replace/assets/101359455/f890b16b-0435-4a5d-8b16-944227ac6fd7)

