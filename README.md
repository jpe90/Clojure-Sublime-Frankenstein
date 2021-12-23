Fork of [Clojure Sublimed](https://github.com/tonsky/Clojure-Sublimed) with [Tutkain's](https://github.com/eerohele/Tutkain) indentation hacked in

Below are (MacOS) bindings which you can add to your User keybindings to indent properly on newline and to add an Emacs style re-indent:

```
{
    "keys": ["enter"],
    "command": "tutkain_insert_newline",
    "context": [
      {
        "key": "selector",
        "operator": "equal",
        "operand": "source.edn | source.clojure"
      },
      {
        "key": "auto_complete_visible",
        "operator": "equal",
        "operand": false
      },
      {
        "key": "panel_has_focus",
        "operator": "equal",
        "operand": false
      },
    ]
  },
   {
     "keys": ["option+tab"],
     "command": "tutkain_indent_sexp",
     "context": [
         {"key": "selector", "operator": "equal", "operand": "source.edn | source.clojure"},
         {"key": "auto_complete_visible", "operand": false},
         {"key": "has_next_field", "operand": false},
     ]
 },
```
