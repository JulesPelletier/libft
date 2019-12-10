
# Libft

## Ta propre bibliothèque à toi tout seul

_Résumé: Ce projet a pour objectif de vous faire coder enCune librairie de fonctions
usuelles que vous pourrez utiliser dans tous vos prochains projets._


## Table des matières

- I Introduction
- II Règles communes
   - II.1 Considérations techniques
   - II.2 Part 1 - Fonctions de la libc
   - II.3 Part 2 - Fonctions supplémentaires
- III Partie bonus


### Part 1 - Fonctions de la libc


Vous devez recoder les fonctions suivantes. Ces fonctions ne nécessitent aucune fonction externe :

- memset
- bzero
- memcpy
- memccpy
- memmove
- memchr
- memcmp
- strlen
- isalpha
- isdigit
- isalnum
- isascii
- isprint
- toupper
- tolower
- strchr
- strrchr
- strncmp
- strlcpy
- strlcat
- strnstr
- atoi
- calloc
- strdup

### Part 2 - Fonctions supplémentaires

| Function name	| ft_substr |
|---------------|-----------|
| Prototype     | char *ft_substr(char const *s, unsigned int start, size_t len); |
|Paramètres		| #1. La chaine de laquelle extraire la nouvelle chaine |
|				| #2. L’index de début de la nouvelle chaine dans la chaine ’s’.|
|				| #3. La taille maximale de la nouvelle chaine.|
|Valeur de retour |La nouvelle chaine de caractere. NULL si l’allocation échoue. |
|Fonctions externes autorisées | malloc|

##

| Function name	| ft_strjoin |
|---------------|-----------|
| Prototype     | char *ft_strjoin(char const *s1, char const *s2); |
|Paramètres		| #1. La chaine de caractères préfixe.|
|				| #2. La chaine de caractères suffixe.|
|Valeur de retour |La nouvelle chaine de caractères. NULL si l’allocation échoue. |
|Fonctions externes autorisées | malloc|

## 

| Function name   | ft_strtrim |
|---------------  |-----------|
| Prototype       | char *ft_strtrim(char const *s1, char const *set); |
|Paramètres		  | #1. La chaine de caractères à trimmer.|
|				  | #2. Le set de reference de caractères à trimmer.|
|Valeur de retour |La chaine de caractères trimmée. NULL si l’allocation échoue. |
|Fonctions externes autorisées | malloc|

## 

| Function name	| ft_split |
|---------------|-----------|
| Prototype     | char **ft_split(char const *s, char c); |
| Paramètres		| #1. La chaine de caractères à découper.|
|				| #2. Le caractère délimitant.|
| Valeur de retour |Le tableau de nouvelles chaines de caractères,résultant du découpage. NULL si l’allocation échoue. |
|Fonctions externes autorisées | malloc, free |

## 

| Function name	| ft_itoa |
|---------------|-----------|
| Prototype     | char *ft_itoa(int n); |
|Paramètres		| #1. l’integer à convertir.|
|Valeur de retour |La chaine de caractères représentant l’integer. NULL si l’allocation échoue. |
|Fonctions externes autorisées | malloc|

## 

| Function name	|  ft_strmapi |
|---------------|-----------|
| Prototype     | char *ft_strmapi(char const *s, char (*f)(unsigned int, char)); |
|Paramètres		| #1. La chaine de caractères sur laquelle itérer|
|				|#2. La fonction à appliquer à chaque caractère.|
|Valeur de retour |La chaine de caractères résultant des applications successives de f. Retourne NULL si l’allocation échoue.|
|Fonctions externes autorisées | malloc|

## 

| Function name	|  ft_putchar_fd |
|---------------|-----------|
| Prototype     | void ft_putchar_fd(char c, int fd); |
|Paramètres		| #1. Le caractère à écrire.|
|				|#2. Le file descriptor sur lequel écrire.|
|Valeur de retour |None|
|Fonctions externes autorisées | write|

## 

| Function name	|  ft_putstr_fd |
|---------------|-----------|
| Prototype     | void ft_putstr_fd(char *s, int fd); |
|Paramètres		| #1. La chaine de caractères à écrire.|
|				| #2. Le file descriptor sur lequel écrire.|
|Valeur de retour |None|
|Fonctions externes autorisées | write|

##

| Function name	|  ft_putendl_fd |
|---------------|-----------|
| Prototype     | void ft_putendl_fd(char *s, int fd); |
|Paramètres		| #1. La chaine de caractères à écrire.|
|				| #2. Le file descriptor sur lequel écrire.|
|Valeur de retour |None|
|Fonctions externes autorisées | write|

##

| Function name	|  ft_putnbr_fd |
|---------------|-----------|
| Prototype     | void ft_putnbr_fd(int n, int fd); |
|Paramètres		| #1. L’integer à écrire.|
|				| #2. Le file descriptor sur lequel écrire.|
|Valeur de retour |None|
|Fonctions externes autorisées | write|


### Partie bonus

Si vous avez réussi parfaitement la partie obligatoire, cette section propose quelques
pistes pour aller plus loin. Un peu comme quand vous achetez un DLC pour un jeu vidéo.


Function name ft_lstnew
Prototype t_list *ft_lstnew(void *content);
Fichiers de rendu -
Paramètres #1. Le contenu du nouvel élément.
Valeur de retour Le nouvel element
Fonctions ex-
ternes autorisées
```
```
malloc
```
```
Description Alloue (avec malloc(3)) et renvoie un nouvel
élément. la variable content est initialisée à
l’aide de la valeur du paramètre content. La
variable ’next’ est initialisée à NULL.
```
```
Function name ft_lstadd_front
Prototype void ft_lstadd_front(t_list **alst, t_list *new);
Fichiers de rendu -
Paramètres #1. L’adresse du pointeur vers le premier élément
de la liste.
#2. L’adresse du pointeur vers l’élément à rajouter
à la liste.
Valeur de retour None
Fonctions ex-
ternes autorisées
```
```
None
```
```
Description Ajoute l’élément ’new’ au début de la liste.
```
```
Function name ft_lstsize
Prototype int ft_lstsize(t_list *lst);
Fichiers de rendu -
Paramètres #1. Le début de la liste.
Valeur de retour Taille de la liste.
Fonctions ex-
ternes autorisées
```
```
None
```
```
Description Compte le nombre d’éléments de la liste.
```
```
Function name ft_lstlast
Prototype t_list *ft_lstlast(t_list *lst);
Fichiers de rendu -
Paramètres #1. Le début de la liste.
Valeur de retour Dernier élément de la liste
Fonctions ex-
ternes autorisées
```
```
None
```
```
Description Renvoie le dernier élément de la liste.

Function name ft_lstadd_back
Prototype void ft_lstadd_back(t_list **alst, t_list *new);
Fichiers de rendu -
Paramètres #1. L’adresse du pointeur vers le premier élément
de la liste.
#2. L’adresse du pointeur vers l’élément à rajouter
à la liste.
Valeur de retour None
Fonctions ex-
ternes autorisées
```
```
None
```
```
Description Ajoute l’élément new à la fin de la liste.
```
```
Function name ft_lstdelone
Prototype void ft_lstdelone(t_list *lst, void (*del)(void
*));
Fichiers de rendu -
Paramètres #1. L’élement à free
#2. L’adresse de la fonction permettant de
supprimer le contenu de l’élement.
Valeur de retour None
Fonctions ex-
ternes autorisées
```
```
None
```
```
Description Libère la mémoire de l’élément passé en argument
en utilisant la fonction del puis avec free(3). La
mémoire de next ne doit pas être free.
```
```
Function name ft_lstclear
Prototype void ft_lstclear(t_list **lst, void (*del)(void
*));
Fichiers de rendu -
Paramètres #1. L’adresse du pointeur vers un élément.
#2. L’adresse de la fonction permettant de
supprimer le contenu d’un élément.
Valeur de retour None
Fonctions ex-
ternes autorisées
```
```
free
```
```
Description Supprime et libère la mémoire de l’élément passé en
paramètre, et de tous les élements qui suivent, à
l’aide de del et de free(3)
Enfin, le pointeur initial doit être mis à NULL.
```

Libft Ta propre bibliothèque à toi tout seul

```
Function name ft_lstiter
Prototype void ft_lstiter(t_list *lst, void (*f)(void *));
Fichiers de rendu -
Paramètres #1 L’adresse du pointeur vers un élément.
#2. L’adresse de la fonction à appliquer.
Valeur de retour None
Fonctions ex-
ternes autorisées
```
```
None
```
```
Description Itère sur la list lst et applique la fonction f au
contenu chaque élément.
```
```
Function name ft_lstmap
Prototype t_list *ft_lstmap(t_list *lst, void *(*f)(void *),
void (*del)(void *));
Fichiers de rendu -
Paramètres #1. L’adresse du pointeur vers un élément.
#2. L’adresse de la fonction à appliquer.
Valeur de retour La nouvelle liste. NULL si l’allocation échoue.
Fonctions ex-
ternes autorisées
```
```
malloc, free
```
```
Description Itère sur la liste lst et applique la fonction f au
contenu de chaque élément. Crée une nouvelle liste
résultant des applications successives de f. la
fonction del est la pour detruire le contenu d un
element si necessaire
```
```
Vous êtes libres d’ajouter des fonctions à votre libft à votre guise.
```

