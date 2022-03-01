# Configuration de Github Au Protocole SSH

Ici j'aborde la configuration d'un compte github au protocole SSH

## Pourquoi Configurer SSH 

Pourquoi configurer SSH:
* parcequ'il facilite la connexion de son compte local vers githib
* il est très utile aussi pour la double authitification.
* il permet l'utilisation du protocole **SSH** au profit de **HTTPS** cela nous permet d'éviter à taper les **identifiants** à chaque opération de **push**, **clone**, ....

### Génération de la Clé SSH

<pre>
<code>
	ssh-keygen
</code>
</pre>

## Pour l'Agent SSH

<pre>
<code>
	eval ssh-agent
</code>
</pre>

## Utiliser Une Clé Spécifique 

<pre>
<code>
	ssh-add lienClePrive
</code>
</pre>

## En cas de Problème

Si vous rencontrez ce problème:
<code>**Could not open a connection to your authentication agent.**</code>

* D'abord vous vous rendez dans le dossier bin avec la commande suivante
<pre>
<code>
	ssh-agent /bin/sh
</code>
</pre>
