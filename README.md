#README
This is my first compiler, wish me luck! :-)

##Environments
```
DOCUMENT(doc) ->
  Flare(flare) ->
    Shell(shell)
    Script(script) -- Default environment
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

Even though there can me multiple environments in the same environment,
only one can be the superior environment.

So when you write .flare scripts, you will automaticly be in the script-environment,
but to access a parallel environment like shell in the superior environment, use this ```<?SHELL ?>```

example:
```
<?SHELL
flare: true
?>

()hello ->
  alert hello world!
```
