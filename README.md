# A Field Guide to the Command Line

Printable field notes for working at a Linux terminal, in the shape of an old
botanical field guide. Each sheet is one page you can print, pin near the
machine, and write on.

**Read them here: https://cedriccliattjr.github.io/solar-grove-field-guide/**

## The sheets

| | Sheet | Covers |
|---|---|---|
| № 01 | A Field Guide to the Command Line | Moving around, files, pacman and yay, systemd, disk and network, permissions, terminal keys, Hyprland |
| № 02 | The Command Line, Second Season | Git, Docker, storage and fstab, hardware inventory, sound, logs, and traps already sprung |

№ 01 gets you around a machine. № 02 is what you need once you're running
things on it. They're sequential — neither replaces the other.

## Who it's for

Someone who has a Linux machine in front of them and would rather learn it than
be walked through it. You don't need prior terminal experience for № 01. № 02
assumes you're comfortable with № 01 and have started running your own services.

The commands lean toward Arch-based systems (EndeavourOS, pacman, yay) and a
Hyprland desktop, because that's what they were written against. Most of it —
files, git, Docker, systemd, logs — is the same on any Linux.

Every entry is a command you'll actually type, described in the words you'd use
explaining it to someone standing next to you. No exhaustive flag tables; `man`
already does that better.

## Printing

Each sheet is laid out for US Letter portrait. Print from the browser with
backgrounds enabled — in Chrome and Firefox that's the "Background graphics" or
"Print backgrounds" checkbox — or the coloured section bands come out blank.
№ 01 is one page, № 02 is two.

On a narrow screen the two-column plate collapses to one column. The print
layout is unaffected.

## How it's built

Plain HTML and CSS. No framework, no build step, no dependencies. Open any
`.html` file in a browser and it works; GitHub Pages serves the same files
unchanged.

```
index.html          the list of sheets
chapter-01.html     № 01
chapter-02.html     № 02
css/field-guide.css every colour, type role, and shared component
css/index.css       index page layout only
```

The only thing loaded from the network is the webfonts, from Google Fonts.

### Changing the look

`css/field-guide.css` defines the whole visual identity in one `:root` block —
ten colours and three type roles. Change a value there and it changes
everywhere. No page defines a colour of its own, and no HTML file contains a
hex value.

The palette is Solar Grove: an ivory ground with green and brown as accents,
never as the field, and a postal blue to keep it from drifting toward spa.
Pure white and pure black are deliberately absent — both read cold against it.

Type fills three roles: one display serif (Fraunces), one body face (Karla),
one utility monospace (IBM Plex Mono). Utility type is always uppercase and
letter-spaced; body type never is. Swapping in different families is fine as
long as the three roles stay distinct.

## License

MIT — see [LICENSE](LICENSE). Use the sheets, print them, fork them, rewrite
them for your own setup.
