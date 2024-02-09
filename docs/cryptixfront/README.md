This is a [Next.js](https://nextjs.org/) project bootstrapped with
[`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

This project is using [Supabase](https://supabase.com/) as a backend, and has
been started using the
[`-e with-supabase`](https://supabase.com/docs/guides/getting-started/quickstarts/nextjs)
flag.

The complete setup command looks like this:

```bash
npx create-next-app -e with-supabase
```

## Getting Started:

- Pull this project from GitHub

- Install the necessary dependencies;

```bash
npm i
```

- Request the .env.development.local file necessary for working on this project.

- Run the development server:

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the
result.

You can start editing the page by modifying `app/page.tsx`. The page
auto-updates as you edit the file.

This project uses
[`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to
automatically optimize and load Inter, a custom Google Font.

## Architecture

### Frontend

![Project architecture](https://cdn.discordapp.com/attachments/1132366414817275994/1202820875817066506/image.png?ex=65ced93c&is=65bc643c&hm=25269dae69ed90a69c8fda29e01a613a302b3b35306421dd6b929877f4f7d7ca&)

This project uses the [Next.js folder routes]() as the website architecture, and
is thus composed of multiple layers, all contained in the common `app` folder.

> [!WARNING] This folder arrangement is still debated and will probably be
> subject to change in the near future. Do not take the following information
> for granted.

- #### `public`

This folder contains all of the assets and media used on the website, such as
videos, images, CSS files, and all that could apply.

- #### `home`/`landing`

This folder contains both the landing page, used for marketing purposes, and the
home page, used for Getting an overview of news concerning events, artists,
etc...

- #### `auth`

This folder contains all pages related to authentication and user profile
creation and management.

- #### `profile`

This folder contains the profile page for the authenticated user.

- #### `p` (personas)

This folder contains all of the pages related to individuals (users, artists,
and organizers).

> [!NOTE] The content displays changes based on the dynamic parameters in the
> URL, such as the user ID, using
> [Next.js dynamic routes](https://nextjs.org/docs/pages/building-your-application/routing/dynamic-routes).

- #### `e` (entities)

This folder contains all of the pages related to entities (venues, tours,
events, and performances).

> [!NOTE] The content displays changes based on the dynamic parameters in the
> URL, such as the user ID, using
> [Next.js dynamic routes](https://nextjs.org/docs/pages/building-your-application/routing/dynamic-routes).

- #### `marketplace`

This folder contains all of the pages related to the secondary market for event
tickets (direct sales or auctions).

> [!NOTE] The content displays changes based on the dynamic parameters in the
> URL, such as the user ID, using
> [Next.js dynamic routes](https://nextjs.org/docs/pages/building-your-application/routing/dynamic-routes).

### Backend

### API

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js
  features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out
[the Next.js GitHub repository](https://github.com/vercel/next.js/) - your
feedback and contributions are welcome!
