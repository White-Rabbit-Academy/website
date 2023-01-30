# Passage de paramètres

Il existe plusieurs façons de passer des paramètres à une commande PowerShell :

1. En ligne de commande : Les paramètres peuvent être passés directement en ligne de commande en utilisant le format suivant : `<cmdlet> -parameterName <value>`.
2. Variables : Les paramètres peuvent être passés sous forme de variables. Par exemple : `$param = "value"; <cmdlet> -parameterName $param`.
3. Arguments positionnels : Les paramètres peuvent être passés en utilisant leur position dans la liste d'arguments. Par exemple : `<cmdlet> <value1> <value2>`.
4. Scripts : Les paramètres peuvent également être passés à un script PowerShell en utilisant les mêmes méthodes que pour les commandes en ligne de commande.

En résumé, les paramètres peuvent être passés à une commande PowerShell en ligne de commande, sous forme de variables, en utilisant leur position dans la liste d'arguments, ou en les passant à un script PowerShell.

