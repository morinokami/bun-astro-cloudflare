# bun-astro-cloudflare

https://bun-astro-cloudflare.pages.dev/

This is an [Astro](https://astro.build/) project built with [Bun 1.0](https://bun.sh/blog/bun-v1.0) and deployed to [Cloudflare Pages](https://pages.cloudflare.com/).

## How I created this project

1. Create a new Astro project with `bunx create-astro`:

   ```sh
   $ bunx create-astro

   ╭─────╮  Houston:
   │ ◠ ◡ ◠  Let's build something awesome!
   ╰─────╯

    astro   v3.0.12 Launch sequence initiated.

      dir   Where should we create your new project?
            ./bun-astro-cloudflare

     tmpl   How would you like to start your new project?
            Use blog template
         ✔  Template copied

     deps   Install dependencies?
            Yes
         ✔  Dependencies installed

       ts   Do you plan to write TypeScript?
            Yes

      use   How strict should TypeScript be?
            Strict
         ✔  TypeScript customized

      git   Initialize a new git repository?
            Yes
         ✔  Git initialized

     next   Liftoff confirmed. Explore your project!

            Enter your project directory using cd ./bun-astro-cloudflare
            Run bun run dev to start the dev server. CTRL+C to stop.
            Add frameworks like react or tailwind using astro add.

            Stuck? Join us at https://astro.build/chat

   ╭─────╮  Houston:
   │ ◠ ◡ ◠  Good luck out there, astronaut! 🚀
   ╰─────╯
   ```
2. Configure build settings and environment variables on Cloudflare Pages:
   - Build command: `bun run build`
   - Build output directory: `dist`
   - Environment variables:
     ```
     SKIP_DEPENDENCY_INSTALL=true
     UNSTABLE_PRE_BUILD=asdf plugin add bun && asdf install bun latest && asdf global bun latest && bun install
     ```

## References

- [Hello from Bun!](https://blog.otterlord.dev/posts/hello-from-bun/)
