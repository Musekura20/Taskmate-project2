# TaskMate: Plain CSS and Tailwind CSS

For this task, I took my TaskMate website and built it again using only Tailwind CSS. This repo has both versions so you can compare them.

```
Plain css version/   index.html, settings.html, dashboard.html, css/style.css, images/   (my first version)
Tailwind version/    index.html, settings.html, dashboard.html, images/                  (Tailwind version)
```

## What changed in the way I work

**I stopped jumping between two files.**
With plain CSS, I wrote my HTML, then opened `style.css` to design it, then went back to the HTML. With Tailwind, I write the style directly on the element, like `flex`, `gap-5` or `px-[7%]`. Everything is in one place, so it felt faster.

**I did not have to think of class names anymore.**
Before, I had to create names like `.stat-card` or `.settings-list` and make sure they matched in the HTML and the CSS. With Tailwind, I just describe how I want the element to look.

**Headings looked plain at first.**
After I added Tailwind, my headings became small and not bold. So I had to add sizes and bold myself, like `text-2xl font-bold`.

**I now start with the small screen.**
In plain CSS, I used `max-width` for mobile. In Tailwind, I design for mobile first, then use `sm:` and `md:` for bigger screens. For example, `grid-cols-1 md:grid-cols-3` means one column on a phone and three columns on a bigger screen.

**Hover was easy.**
In plain CSS I wrote a separate hover rule. Now I just add `hover:bg-[#ca5aef]` to the same element.

**I kept my own colors.**
My design uses exact colors, so I used square brackets, like `bg-[#877bf4]` and `w-[230px]`.

**The one design change I made.**
The sidebar and the settings panel now go all the way to the bottom and stay in place when I scroll the page. I did this with `md:sticky md:top-0 md:h-screen`. Everything else looks the same as before.

## Setup

I used the Tailwind CDN link (one `<script>` tag in the head), so I did not install anything.
