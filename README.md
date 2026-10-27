# J-MUSIC

A responsive, single-page music discovery website.

The public Admin preview is available at `admin.html`. It contains sample dashboard data and front-end-only review actions; it is not a secure or connected admin system.

## Run locally

Open `index.html` in a browser. The music player uses demo audio. User sign-up and login use Supabase Auth after the project is configured; artist forms are still a UI demonstration.

## Configure user sign-up

1. Create a Supabase project and open **Project Settings → API**.
2. Copy the project URL and the public anon/publishable key into `supabase-config.js`.
3. In Supabase **Authentication → URL Configuration**, set the site URL to `https://onuja070-lang.github.io/J-MUSI/` and add `https://onuja070-lang.github.io/J-MUSI/` to the redirect URLs.
4. Configure Supabase email delivery and confirmation settings. By default, new users may need to confirm their email before logging in.

The anon/publishable key is intended for browser use. **Never put a Supabase service-role/secret key in this website or its public repository.** Add only `supabase-config.js` values that are safe to publish.

## Publish with GitHub Pages

1. Push the contents of this folder to the `main` branch of `onuja070-lang/J-MUSI`.
2. In the repository, open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/(root)`, then save.
4. After GitHub Pages finishes deploying, the site will be at `https://onuja070-lang.github.io/J-MUSI/`. The dashboard preview is at `https://onuja070-lang.github.io/J-MUSI/admin.html`.
