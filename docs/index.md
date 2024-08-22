# MkDocs curriculum vitae theme

A MkDocs theme, made for curriculum vitae.

This theme allows you to generate a curriculum vitae, without markdown, only configuration with variables.

## How to use it

In you `mkdocs.yml` file, put the curriculum-vitae theme :

```yml
theme:
  name: curriculum-vitae
```

Next, you just have to create a `docs` folder in your repo, and only put an empty `index.md`.

## Configuration

What you have to do is play with the theme variables :

### Basic informations

- `firstname`
- `lastname`
- `mail`
- `location`

Example :

```yml
firstname: John
lastname: Doe
mail: john.doe@example.com
location: Tours
```

### Experiences

- `experiences`

Each `experience` has a `title`, and a `description`.

Example :

```yml
experiences:
  - title: First experience
    description: First experience description
  - title: Second experience
    description: Second experience description
```

### Education

- `schools`

Each `school` has a `title`, and a `description`.

```yml
schools:
  - title: First school
    description: First school description
  - title: Second school
    description: Second school description
```

### Full Example

```yml
# mkdocs.yml

theme:
  name: curriculum-vitae
  firstname: John
  lastname: Doe
  mail: john.doe@example.com
  location: Tours
  experiences:
    - title: First experience
      description: First experience description
    - title: Second experience
      description: Second experience description
  schools:
    - title: First school
      description: First school description
    - title: Second school
      description: Second school description
```
