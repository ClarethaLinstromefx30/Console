# Console
ConsoleEraseLine($vIn) ; Erase one line (only) from console output (DOS only, not SciTE) ; $vIn = Line_to_Erase ; Does NOT work if line ends with @LF !!     If StringRight($vIn, 1) = @LF Then Return     Local $sOut = ""     For $i = 1 To StringLen($vIn)         $sOut &amp;= Chr(8) &amp; " " &amp; Chr(8)     Next     ConsoleWrite($sOut) EndFunc  ;==>_ConsoleEraseLine
