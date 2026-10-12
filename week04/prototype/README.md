# Your clickable prototype

A prototype shows how the app will be used before any of it is built. Nothing here is
real: there is no server, and the data is invented. What is real is the flow, which shows
which screen comes after which, what each screen asks for, and what the user sees when
something goes wrong.

**The rules**

- One HTML file for each screen, all in this folder. `index.html` is the first screen.
- It opens with a double click on `index.html`: no server, no framework, no build step.
  Plain HTML, the shared `style.css`, and a few lines of JavaScript where a screen has to
  react, as in `code.html`.
- Every screen can be reached from `index.html` by clicking, and every link leads to a
  screen that exists. Write each link with the full file name, in lower case and in
  quotes: `href="rooms.html"`. The checker follows only links written this way.
- Every screen has a comment near the top that names the requirements it serves:
  `<!-- serves: REQ-001, REQ-006 -->`. That is how a screen is traced back to the
  requirement it exists for. If your phone-screen requirement is not REQ-006, change
  REQ-006 to its id in the three starter screens.
- The invented data is the same every time, so that your collaborator can follow the steps of a
  test case. In `code.html` the correct code is always 1234; write the invented values that
  your own screens use in this file, under "Invented data".
  Choose them from your acceptance criteria: a free slot and a busy one, a right code and a
  wrong one, an empty list, the edge values. Your assistant can propose them; you approve
  them and use the same values on every screen. No real names or e-mail addresses.
- There is no server, so a screen remembers nothing: after a booking, the next screen shows
  the same fixed data with that booking already in it.
- When you ask an assistant for a screen, tell it: plain HTML and CSS, one file for the
  screen, the `style.css` of this folder, no framework. One screen, one commit.
- Look at every screen 390 px wide. In Chrome or Edge, press F12 and then the phone icon
  (Ctrl+Shift+M, or Cmd+Shift+M on a Mac), and choose a width of 390.

The three starter screens (`index.html`, `code.html`, `home.html`) are the login that
everyone shares (REQ-001). Replace the [bracketed] parts, then build your main flow from
`home.html` onwards.

**Invented data**

- Login code: 1234
