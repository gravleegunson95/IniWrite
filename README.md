# IniWrite
i("Key1", "ExpectedValue1") _SaveIni("Key2", "ExpectedValue2") _SaveIni("Key3", "ExpectedValue3")  Func _SaveIni($_sKey, $_sValue)     Local $sFilePath = @ScriptDir &amp; "\FilePath.ini"     Local $sSection = "Section"     Local $sIniRead = IniRead($sFilePath, $sSection, $_sKey, "")     If $sIniRead = $_sValue Then Return     IniWrite($sFilePath, $sSection, $_sKey, $_sValue) EndFunc
