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

So when you write .flare scripts, you will automaticly be in the (superior)script-environment,
but to access a parallel environment like shell in the superior environment, use this ```<?SHELL ?>```

example:
```
// SCRIPT environment
<?SHELL
// SHELL environment
flare: true
?>

// back to SCRIPT environment
()hello ->
  alert hello world!
```

##Declarations
I will try my best to make the best, shortest but readable compiler language.

```
--- FLARESCRIPT ---

hello = world

(str)shout ->
  alert str

shout woohoo

--- JAVASCRIPT ---

var hello;
hello = 'world';

var shout = function(str) {
  alert(str);
}

shout('woohoo');
```
