# Life in Weeks

This is an interactive map of my life, where each week I've been alive is a little box. The box's border color represents where I was living, the fill color what I was doing. Tap a box to see what I was doing where that week.

I made this to help myself see the bigger picture of the road I've walked.

Read more about [Life in Weeks at Wait But Why](https://waitbutwhy.com/2014/05/life-weeks.html).

This code was copied and adapted from [Buster Benson](https://busterbenson.com/life-in-weeks). It is a single webpage statically-rendered with [Hugo](https://gohugo.io/) hosted on Netlify. It consists of two [data](data/events.yml) [files](data/colors.yml), [an introduction](content/index.md), and a [template](layouts/_default/index.html).

## 🚀 Setup

1. Install Hugo:
   ```sh
   brew install hugo  # Mac
   ```
2. Clone and run locally:
```sh
    git clone https://github.com/ginatrapani/life-in-weeks.git
    cd life-in-weeks
    hugo server -D
```
3. Visit [http://localhost:1313/](http://localhost:1313/).

## ✨ Customize

- `content/` → Page content
- `layouts/` → Templates
- `assets/scss/` → Styles
- `assets/imgs/` → Site-wide images
- `static/` → Unprocessed assets
- `hugo.toml` → Site settings

## Colophon

This page uses [Bootstrap](https://getbootstrap.com/) for layout and interaction, and a smidge of [jQuery](https://jquery.com/) to reflect the current week on the map.

The font is [IBM Plex Sans](https://fonts.google.com/specimen/IBM+Plex+Sans) loaded from Google Fonts. The color scheme features a calming pine green aesthetic. Edited in [Zed](https://zed.dev).

## Recent Updates

### Tooltip System Improvements (Latest)
- **Selective Tooltips**: Removed tooltips from empty week boxes to reduce visual clutter while preserving them for meaningful events and birthdays
- **Week-Based Numbering**: Replaced calendar dates in tooltips with cumulative week numbers from birth (e.g., "Week 1300 – Turned 25 years old")
- **Conditional Rendering**: Implemented smart tooltip activation using `hasTooltip` flag for better performance and user experience

### Design & Typography
- **Pine Green Theme**: Replaced orange accent colors with a calming pine green color palette
- **Typography Upgrade**: Switched from Red Hat Display to IBM Plex Sans for better web performance and readability
- **Font Loading**: Migrated from local font files to Google Fonts CDN for improved loading

### Navigation & UX Improvements
- **Smart Scroll Padding**: Implemented dynamic scroll padding using CSS custom properties instead of fixed pixel values
- **Responsive Navigation**: Enhanced navbar padding system that automatically adjusts for different screen sizes
- **Improved Anchor Links**: Fixed navigation scroll positioning to properly account for sticky header height

### Technical Enhancements
- **CSS Architecture**: Introduced CSS custom properties for maintainable color and spacing systems
- **Dynamic Calculations**: Navbar height now automatically calculated based on font sizes and padding
- **Consistent Theming**: Centralized color management through CSS variables

## More Life in Weeks

There are several neat Life in Weeks examples and tools, including:

- [Weeksofyour.life](https://www.weeksofyour.life/): Make your own, completely browser-based
- [Life Calendar](https://lifecalendar.io): Make your own, with multiple layers
- [My Life in Days](https://days.sonnet.io/): Beautiful refactor, by days

🍯 “I always get to where I am going by walking away from where I have been.” – Winnie the Pooh
