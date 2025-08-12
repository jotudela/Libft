# 📚 Libft

Libft est une bibliothèque en langage C réimplémentant plusieurs fonctions standards ainsi que des utilitaires supplémentaires.  
Elle constitue une base solide pour de futurs projets C en fournissant des outils fiables et réutilisables.

---

## 📂 Fonctions

### Partie 1 — Fonctions de la libc
| Fonction       | Prototype                                       |
|----------------|------------------------------------------------|
| ft_atoi        | `int ft_atoi(const char *str);`                |
| ft_bzero       | `void ft_bzero(void *s, size_t n);`            |
| ft_calloc      | `void *ft_calloc(size_t count, size_t size);`  |
| ft_isalnum     | `int ft_isalnum(int c);`                        |
| ft_isalpha     | `int ft_isalpha(int c);`                        |
| ft_isascii     | `int ft_isascii(int c);`                        |
| ft_isdigit     | `int ft_isdigit(int c);`                        |
| ft_isprint     | `int ft_isprint(int c);`                        |
| ft_memccpy     | `void *ft_memccpy(void *dst, const void *src, int c, size_t n);` |
| ft_memchr      | `void *ft_memchr(const void *s, int c, size_t n);` |
| ft_memcmp      | `int ft_memcmp(const void *s1, const void *s2, size_t n);` |
| ft_memcpy      | `void *ft_memcpy(void *dest, const void *src, size_t n);` |
| ft_memmove     | `void *ft_memmove(void *dst, const void *src, size_t len);` |
| ft_memset      | `void *ft_memset(void *b, int c, size_t len);` |
| ft_strchr      | `char *ft_strchr(const char *s, int c);`       |
| ft_strdup      | `char *ft_strdup(const char *s1);`              |
| ft_strlcat     | `size_t ft_strlcat(char *dst, const char *src, size_t dstsize);` |
| ft_strlcpy     | `size_t ft_strlcpy(char *dst, const char *src, size_t dstsize);` |
| ft_strlen      | `size_t ft_strlen(const char *s);`              |
| ft_strncmp     | `int ft_strncmp(const char *s1, const char *s2, size_t n);` |
| ft_strnstr     | `char *ft_strnstr(const char *haystack, const char *needle, size_t len);` |
| ft_strrchr     | `char *ft_strrchr(const char *s, int c);`       |
| ft_tolower     | `int ft_tolower(int c);`                         |
| ft_toupper     | `int ft_toupper(int c);`                         |

### Partie 2 — Fonctions supplémentaires
| ft_itoa        | `char *ft_itoa(int n);`                          |
| ft_putchar_fd  | `void ft_putchar_fd(char c, int fd);`            |
| ft_putendl_fd  | `void ft_putendl_fd(char *s, int fd);`           |
| ft_putnbr_fd   | `void ft_putnbr_fd(int n, int fd);`               |
| ft_putstr_fd   | `void ft_putstr_fd(char *s, int fd);`             |
| ft_split       | `char **ft_split(char const *s, char c);`        |
| ft_strjoin     | `char *ft_strjoin(char const *s1, char const *s2);` |
| ft_strmapi     | `char *ft_strmapi(char const *s, char (*f)(unsigned int, char));` |
| ft_strtrim     | `char *ft_strtrim(char const *s1, char const *set);` |
| ft_substr      | `char *ft_substr(char const *s, unsigned int start, size_t len);` |
| ft_striteri    | `void ft_striteri(char *s, void (*f)(unsigned int, char*));` |

### Bonus — Listes chaînées
| ft_lstnew       | `t_list *ft_lstnew(void *content);`              |
| ft_lstadd_front | `void ft_lstadd_front(t_list **lst, t_list *new);` |
| ft_lstsize      | `int ft_lstsize(t_list *lst);`                    |
| ft_lstlast      | `t_list *ft_lstlast(t_list *lst);`                |
| ft_lstadd_back  | `void ft_lstadd_back(t_list **lst, t_list *new);`  |
| ft_lstdelone    | `void ft_lstdelone(t_list *lst, void (*del)(void *));` |
| ft_lstclear     | `void ft_lstclear(t_list **lst, void (*del)(void *));` |
| ft_lstiter      | `void ft_lstiter(t_list *lst, void (*f)(void *));`  |
| ft_lstmap       | `t_list *ft_lstmap(t_list *lst, void *(*f)(void *), void (*del)(void *));` |

---

## 💾 Installation
```bash
git clone https://github.com/ton-utilisateur/libft.git
cd libft
make
```
Cela génère le fichier `libft.a` à l'intérieur du dossier.

---

## 🛠 Utilisation
Inclure `libft.h` dans vos fichiers C, puis compiler avec la bibliothèque :
```bash
gcc main.c libft.a -o programme
```

---

## 🧪 Tests
Vous pouvez utiliser vos propres tests ou un framework de test externe :
```bash
make test
```

---

## 🤝 Contribution
Les contributions sont les bienvenues !

1. Fork le projet  
2. Crée une branche (`git checkout -b feature/ma-fonction`)  
3. Commit (`git commit -m "Ajout de ma fonction"`)  
4. Push (`git push origin feature/ma-fonction`)  
5. Ouvre une Pull Request

---

## 📜 Licence
MIT
