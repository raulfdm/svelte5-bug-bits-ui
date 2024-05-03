# Svelte@5.0.0-next.121 bits-ui bug

![error](./assets/CleanShot%202024-05-03%20at%2017.26.26.png)

This repo was created to show a bug that start happening migrating from `svelte@5.0.0-next.120` to `svelte@5.0.0-next.121` while using shadcn-svelte (bits-ui).

## Repro steps

1. install dependencies:
   ```bash
   npm i
   ```
1. run the dev server:
   ```bash
   npm run dev
   ```
1. open [http://localhost:5173](http://localhost:5173)
1. see the page working. Try to click on "OPEN" and see the dropdown menu

Now, to see the error:

1. stop the server
1. go to package.json, bump svelte to `5.0.0-next.121`
1. run `npm install` again
1. run the dev server again (`npm run dev`)
1. open [http://localhost:5173](http://localhost:5173)
1. refresh the page, it'll be blank
