# rotn-content

Prose, scenes, dialogue and quest copy for rotn. Venice lane only.
Coders never clone this repo; they consume generated types from
`rotn-src/src/generated/content-types.ts`.

Layout: `schema/` (one JSON Schema per type), `scenes/`, `realms/`,
`quests/`. Every file needs a unique slug `id` matching
`^[a-z0-9]+(-[a-z0-9]+)*$`. Ids are never renumbered; a rename is a new
id plus an alias.

Validate and emit types from `rotn-src`: `npm run content:types`.
