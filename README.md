#README
This is my first compiler, wish me luck! :-)

##Environments
```
DOCUMENT(doc) ->
  Flare(flare) ->
    Shell(shell)
    Script(script)
```

Environments in FLARE is like tags in html5,
and works most like function scopes.

example:
```
<doc>
  <flare>
    <shell>
      inside doc->flare->shell
    </shell>

    <script>
      inside doc->flare->script
    </script>
  </flare>
</doc>
```
