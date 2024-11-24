# How to use it

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

### Profile picture

- `profile_picture`

Example :

```yml
profile_picture: https://dummyimage.com/600x600/
```

### Experiences

- `experiences`

Each `experience` has a `title`, and a `description`. You can also add a `start_date` and `end_date`.

You can set `start_date` without `end_date`, this will put "now" instead.

Example :

```yml
experiences:
  - title: First experience
    description: First experience description
    start_date: 2024-01-01
  - title: Second experience
    description: Second experience description
    start_date: 2023-01-01
    end_date: 2023-12-31
```

### Education

- `educations`

Each `education` has a `title`, and a `description`. You can also add a `start_date` and `end_date`.

You can set `start_date` without `end_date`, this will put "now" instead.

```yml
educations:
  - title: First education
    description: First education description
    start_date: 2024-01-01
  - title: Second education
    description: Second education description
    start_date: 2023-01-01
    end_date: 2023-12-31
```

### Titles override

You can override titles with ease with those variables. You don't need to define them, as they have default values.

```yml
main_title: Main title override
basic_informations_section_title: Basic infos title override
personnal_links_section_title: Links title override
experiences_section_title: Experiences title override
education_section_title: Education title overrride
```

### Personnal links

You can add links to your CV, those variables are optionnal. The link will appear only if the associated variable is defined.

```yml
personnal_links:
  github: https://example.com/
  gitlab: https://example.com/
  linkedin: https://example.com/
  facebook: https://example.com/
  youtube: https://example.com/
  Instagram: https://example.com/
  tiktok: https://example.com/
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
  profile_picture: https://dummyimage.com/600x600/
  main_title: Main title override
  basic_informations_section_title: Basic infos title override
  personnal_links_section_title: Links title override
  experiences_section_title: Experiences title override
  education_section_title: Education title overrride
  personnal_links:
    github: https://example.com/
    gitlab: https://example.com/
    linkedin: https://example.com/
    facebook: https://example.com/
    youtube: https://example.com/
    Instagram: https://example.com/
    tiktok: https://example.com/
  experiences:
    - title: First experience
      description: First experience description
      start_date: 2024-01-01
    - title: Second experience
      description: Second experience description
      start_date: 2023-01-01
      end_date: 2023-12-31
  educations:
    - title: First education
      description: First education description
      start_date: 2024-01-01
    - title: Second education
      description: Second education description
      start_date: 2023-01-01
      end_date: 2023-12-31
```
