# API contract — the title from PROPOSAL.md §1

> **The login rows are written by you, by hand, before you ask an assistant for any code.**
> They are this week's decision: what a client sends, what comes back, and every way it can
> fail. The code is written from them, not the other way round.
>
> **Giriş satırlarını, bir asistandan herhangi bir kod istemeden önce, siz elle yazarsınız.**
> Bu haftanın kararı onlardır: istemcinin ne gönderdiği, ne döndüğü ve her başarısızlık
> durumu. Kod onlardan yazılır, tersi değil.
>
> Delete these quoted lines before you commit. / Commit etmeden önce bu alıntı satırlarını silin.

<!--
ONE ROW FOR EACH ENDPOINT OF YOUR SERVER (server/main.py).

Method:   GET, POST, PUT, PATCH or DELETE.
Path:     begins with /, such as /auth/code. A part that changes goes in braces: /rooms/{room_id}.
Request:  what the client sends: the JSON body, or a header such as Authorization: Bearer <token>.
          Write — if it sends nothing.
Response: the status code when it works, and what comes back: 200 {"sent": true}.
Errors:   every way it can fail, each with its status code: 422 not an e-mail address · 429 too soon.
REQ:      the requirements it serves, as in week02/requirements.json. — for a technical
          endpoint such as /health.

The checker compares this table with the routes in server/: the same method and the same
path, in both directions. An endpoint that is not built yet still has its route; it answers
501 until its week comes.

STRONG: | POST | /bookings | {"room": 3, "start": "16:00", "minutes": 90} | 201 {"booking_id": 12} | 409 the slot is taken · 422 minutes not between 30 and 120 · 401 not logged in | REQ-002 |

Replace the [bracketed] row with your own rows; the login (REQ-001) needs at least two.
Bu tablonun Türkçe açıklaması ASSIGNMENT_05_TR.md §2'dedir.
Delete this comment when you are done.
-->

| Method | Path | Request | Response | Errors | REQ |
|---|---|---|---|---|---|
| GET | /health | — | 200 {"status": "ok"} | — | — |
| [POST] | [/auth/…] | [what the client sends] | [200 and what comes back] | [status code: when] | REQ-001 |
