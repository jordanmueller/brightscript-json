Full JSON parser for Roku's proprietary Brightscript


BrightScript JSON Parser
This parser can be used to parse json for the Roku Digital Video Player SDK

Example
**Code**

    Function Main()
        '{
        ' "test" : [
        '  123,
        '  234.4,
        '  9393
        ' ]
        '}
        str = "{"+CHR(34)+"test"+CHR(34)+" : [123,234.4,9393]}"
        json = BSJSON()
        myjson = json.JsonDecode(str)
        
        print myjson["test"][2]
    End Function

**Result**
    9393
