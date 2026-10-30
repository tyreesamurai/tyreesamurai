# Hey, I'm Tyree

I'm a Senior Software Engineer at Clarity Innovations. Before that I was a DevSecOps Developer at Sabel Systems, where most of my days were spent on Kubernetes, GitOps, CI/CD pipelines, and security tooling. I studied Computer Science (Software Engineering) at Virginia Commonwealth University.

This account is where my personal projects live. Most of them run on a homelab I'm building at home, and the idea behind all of it is pretty straightforward: build software that my fiancée and I actually use every day, and hold it to the same standard I'd hold production work to.

## What I'm working on

**The homelab.** A k3s cluster that hosts my own apps alongside the usual self-hosted services. It's managed with GitOps through Flux, so the whole cluster lives in code and can be rebuilt from a repo. After some hardware trouble with my old server I'm rebuilding everything on new hardware, which is also why older repos are disappearing and new ones are taking their place.

**Auth middleware.** The first thing going on the new cluster. One service that sits in front of every app, handles authentication, strips any identity headers coming in from outside, and sets trusted ones before a request reaches the app. Each app can rely on those headers instead of reinventing auth on its own.

**Then the apps**, rebuilt on top of that foundation:

- **Recipes**: keep and organize recipes, share them with other people, and turn a set of recipes into a shopping list.
- **Finance dashboard**: personal budgeting and tracking that's actually pleasant to use long term.
- **Task board**: a kanban board that leans closer to Jira than a typical todo list.
- **A mobile game**: one that means a lot to my fiancée and me, built so the two of us can play it together.

Across all of them, the focus is real multi-user support and apps that work together, so sharing a recipe or a board with someone is a first-class feature and not an afterthought.

## What I build with

- **Platform:** Kubernetes (k3s), Flux, Traefik, Sealed Secrets, Cloudflare Tunnel
- **Apps:** Go, TypeScript, Next.js, Bun, PostgreSQL, Drizzle
- **Delivery:** GitHub Actions, Trivy, Semgrep
- **Observability:** Prometheus, Grafana

## Find me

Portfolio: [tyreesamurai.github.io/portfolio](https://tyreesamurai.github.io/portfolio)

Thanks for stopping by.
