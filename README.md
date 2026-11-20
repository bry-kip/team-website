# Team Name: Vic & Bry

**Live site:**[ https://username.github.io/team-website/](https://bry-kip.github.io/team-website/)

## Team: Vic & Bry

| Name            | Registration no. | GitHub username |
| --------------- | ---------------- | --------------- |
| Victor Mutugi   | COM/3415/26      | MG-studio1      |
| Brian Kiprotich | COM/3447/26      | bry-kip         |

## Who drove each part

Brian Kiprotich- Part 0, 2, 4:
Victor Mutugi- Part 1, 3:

## Personalisation

- Our colours: Midnight Navy `#16283F` (light mode primary) and Champagne Gold `#D9B98C` (dark mode primary) on a warm ivory background `#F7F5F0` / dark background `#0E141E`.
- Contrast checked with WebAIM Contrast Checker: Primary `#16283F` on white = 15.2:1, White text on `#16283F` = 15.2:1, Muted `#5D6875` on `#F7F5F0` = 5.5:1, Champagne `#D9B98C` on `#0E141E` = 8.4:1. All pass WCAG AA 4.5:1.
- Projects we added: git & github setup page and html page
- Extension challenge(s) completed: Added a fourth page from the projects (FAQ page)

## Reflection

1. A div element has no built-in keyboard support like focus or activation with enter/space and the biult-in semantics because it is not announced as a button by assistive technology.

2. The script would break because the browser parses HTNML from top to bootom and would run the script in head before the body element exist.Defer tells the browser to download the script now run it only afterthe whole html document has been parsed

3. innerHTML treats input as HTML so if a visitor typed a title containing markup the browser would parse and run it causing a croos-site scripting (xss) attack which could steal data or change the page for other visitors. textContent treats input as plain text so as not to run a code and display as harmless text.

4. Browser validation is only a courtesy to help honest users fix mistakes quickly, it is not security. Anyone can turn JavaScript off in DevTools, edit the page, or send a request directly with a tool like curl, bypassing our checks completely. The server is the last line of defence, so it must check everything again and never trust data from the client.

5. localStorage is stored per origin, which is the combination of protocol, host and port. Home and Contact on Live Server share the same origin http://127.0.0.1:5500, so they share the same stored theme. A double-clicked file uses file://, a different origin with its own separate storage, so it cannot see the theme saved by Live Server.

6. The <header> and <footer>, including the navigation, logo and theme button, are duplicated in index.html, projects.html and contact.html. If we change the team name or add a new page, we must edit all three files, and forgetting one leaves the site inconsistent. This could be avoided by using a component or template system, like in a framework, where the header is written once and reused on every page.
