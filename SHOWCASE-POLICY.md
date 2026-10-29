# Showcase publication policy

## Two separate purposes

The private development repository remains the working source for implementation, tests, operational records and releases. This public repository contains curated presentation material only. It is not a mirror and is not used to deploy the application.

## Allowed here

- Newly written product explanations and conceptual diagrams.
- Fictional examples clearly labelled as such.
- Future screenshots from a disposable synthetic demo, after visual and metadata review.
- General engineering lessons without private incident details.

## Excluded

- Real names, care records, photos or account details.
- Credentials, tokens, cookies, private keys or configuration exports.
- Production addresses, internal hostnames, personal filesystem paths or raw logs.
- Private source history, agent conversations, backups or database files.
- Screenshots of production or authenticated private sessions.

## Updating the showcase

1. Keep development changes in the private project.
2. Select a small presentation update; never copy the private Git history.
3. Review wording, images and file metadata for private information and unsupported claims.
4. Run a personal-information scan and a separate credential scan. Inspect findings rather than treating a green scan as a guarantee.
5. Commit only reviewed files using a public/noreply identity and publish deliberately.

There is no automatic synchronization. A future maintainer must preserve this boundary.
