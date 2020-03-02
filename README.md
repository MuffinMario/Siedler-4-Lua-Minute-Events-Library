# Siedler-4-Lua-Minute-Events-Library
Eine easy-to-use library zum benutzen von callback funktionen die zu bestimmten Minuten aufgerufen werden

# Benutzung
- in deine new_game Funktion musst du die Funktion MinuteEvents.new_game() aufrufen
- in deine register_functions Funktion musst du die Funktion MinuteEvents.register_functions() aufrufen
- du benötigst eine Funktion mit dem Namen register_minute_events(), in der du die Funktionen, die zu bestimmten Minuten einmalig aufgerufen werden sollen registrierst

# Beispiel

```lua
-- ... füge hier die library ein

function new_game()
  MinuteEvents.new_game()
end

function register_functions()
  MinuteEvents.register_functions()
end

function testFunc()
  dbg.stm("testfunc")
end

function register_minute_events()
  requestMinuteEvent(testFunc,5)
end```
