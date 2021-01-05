# Git flow

### Installation

```sh
$ apt-get install git-flow
```

### Iniciando

```sh
$ git flow init

Initialized empty Git repository in ~/project/.git/
No branches exist yet. Base branches must be created now.
Branch name for production releases: [master]
Branch name for "next release" development: [develop]


How to name your supporting branch prefixes?
Feature branches? [feature/]
Release branches? [release/]
Hotfix branches? [hotfix/]
Support branches? [support/]
Version tag prefix? []


$ git branch
* develop
 main
```

### Subiendo al repositorio remoto

```sh
$ git remote add origin [url-gitHub]
$ git branch -M develop
$ git push -u origin develop
```

### Ramas

[![N|Solid](<https://wac-cdn.atlassian.com/dam/jcr:b5259cce-6245-49f2-b89b-9871f9ee3fa4/03%20(2).svg?cdnVersion=1389>)](https://www.atlassian.com/es/git/tutorials/comparing-workflows/gitflow-workflow)

# Creacion de una nueva rama (feature)

```sh
$ git flow feature start feature_branch
...
$ git flow feature finish feature_branch
```

# Ramas de publicación

[![N|Solid](<https://wac-cdn.atlassian.com/dam/jcr:a9cea7b7-23c3-41a7-a4e0-affa053d9ea7/04%20(1).svg?cdnVersion=1389>)](https://www.atlassian.com/es/git/tutorials/comparing-workflows/gitflow-workflow)

```sh
$ git flow release start 0.1.0
Switched to a new branch 'release/0.1.0'
...
$ git flow release finish '0.1.0'7
```

# Ramas de corrección

[![N|Solid](<https://wac-cdn.atlassian.com/dam/jcr:61ccc620-5249-4338-be66-94d563f2843c/05%20(2).svg?cdnVersion=1389>)](https://www.atlassian.com/es/git/tutorials/comparing-workflows/gitflow-workflow)

```sh
$ git flow hotfix start hotfix_branch
...
$ git flow hotfix finish hotfix_branch
```
