---
title: Considering graduate studies
summary: An short primer about grad studies
authors: [Jean-Pierre Hickey]
tags: []
categories: []
date: "2021-01-01T00:00:00Z"
slides:
  # Choose a theme from https://github.com/hakimel/reveal.js#theming
  theme: black
  # Choose a code highlighting style (if highlighting enabled in `params.toml`)
  #   Light style: github. Dark style: dracula (default).
  #References
  #http://www.tonysaad.net/uncategorized/how-to-fail-in-grad-school/
  highlight_style: dracula
---

# Are graduate studies for me?

[MPILAB](https://mpilab.ca/) | [UWaterloo](https://uwaterloo.ca)

---

## Questions to ask onself

- Why do I want to go to graduate school?
- What type of career to I hope to achieve?
- How will a graduate degree help me reach my goals?

---
## Type of people that do well in graduate school

- Intellectually curious, self-motivated
- Focused on long-term personal development
- Seeking research/technical career focus


---

## Skills that will be developed: technical skills

- Programing
- High-performance computing
- Technical writing and communication
- Computational physics
- Application of fluid mechanics


---

## Skills that will be developed: soft skills

- Time-management
- long-term project management
- Independent thought

---

## Math

In-line math: $x + y = z$

Block math:

$$
f\left( x \right) = \;\frac{{2\left( {x + 4} \right)\left( {x - 4} \right)}}{{\left( {x + 4} \right)\left( {x + 1} \right)}}
$$

---

## Fragments

Make content appear incrementally

```
{{%/* fragment */%}} One {{%/* /fragment */%}}
{{%/* fragment */%}} **Two** {{%/* /fragment */%}}
{{%/* fragment */%}} Three {{%/* /fragment */%}}
```

Press `Space` to play!

{{% fragment %}} One {{% /fragment %}}
{{% fragment %}} **Two** {{% /fragment %}}
{{% fragment %}} Three {{% /fragment %}}

---

A fragment can accept two optional parameters:

- `class`: use a custom style (requires definition in custom CSS)
- `weight`: sets the order in which a fragment appears

---


---

## Themes

- black: Black background, white text, blue links (default)
- white: White background, black text, blue links
- league: Gray background, white text, blue links
- beige: Beige background, dark text, brown links
- sky: Blue background, thin dark text, blue links

---

- night: Black background, thick white text, orange links
- serif: Cappuccino background, gray text, brown links
- simple: White background, black text, blue links
- solarized: Cream-colored background, dark green text, blue links

---

{{< slide background-image="/media/boards.jpg" >}}

## Custom Slide

Customize the slide style and background

```markdown
{{</* slide background-image="/media/boards.jpg" */>}}
{{</* slide background-color="#0000FF" */>}}
{{</* slide class="my-style" */>}}
```

---

## Custom CSS Example

Let's make headers navy colored.

Create `assets/css/reveal_custom.css` with:

```css
.reveal section h1,
.reveal section h2,
.reveal section h3 {
  color: navy;
}
```

---

# Questions?

[Ask](https://github.com/wowchemy/wowchemy-hugo-modules/discussions)

[Documentation](https://wowchemy.com/docs/managing-content/#create-slides)
